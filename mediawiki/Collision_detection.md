This article describes '''Collision Detection''' '''(CD)''' schemes that were, are or should be implemented in ''SuperTux''

There's a very good introduction into collision detection techniques at http://www.metanetsoftware.com/technique/tutorialA.html
Make sure you've read that if you want to work on collision detection.

== New Collision Detection ==

We're currently (July 2006) in the process of rewriting some parts of the collision detecion. Here are some random notes on how it works:

=== Simple BoundingBox / Triangle tests ===
We don't do any complicated [[Sweep collision algorithms|sweep tests]] anymore, but simply test the destination positions of objects. When pushing objects out of collisions we also mostly ignore object movement now and simply push the object out of the collision in the shortest way possible. We don't sort collisions by time anymore, but try to resolve all collisions at once. The staged approach of the old system remains though.

=== Several Collision Detection Phases ===
We do collision detection in several phases with different groups of [[game object|object]]s with slightly different characteristics each time. Currently defined collision groups:

 enum CollisionGroup {
  /** Objects in DISABLED group are not tested for collisions */
  COLGROUP_DISABLED,
  /**
   * "default" is moving object. [[MovingObject]]s get tested against all other
   * objects and against other movingobjects
   */
  COLGROUP_MOVING,
  /**
   * a Moving object, that is not tested against other MovingObjects (or other
   * MovingOnlyStatic objects), but is tested against all other objects.
   */
  COLGROUP_MOVING_ONLY_STATIC,
  /**
   * Doesn't move and isn't explicitly checked for collisions with other
   * objects (but other objects might check with this)
   * The difference to COLGROUP_TOUCHABLE is that we can do multiple
   * collision response tests in a row which is needed for static object
   * that tux walks on. The results for collisions with STATIC objects
   * are also sorted by time (so that the first hit gets handled first).
   *
   * Use this for static obstacles
   */
  COLGROUP_STATIC,
  /**
   * Isn't explicitly checked for collisions with other objects. But other
   * objects might check with this object.
   * Difference to COLGROUP_STATIC is that collisions with this object are
   * only tested once and collision response is typically not handled
   *
   * Use this for touchable things like spikes/areas or collectibles like
   * coins
   */
  COLGROUP_TOUCHABLE,
  /**
   * Should be used for tilemaps
   */
  COLGROUP_TILEMAP
 };

Current collision detection Phases:

# COLGROUP_MOVING vs. COLGROUP_STATIC, this handles all collisions against solid objects (see below for details)
# COLGROUP_MOVING vs tile attributes, handles collisions against tilemap and reports touched tiles with special attributes (like spike). This is a separate phase to avoid collisions with spikes and similar stuff that are avoided by resolving the solid collisions.
# COLGROUP_MOVING vs COLGROUP_TOUCHABLE handles collisions of objects vs. touchable objects like coins/firefly.
# COLGROUP_MOVING vs COLGROUP_MOVING we finally handle inter-object collisions

=== Collisions with solid objects ===
Collisions with solid objects are handled separately before all other collisions. We use several tricks there:

* Constraints: We calculate constraints into the left, right, top, bottom position, so that we can detect cases where tux gets crushed between 2 objects
* Do collision detection into Y direction before doing it into X direction. That's the only way to avoid a collision on the right side in cases like picture 1.
* We adjust tuxs position slightly when he only touches objects lightly. This helps when trying to jump through small holes and when running over 1 tile wide holes. (See picture 2,3)

<gallery>
Image:Colldet1.png|Picture 1: Typical walking to the right situation
Image:Colldet0.png|Picture 2: Typical Collision Detection situation
Image:Colldet2.png|Picture 3: 1 tile hole problem
Image:Supertuxvsmario2.png|Picture 4: Adjustment when sliding along edges
</gallery>

=== Sketch of the algorithm ===

# Calculate desired destination position of all objects
# For each object in MOVING_OBJECT group do: (solid phase)
## Calculate top/bottom constraints you handle y-movement only. Adjust destination position to the constraints. (but don't report crushes yet)
## Calculate left/right constraints with full object movement. Adjust desination position to the constraints. Report a crush if not enough horizontal space is left.
## Calculate top/bottom constraints and report a crush if not enough vertical space is left
# For each object in MOVING_OBJECT group do: (tile attribute phase)
## if the destination position touches any tiles with special attributes: report a collision (call object->collision_tile)
# For each object in MOVING_OBJECT group do: (touchable phase)
## For each object in TOUCHABLE group do:
### If the 2 objects intersect report a collision (object1->collision and object2->collision is called)
# For each object in MOVING_OBJECT group do: (inter-object phase)
## For each object in MOVING_OBJECT group do:
### if the objects intersect report a collision (call object->collision and object2->collision) and push objects out of the collision depending on the rerturned policy from the collision calls.
# Move all objects to their destination positions

TODO: Sketch the algorithm for calculating solid constraints

=== Problems ===

The following 2 cases always results in tux ending in a crushed situation. No nice solution for these cases has been proposed yet (except avoiding these situations in levels, which should be easy).

The first problem is currently worked around by relaxing the crushed condition a bit.

<gallery>
Image:Colldet_problem1a.png|Problem 1a
Image:Colldet_problem1b.png|Problem 1b
</gallery>

[[Category:Game Engine]]
[[Category:Game Engine]]