[[Template:Navbox Milestone 2 Design Document]]

[[Template:nextversion]]
== Code Tasks ==
* properly GPL'ify the supertux-editor (COPYING file, GPL headers, etc.)
* SDL2 migration (and all related side effect)

== Sound and Music Tasks ==
* Improve the sounds
* Compress music more. The 40 MBytes of music make up two thirds of the source tarball.

== Graphics / Sprites ==
* Create SuperTux idle animations (<del>stage1: blinking with the eye,</del> stage2: tipping with the foot, stage3: scratching the head)
** <small>I've added the code for idle animations, we just need the graphics now. The blinking animation already exists, but it needs some tweaking - [[User:Sik0fewl|sik0fewl]] 06:25, 16 June 2008 (UTC)</small>
** [https://supertux.lethargik.org/bugs/view.php?id=681]
* when Tux dies he can fly behind blocks instead of in front of them, drawing order bug
* Tux isn't centered properly to his collision box
* repair jump Tux sprite (to dark black) (Grumbel)
* do a 32x32 top-down water animation for the worldmap
** use these tiles [https://supertux.lethargik.org/bugs/view.php?id=852]
* finish [[cannon]] graphics, also snowball graphics, death, etc (Grumbel)
* [[Snowman]] graphics (death animation, turn-around graphics) (Grumbel)
* [[Owl]] graphics (basically placeholder graphics right now) <small>—[[User:Octo|octo]] 07:53, 9 March 2010 (UTC)</small>
* some decor for ice tiles, cracks and stuff (Grumbel)
* finish icecrusher graphics
* deep snow tiles
** [https://supertux.lethargik.org/bugs/view.php?id=911]
* icicle graphics for decoration purpose
** [https://supertux.lethargik.org/bugs/view.php?id=911] an okay job, but not the best -CT.da'Bomb
* animate minibomb
* think of a new way to represent the exit area (snow molted with smooth ground below or so)
* add turn-around animation for smart-snowball

== Editor / Developer Conveniences ==

*# directly accessible powerups
* finish editor improvements (MatzeB)
* editor doesn't align [[Cannon]] and [[Krush and Krosh]] properly (grid is wrong)
** I think it's using the 0,0-position of the ''image'' to align objects, not the ''hitbox''. —[[User:Octo|octo]] 07:50, 9 March 2010 (UTC)

== Meta / Organization ==
* create a timeline what shall be done and when — [[Milestone 2 Design Document/Timeline]]
* discuss in the meetings what shall be done over the coming week — [[Next Meeting Agenda]]

== Menu System / Game Configuration ==
* add gamma control to the option menu, see: int SDL_SetGamma (float redgamma, float greengamma, float bluegamma);
* make aspect ratio option menu thing work
* need to properly auto-detect and set aspect ratio on games first startup (i.e. on a 1280x1024 screen aspect must be set to 5:4, not 4:3)
* option menu entries are currently not in sync with gameconfig
* add scale-with-window option to magnification or something like that
* make left/right change an option in the menu, let enter apply it (needed for fullscreen)

== Levels / Scripting / Gameplay ==
* level startup needs a fade-in, so does game startup, level abort and a few other places
* add all fade-in/out effects to DisplayEffect
* camera vertical scroll doesn't work properly in a small window (i.e. it doesn't move at all)

== Other ==
* aspect ratio init code (Grumbel)
* think about peeking in relation to large screen size
** <small>Maybe disable peeking if the resolution is at a certain size or greater? Tux would just be centered. [[User:Sik0fewl|sik0fewl]] 18:34, 30 April 2009 (UTC)</small>

== Enemies ==
* fix and cleanup all the enemy names - see [[Milestone 2 Design Document/Enemies]] for new names
** A beginning has been made by renaming ''Kamikaze Snowball'' to [[Snowshot]]. There's not much consensus about the other changes though, see [[Meeting 2010-02-27]]. --[[User:Octo|octo]] 07:01, 5 March 2010 (UTC)
* AngryBonusBlock: Have a bonus block type that comes to life when tux jumps against it and then chases Tux
:Break the "only good stuff from bonus blocks" and "same look same behaviour" rules? --[[User:WolfgangB|WolfgangB]] 01:27, 25 May 2008 (UTC)
::Secret Maryo has a poisonous mushroom... if they break the rules, why not us? Also, bonus blocks already have varied behaviors. --[[User:Mathnerd314|Mathnerd314]] 04:23, 7 September 2008 (UTC)
* create an enemy type that doesn't just walk straight into one direction, but does something different depending on Tux direction (ninja)
** <small>Is this a dupe of the Crystallo proposal for week 4? - [[User:Sik0fewl|sik0fewl]] 19:58, 15 May 2008 (UTC)</small>
*** <small>No, this enemy is intelligent (reacts to Tux) --[[User:Mathnerd314|Mathnerd314]] 20:43, 19 March 2010 (UTC) </small>
* [[Mr. Bomb]]: let the fuse burn after one touched it
* [[Flying Snowball]]: Remove randomness, should be periodic and predictable
* [[Flying Snowball]]: Change timings to match that of Milestone1
* [[Flying Snowball]]: smoke effect for the motor seem to be to seldomly triggered
* [[Krush and Krosh|Icecrusher]]: gravitation instead of linear, facial expression.
*: Gravitation has been done in [[Template:Revision|6403]]. —[[User:Octo|octo]] 19:19, 26 February 2010 (UTC)
* [[Krosh]] (big icecrusher): add a larger version of [[Krush]] (the icecrusher), twice the size (4x4 files)

== Postpone to Milestone 3 ==

These are items that can be postponed until milestone 3, but are still welcome for milestone 2.

===Code Tasks===
* separate lisp reader, tinygettext and other libraries properly out of SuperTux

===Editor / Developer Conveniences===
* optimize the build process, building SuperTux currently takes ages (I don't see how we could speed it up..., MatzeB)

===Levels / Scripting / Gameplay===
* fix console command set_game_speed() so that it doesn't slow down the console
* replace "you found a secret area" with a special sound (Wansti)
**why I like it the way it is. -ctdabomb
* General: Do something about the walking speed, feels wrong at the moment, maybe a bit slower
===Other===
* create SuperTux .xo Activity for OLPC (Grumbel)
* Have particle throwing starting enemies (fireflower like)
* add sprite scaling

== Finished ==
* document the behaviour of all badguys to be used in Milestone2 along with how they interact with each other - [[Milestone 2 Design Document/Enemies]]
* reorganize the editor to something more like this [http://pingus.seul.org/~grumbel/tmp/md5/68413a9004b402c38a8dd24bf785e2f0-supertux-editor-mockup.png SuperTux-Editor MookUp]
* Editor: show tile attributes in editor, especially for non-solid and unisolid there is often a very similar solid tile. Either add special editor-images for unisolid, some overlay icon for the tile selector <strike>or at least a hint in the status bar</strike>. (status bar done)
* General: Get rid of enemies stacking on top of each other
** <small>What does that mean? —[[User:Octo|octo]] 07:45, 9 March 2010 (UTC)</small>
** <small>I'm not sure if this issue still exists, but when one badguy falls on top of another and can't move left or right he will get stuck on top. - [[User:Sik0fewl|sik0fewl]] 16:53, 19 March 2010 (UTC)</small>
* SuperTux should stand on the ground when a level starts, not fall down (move all spawnpoints to 1 tile above ground)
* paint tutorial board for backflip
* draw a bigger arrow for when Tux is jumping out of the screen
** [[https://supertux.lethargik.org/wiki/Image:Airarrow.png]]
* Create more music tracks for IcyIsland or add BlastOffTek's pack or the music by semaJD [https://supertux.lethargik.org/bugs/view.php?id=875].
**semajd's music is added, we just need to add the music to levels
* [[Mr. IceBlock]]: transparency looks horrible on dark backgrounds, Wiki had a better looking version floating around
* [[Haywire]]: new bomb type (crazy pink bomb) that runs around after being touched
** Initial version is done. Waiting for feedback and improvements. See [[Milestone 2 Design Document/Enemies]] --[[User:Octo|octo]] 07:08, 5 March 2010 (UTC)
* [[Mr. Bomb]]: Roll back to behavior of [[Milestone 1]], get rid of particle effects
** Particle effects are currently deactivated in [[Template:SvnFile|src/object/explosion.cpp]]. --[[User:Octo|octo]] 07:08, 5 March 2010 (UTC)
* add PNG support for screenshots, BMP support currently broken
** <small>What's wrong with BMP support? It seems to work for me - [[User:Sik0fewl|sik0fewl]] 06:11, 13 June 2008 (UTC)</small>
*** ACK, BMP-based screenshots work, at least with the SDL renderer. --[[User:Octo|octo]] 06:53, 5 March 2010 (UTC)
* at large resolutions frame rate starts to sucks, but CPU usage continues to stay very low, is that a artifact of GPU use or something wrong with our timing/frameskipping code?
** <small>Fixed?</small>
* bug: can't walk left and jump while pressing ctrl, when going right the same works, might be keyboard specific (Microsoft Natural Ergonomic Keyboard 4000 USB suffers from it, on the same PC a PS/2 keyboard works, maybe kernel driver bug), capslock is bound to ctrl and ctrl is bound as action key, using space for action works as workaround (Grumbel)
* peeking should stick instead of jumping back or jumping back should be limited to normal range that the camera can do
** <small>I think this is fixed or at least better now? - [[User:Sik0fewl|sik0fewl]] 18:34, 30 April 2009 (UTC)</small>
* <strike>add an cmd option --default</strike> and/or a menu entry "Reset to Default" to reset any changes to resolution or aspect ratio (or something along those lines) (cmd done, WolfgangB)
* <strike>create an overview of the current levels</strike> — [[Milestone 2 Design Document/Levels]]
*: —[[User:Octo|octo]] 07:24, 11 January 2011 (UTC)
*# <strike>New unisolid snow tiles</strike>
*# Parallax backgrounds
*#: <small>That's heavily used in ''Above the Arctic Skies''. —[[User:Octo|octo]] 07:22, 11 January 2011 (UTC)</small>
*# <strike>Sector/Scripting use</strike>
*# <strike>Crystallo and IceBlock badguys</strike>
*# <strike>Add-ons + manager (To distribute these new levels, of course!)</strike>
*#: [[Incubator Island]] and [http://verplant.org/supertux octo's levels] should do most of this
*# <strike>Slopes and background tiles</strike>
*# Moving platforms <strike>(ice platforms haven't been used yet...)</strike>
*# <strike>Climbable ladders</strike>
*#: <small>Ladders are not in the Milestone&nbsp;2 document, but in Milestone&nbsp;3. —[[User:Octo|octo]] 07:22, 11 January 2011 (UTC)</small>
* try to fix white-lines around graphics problems (MatzeB)
** Where? -CT. da'Bomb
* butt jump animation (Grumbel)
* backflip animation (Grumbel)
* Crystallo dead/dying sprites
* Empty top/middle/bottom background image string should be handled as transparent image (more parallax backgrounds)
* write TexturePacker to place multiple images on a single texture (better use of texture space and fixes bug with tiles having junk on the edge)
** <small>Fixed with non_power_of_two? --[[User:Mathnerd314|Mathnerd314]] 20:43, 19 March 2010 (UTC)</small>
* Malformed UTF-8 sequences should not be handled as fatal error, just insert '?' instead (happens with German translation) (fixed? MatzeB)
* create some playable test levels for new stuff
** <small>Anything in particular? - [[User:Sik0fewl|sik0fewl]] 20:07, 15 June 2008 (UTC)</small>
*:Try these, since they're probably most noticeable to Milestone1 users: --[[User:Mathnerd314|Mathnerd314]] 04:23, 7 September 2008 (UTC)
* remove border from menu screen or make it scalable for different resolutions
* remove pictures from credits, looks to uneven that way 
:<small>Really? I like the pictures. --[[User:WolfgangB|WolfgangB]] 19:00, 29 April 2008 (UTC)</small>
:<small>I do too. --[[User:Mathnerd314|Mathnerd314]] 00:05, 6 July 2008 (UTC)</small>
* replace old bomb with new bomb sprite
* <strike>change game back to use Milestone1 single-sprite SuperTux (done)</strike>
* <strike>switch supertux-editor over to CMake? (done, is now a simple Makefile)</strike>
* <strike>when BigTux ducks, the camera moves/jumps, but should stand still (fixed, MatzeB)</strike>
* <strike>there should be an script command to change the game speed (i.e. run in slowmotion)</strike>
* <strike>Tux isn't animated when he dies (caused by "grow-right" and then "gameover" being set over and over again, so framecount is always 0) - sik0fewl</strike>
* <strike>bring back single-sprite SuperTux (done)</strike>
* <strike>jump with keyboard up (done, WolfgangB)</strike>
* <strike>figure out a Jumpy replacement (Grumbel)</strike>
* <strike>rename trunk/supertux-sharp to trunk/supertux-editor to make it clear that it is the primary editor (MatzeB)</strike>
* <strike>Stay-on-platform snowball (done, WolfgangB)</strike>
* <strike>snowball-launcher (done. WolfgangB)</strike>
* <strike>integrate snowjumpy</strike>
* <strike>use pink snowball for stay on platform, use normal snowball for straight forward walk</strike>
* <strike>add a "scan for joysticks" to the "No Joysticks found" in "Setup Joystick" to allow hotplugging (done, WolfgangB)</strike>
* <strike>peeking should work in in both X and Y at the same time (for use with second analog stick on todays gamepads) (done, WolfgangB)</strike>
* <strike>add a way to enable the console from within the game</strike>
* <strike>the menu should shrink instead of just disappear - sik0fewl</strike>
* <strike>add a set_gamespeed() so that the game can run in slow motion for debugging '''[done]'''</strike>
* <strike>fix default peek keybindings, seem to be wrong</strike>
* <strike>Esc should pop the current menu (ie, back), not escape the entire menu - sik0fewl</strike>
* <strike>bomb can't be carried, but should be able to</strike> - sik0fewl
* <strike>make F10 toggle print-fps</strike> - sik0fewl
* <del>Spiky: Shouldn't alway sleep, either make it an option or better make a new enemy type for sleeping behaviour</del> (Thats already done that way, there is [[Spiky]] and [[Sleeping Spiky]]).
* <del>Spiky: Walkcycle animation looks broken, there is a frame missing</del>
* <del>Snowball(normal): Animation ruined</del>
* <del>Snowball(stay-on-platfrom): Replace with female snowball graphic</del>
* <del>Bomb: Replace graphic with new bomb graphic</del>
* <strike>fix editor so that it works without a mouse wheel</strike> (done, WolfgangB)
* <del>Translations for Chinese and Russian (Cyrillic)</del>
* <del>InfoBox crashes when Text doesn't start with a marker character</del>
* <del>create ice-spikes graphics (Grumbel)</del>
* <del>create ice-tiles graphics (Grumbel)</del>
* <del>create angry ice-block graphics (Grumbel)</del>
* <del>Editor: sort (new) layers by z-value</del>
* <del>peeking up/down keys seem to be unbound by default</del>
* <del>fix/add/cleanup menu entry names and descriptions to be better understandable</del> - '''[done, but should probably be reviewed before release]'''
* <del>create mountain and night background</del>
* <del>create proper background tiles for level22</del> - all you need are the blue bg tiles and maybe some unisolid ones
* <del>new enemy type with more interesting walking pattern (follows Tux as long as Tux doesn't look, walks forward and backward, etc.), see Crystallo for a possible sprite</del>
* <strike>add 'recent files' to level editor</strike>
* <strike>can't run while carrying an object, but should be able to</strike>
:No, that is on purpose: Tux can't run when carrying heavy objects. So you can control where the player can not bring eg. the trampoline without a artificial "no stuff behind this line" object. Any reason why Tux should be able to run when lugging objects almost as big as himself? --[[User:WolfgangB|WolfgangB]] 01:22, 25 May 2008 (UTC))  
:: With *large* objects I might agree, but an Iceblock or any other 32x32 one isn't a large object, it just robs the gameplay from being dynamic. -- [[User:Grumbel|Grumbel]] 17:13, 28 May 2008 (UTC)
::: The speed limiting code has been deactivated in [[Template:Revision|6540]]. --[[User:Octo|octo]] 06:51, 5 March 2010 (UTC)
* <strike>General: Get rid of bouncing snowballs killing normal snowballs and other unintended behaviour</strike>
** Fixed in [[Template:Revision|6554]] —[[User:Octo|octo]] 07:35, 9 March 2010 (UTC)
* <strike>[[Flying Snowball]]: Add acceleration/deceleration instead of linear up and down</strike>
*: Isn't this the current behavior ([[Template:Revision|6402]])? —[[User:Octo|octo]] 18:22, 26 February 2010 (UTC)
* <strike>background graphics glitch at non-800x600 resolutions (black line where background tiles), reason for this is that background gets copied to a 1024x1024 texture with a black border, at non 800x600 resolutions the right edge becomes blended with this black border, need to add 1px border around the texture to fix this blending bug (alternative: use GL_NEAREST instead of GL_LINEAR)</strike>

[[Category:Development]]