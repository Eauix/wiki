__NOTOC__

== Summary ==

A ScriptedObject is basically a SuperTux object that can be scripted to move around and animate.

== Instances ==
ScriptedObjects are created by being defined in level files. Each scripted object will be exposed under its name to the scripting engine. Access through the console is realised via the <tt>sector</tt> object.

=== Example ===

Example of a definition:
 <pre>
  (scriptedobject
    (x 2291)
    (y 1275)
    (name "SUPERTUX")
    (sprite "images/creatures/tux_big/tux.sprite")
    (layer 100)
    (visible #t)
    (physic-enabled #t)
    (solid #t)
  ) 
 </pre>

The above object will be exposed under the name <tt>SUPERTUX</tt> in the scripting engine. Example usage:

 <pre>
  // This script will make tux look and walk left/right (this should make him appear
  //   "upset")
  SUPERTUX.set_action("stand-right");
  wait(2);
  SUPERTUX.set_velocity(200,0);
  wait(0.3);
  SUPERTUX.set_velocity(0,0);
  wait(0.4);
  SUPERTUX.set_action("stand-left");
  SUPERTUX.set_velocity(-200,0);
  wait(0.3);
 </pre>

The object can be accessed from the console <tt>sector.SUPERTUX</tt>.

== Methods ==
{| class="objectlist"
! class="method"| set_action(string animation)
| Activates the sprite's action specified in <tt>animation</tt>.
|-
! class="method"| get_action()
| Returns the name of the sprite's current action.
|-
! class="method"| move(float x, float y)
| Moves the object by <tt>x</tt> units to the right and <tt>y</tt> down relative to its current position.
|-
! class="method"| set_pos(float x, float y)
| Basically identical to <tt>move</tt>, except its relativity to the sector origin.
|-
! class="method"| get_pos_x()
| Returns the X coordinate of the object's position.
|-
! class="method"| get_pos_y()
| Returns the Y coordinate of the object's position.
|-
! class="method"| set_velocity(float x, float y)
| Makes the object move in a certain direction (with a certain speed) given by the <tt>x</tt> and <tt>y</tt> coordinates.
|-
! class="method"| get_velocity_x()
| Returns the X coordinate of the object's velocity.
|-
! class="method"| get_velocity_y()
| Returns the Y coordinate of the object's velocity.
|-
! class="method"| enable_gravity(bool gravity_enabled)
| Shows or hides the object according to the value of <tt>gravity_enabled</tt>.
|-
! class="method"| gravity_enabled()
| Returns true if the object's gravity is enabled, false otherwise.
|-
! class="method"| set_visible(bool visible)
| Shows or hides the object according to the value of <tt>visible</tt>.
|-
! class="method"| is_visible()
| Returns true if the object is visible, false otherwise.
|-
! class="method"| set_solid(bool solid)
| Makes the object solid according to the value of <tt>solid</tt>.
|-
! class="method"| is_solid()
| Returns true if the object is solid, false otherwise.
|-
! class="method"| get_name()
| Returns the name of the object
|}

== Constants ==

None

[[Template:Navbox Scripting reference]]
[[Category:Scripting Reference]]