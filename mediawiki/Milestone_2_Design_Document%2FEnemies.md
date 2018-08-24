[[Template:Navbox Milestone 2 Design Document]]
__NOTOC__
This page shall describe all enemies, old and new, in as much detail as possible. We also need to settle down on proper names for enemies, since currently there is a lot of confusion. If you want see on real names, click [[real_badguys_names|here]].

<br clear="all" />

== [[Snowball]] ==

[[Image:SnowballSprite.png|right]]

Snowball is a straight forward walking enemy, when reaching an edge he will fall down and continue walking on the platform below. Jumping on him will squish him and thus kill him.

'''Status:''' Basic behavior is implemented, could however be improved with additional animations when turning around or when falling from a cliff. -- [[User:Grumbel|Grumbel]] 09:41, 23 February 2010 (UTC)
<br clear="all" />

== <strike>[[Mrs. Snowball]]</strike> smartball ==

[[Image:SmartSnowballSprite.png|right]]

Mrs. Snowball behaves like a normal [[Snowball]], but instead of walking off a platform she will turn around when reaching the edge.
<br clear="all" />

== [[Snowman]] ==
[[Image:SnowmanSprite.png|right]]
A snowman enemy shall be added, a snowman is build out of a base body combined with a snowball head, if the body is destroyed, the snowman turns into a snowball. Alternative: Let the head get destroyed and the body turn into a snowball that can be rolled around.

'''Status:''' A very basic Snowman prototype is in [[SVN]], but lacks death animation and the whole separation behavior. Could use fists instead of balls as hands. -- [[User:Grumbel|Grumbel]] 09:39, 23 February 2010 (UTC)
: Basic separation behavior has been implemented in [[Template:Revision|6418]]. We're missing a graphic for the Snowman's body though. —[[User:Octo|octo]] 19:07, 27 February 2010 (UTC)
: The snowman's body is now falling down when he's squished. [[User:Grumbel|grumbel]] wants to make a proper death graphic though. --[[User:Octo|octo]] 22:20, 2 March 2010 (UTC)
<br clear="all" />

== <strike>Bouncy, </strike>Bouncing Snowball ==

[[Image:BouncingSnowball.png|right]]
The [[Bouncing Snowball]] is a leg-less Snowball that jumps around like a ball.

'''Status:''' Jump height and width could be tweaked a bit to make it easier to stand below it. Placement in the levels is the biggest problem, should only be used in open spaces, not closed ones where bouncing becomes unpredictable. -- [[User:Grumbel|Grumbel]] 09:48, 23 February 2010 (UTC)
<br clear="all" />

== <strike>Avior, Dex,</strike> Flying Snowball ==
[[Image:Flyingsnowball.png|Flying Snowball|right]]
The flying snowball has a propeller at his bottom which keeps him floating in the air. Due to Nolok's hurry, the motor is inefficient and varies in effectiveness, causing the flying snowball to move up and down while coughing out smoke and possibly other debris.

'''In need of a "good" name.'''

What about Mr. Flyball?--[[User:Noporque|Noporque]] 09:00, 10 April 2010 (UTC)

Here are some ideas: Flyper, Propeller, Gadget, and Floatall. I'm Agent Spook, and I'm just trying to help.

<br clear="all" />

== <strike>[[Snowshot]]</strike> kamikazesnowball ==
[[Image:Kamikaze-left2.png|Snowshot|right]]
The [[Snowshot]] comes out of a [[Cannon]]. He is very angry, or very "wise", and so can levitate through the force of his will. He is so concentrated on this, however, that he cannot turn or adjust his velocity.

'''Status:''' There is MrRocket in SVN which should be recycled and turned into a Snowshot. There is also a cannon that can be reused after its graphics have been replaced. -- [[User:Grumbel|Grumbel]] 11:55, 23 February 2010 (UTC)
: There's a Kamikaze Snowball in SVN, too. "Mr. Rocket" has been removed in [[Template:Revision|6408]]. —[[User:Octo|octo]] 21:03, 26 February 2010 (UTC)
<br clear="all" />

== [[Mr. IceBlock]] ==

[[Image:MrIceblockSprite.png|right]]
Like Snowball, Mr. IceBlock is a simple straight forward enemy. He will not stay on platforms. When jumped upon he will get knocked out and become a portable item that one can use to throw at other enemies.
<br clear="all" />

== <strike>Fuse,</strike> MrBomb ==

[[Image:Mrbomb.png|right]]
The base behavior of [[Mr. Bomb]] is similar to the normal Snowball, except that when hit he doesn't get squished, but his fuse starts burning. After ~5 seconds he then explodes. While the fuse is burning he doesn't move, but instead can be carried around like an iceblock. Throwing MrBombs is more like a normal throw, not like MrIceblock getting kicked.

'''Status:''' Explosion timing is wrong, should be long enough to grab it and carry it around. -- [[User:Grumbel|Grumbel]] 09:51, 23 February 2010 (UTC)

<br clear="all" />

== [[Haywire]],(Crazy Fuse) ==

[[Image:MrBombCrazy.png|right]]

When the fuse isn't burning Haywire looks similar to a normal Bomb except color and face.
When the fuse of Haywire gets activated he starts to run around, maybe chasing Tux. He can't be carried around. Jumping on him when the fuse is burning will cause Tux to bounce and Haywire to be stunned for a short moment (fraction of a second).

'''Status:''' An initial version is available since [[Template:Revision|6443]].

<br clear="all" />

== [[Crystallo]] ==

[[Image:Crystallo.png|right]]

Again a very basic enemy, but unlike the Snowball he doesn't walk around in a straight pattern, but walks forward and backward around a fixed position. It is a stationary enemy.
<br clear="all" />

== [[Spiky]] ==

[[Image:SpikySprite.png|right]]
Spiky behaves like ''Mrs. Snowball'', i.e. he stays on platforms, but he carries a helmet which makes him invulnerable against jump attacks.

<br clear="all" />

== <strike>Sleeping Spiky</strike> Spiky ==

[[Image:SleepingSpikySprite.png|right]]
Sleeping Spiky sleeps, when Tux comes near he activates and behaves like a normal Spiky. (Grumbel: Not sure that guy is a good idea)
<br clear="all" />

== <strike>Recoil, SnowJumpy</strike> Jumpy ==

[[Image:SnowJumpySprite.png|right]]
[[Jumpy]] jumps up and down and stays stationary on the same position. His viewing direction might follow [[Tux]]. The spring should react when hitting the ground.

<br clear="all" />

== Ice Fish / [[Fish]] == 

[[Image:IceFish.png|right]]
Already in the code, but not much used in Milestone1 Levels. This badguy shouldn't be used in Icyland, it is a forest enemy. 
<br clear="all" />

== [[Owl]] ==
[[Image:Owl.png|right]]
A flying enemy that can carry things around and let them drop on Tux. One thing it is throwing might be ''SkyDive''.

Some initial code is available from the [[SVN]] repository since [[Template:Revision|6558]]. Graphics are still pretty much a to-do. —[[User:Octo|octo]] 17:25, 6 March 2010 (UTC)

<br clear="all" />

== [[SkyDive]] == 

[[Image:BombFish.png|right]]
An enemy that is let go by ''Owl'' and then falls down to the ground and explodes.

An initial version of this badguy has been committed to [[SVN]] in [[Template:Revision|6564]].

<br clear="all" />

== <strike>[[Krush and Krosh]]</strike> Icecrusher ==
[[Image:Iceblock.png|right]]

Krush and Krosh are enemies that are hanging on the ceiling. When [[Tux]] gets within one tile they will fall down and try to smash Tux. When hanging on the ceiling, Krush and Krosh'es eyes shall follow Tux. The face expression shall become angry when he is falling down.

'''Status:''' Needs a cool-down time after an attack, so it doesn't go up instantly. Needs particle effects when it hits the ground. Eyes should follow Tux. Should be larger, maybe 3x3 tiles or 4x4. Should accelerate while falling down, currently looks to much like constant velocity. -- [[User:Grumbel|Grumbel]] 09:54, 23 February 2010 (UTC)
: Acceleration has been fixed in [[Template:Revision|6403]]. —[[User:Octo|octo]] 19:38, 26 February 2010 (UTC)
: A cooldown timer has been added in [[Template:Revision|6405]]. —[[User:Octo|octo]] 19:49, 26 February 2010 (UTC)
<br clear="all" />

== ([[Cannon]]) Dispenser ==
[[Image:Dispenser rocket launcher.png|right]]
The cannon can be mounted on either static or rotatable pedestal. It shoots angry looking snowballs. It is indestructible.
[[SVN]] for non-captainsnowball/kamizazesnowball enemies
: The version in SVN can in fact shoot [[Snowshot]]s. Can this sentence be removed or do you mean something else? --[[User:Octo|octo]] 07:55, 27 February 2010 (UTC)
: I didn't find any mention of [[Captain Snowball]] in neither the Milestone 2 nor the Milestone 3 design documents. What's the status on him? --[[User:Octo|octo]] 07:55, 27 February 2010 (UTC)
:Captain snowball is used in several level in bonus 3 --[[User:giby|giby]] Fev 2014
<br clear="all" />

== [[Stalactite]] ==
[[Image:Falling.png|Stalactite|right]]
The stalactite stays stuck to the ceiling until Tux walks near it, then begins shaking. After a bit of shaking, it falls down in an attempt to hurt Tux, while also harming badguys that get in the way.

<br clear="all" />

== [[Flame]] ==
[[Image:Flame.png|Flame|right]]
The flame rotates around in a circle, hurting Tux when he gets too close. It is indestructible. Do we want it to come in a line of fire?

<br clear="all" />

== 295 ==
[[Image:up.png|right]]The spike isn't really an enemy, so much as an obstacle, but for some strange reason, it's in the creatures' image directory, but implemented as a tile. Currently the spike only hurts Tux, instead of insta-killing him as might be wanted, for example at the bottom of deep pits. Alternately, we could simply have shallow pits that are easy to jump out of. (but that still hurt Tux)

== [[Short Fuse]], <strike>Mini Bomb</strike> ==
[[Image:Short Fuse.png|right]]
[[Image:Minibomb.png|thumbnail|right|Mini-Bomb]]
The Mini-Bomb is an small version of the normal bomb, it approaches in groups most of the time and is aggressive, it however is non-lethal to Tux and only works to either distract him and throw him back.

A first version of this badguy has been added to [[SVN]] in [[Template:Revision|6511]].

Should "pop" like it was filled with air pressure air, not explode in fire, to make it clear that its not deadly.

<br clear="all" />

== Spitter (proposed) ==
[[Image:Spitter.png|thumbnail|right|Spitter]]
The spitter acts as walking dispenser, the enemy type that he can spit out might be limited to mini-bombs and similarly small enemies.
<br clear="all" />



== Yeti ==
[[Image:Yeti-concept.jpg|thumbnail|right|64px|Yeti]]
[[Image:Yetiapproach.png|thumbnail|left|Yeti Boss Cutscene]]

The Yeti is the boss that awaits Tux in the first castle. After entering the throne room Tux will find a letter in which Nolok tells Tux of the other castles in other worlds (see Milestone1 extro.txt). In the background there is a window. While reading the note one will see a shadow approaching the window and soon after the Yeti jumping through the window. The normal boss battle starts instantly after the jump.

Alternative: Sequence at end of castle: Tux find Yeti, Yeti jumps out of the window and flees
<br clear="all" />

== Gulpy, <strike>Eater</strike> (proposed) ==
[[Image:Eater.png|thumbnail|right|Eater]]
The Eater is a very small enemy, half the size of a snowball, he can however expand a lot. If Tux gets to close to him the Eater will open his mouth wide enough that he can devour Tux or even other badguys. He is not defeatable by jumping onto him, since he will then just eat Tux. Throwing stuff at him won't work either, since again he will just eat them.

: So how can you defeat Gulpy? As-is, he just seems to be a moving hurting platform. --[[User:Mathnerd314|Mathnerd314]] 23:28, 7 March 2010 (UTC)
::Maybe with starman--[[Special:Contributions/173.59.123.229|173.59.123.229]] 16:35, 23 December 2010 (UTC)
<br clear="all" />

<!-- Castle/Endgame badguys
[[Image:Flying-2.png|Mr. Rocket]]
[[Image:Dropper.png|Dispenser (Dropper)]]
[[Image:Standing-0.png|Skully Hop]]
[[Image:FishRed.png|Flame Fish]]
[[Image:Dart.png|Dart]]

[[Image:Jump-1.png|Nolok]] -->

[[Image:Minibomb-and-stuff.png|Milestone 2 Enemies]]

[[Template:Navbox Badguys]]
[[Category:Milestone 2]]
[[Category:Development]]