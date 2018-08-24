:''This page is about the class in the source code. For a list of objects available in the game, see [[Objects]].''

[[Template:Outdated]]
[[Image:gameobjects2.png|thumb|A diagram illustrating the planned design for the GameObjects]]
'''GameObject''' is a base class in the ''SuperTux'' source code. It is the most basic class for objects in the game. Nearly everything should inherit from this class, for instance [[badguy]]s, [[unstable tile]]s and [[trampoline]]s. All ''GameObjects'' are stored in a list by the engine.
This list will be traversed twice per frame. First the action function is called on each object, and then the draw function of each object is called.

The class also contains a flag that indicates if the object should be removed at the end of the frame. You can call <code>-&gt;remove_me()</code> to set this flag.

== Derived classes ==

=== InteractiveObject ===

These are objects you can interact with. The objects will have an area in the world. And you can send interaction events to them. Typical interaction events will be activate/push, ~EnterArea/touch, ~LeaveArea, hit with object

=== MovingObject ===

This class provides a position and functions for collision detection. All Moving objects are held in a separate list by the engine which is also traveled once (between action and draw calls) for collision detection.

== Class hierarchy ==
:''As of [[Template:Revision|6274]].''

* GameObject
** AmbientSound
** Background
** BouncyCoin
** BrokenBrick
** Camera
** DisplayEffect
** Electrifier
** EndSequence
*** EndSequenceFireworks
*** EndSequenceWalkLeft
*** EndSequenceWalkRight
** FallingCoin
** Fireworks
** FloatingImage
** FloatingText
** Gradient
** LevelTime
** Light
*** PulsingLight
** MovingObject
*** Block
**** BonusBlock
**** Brick
**** InfoBlock
**** InvisibleBlock
*** Bullet
*** Flower
*** MovingSprite
**** BadGuy
***** AngryStone
***** Bomb
***** BouncingSnowball
***** Dart
***** DartTrap
***** Dispenser
***** Fish
***** Flame
***** FlyingSnowBall
***** GhostTree
***** Jumpy
***** KamikazeSnowball
***** Kugelblitz
***** Mole
***** MoleRock
***** MrRocket
***** Plant
***** Root
***** SkullyHop
***** SpiderMite
***** Stalactite
****** YetiStalactite
***** Toad
***** Totem
***** TreeWillOWisp
***** WalkingBadguy
****** CaptainSnowball
****** Crystallo
****** Igel
****** MrBomb
****** MrIceBlock
****** MrTree
****** PoisonIvy
****** SmartBall
****** Snail
****** SnowBall
****** Spiky
****** SSpiky
****** Stumpy
****** WalkingLeaf
***** WillOWisp
***** Yeti
***** Zeekling
**** BicyclePlatform
**** Candle
**** Coin
**** Decal
**** Explosion
**** Firefly
**** GrowUp
**** IceCrusher
**** InvisibleWall
**** Ispy
**** MagicBlock
**** OneUp
**** Platform
***** HurtingPlatform
**** PneumaticPlatform
**** PowerUp
**** PushButton
**** Rock
**** ScriptedObject
**** SkullTile
**** Star
**** UnstableTile
**** WeakBlock
*** Player
*** TriggerBase
*** Wind
** Particles
** ParticleSystem
*** CloudParticleSystem
*** GhostParticleSystem
*** SnowParticleSystem
** ParticleSystem_Interactive
*** CometParticleSystem
*** RainParticleSystem
** RainSplash
** SmokeCloud
** SpecialRiser
** Spotlight
** SpriteParticle
** TextObject
** Thunderstorm
** TileMap
** worldmap::LevelTile
** worldmap::SpecialTile
** worldmap::SpriteChange
** worldmap::Teleporter
** worldmap::Tux

[[Category:Game Engine]]
[[Category:Game Object]]