This could be useful in underwater levels.

Before implementing swimming there are some details that need to be specified:

* What can Tux do in water?

Swim left, swim right, dive, and porpoise.

Tux could be able to move a lot faster in water than on land, and he could be able to jump higher when jumping out of a pool of water - like real penguins.

* How does he leave the pool, ie. how high can Tux jump while swimming?
** By jumping when near the surface.

* What happens to existing levels, especially in situations where the water is on the bottom of a shaft with no way to climb out?

== Breathing ==
I don't know if penguins can breath underwater, but maybe Tux need swim to surface to breath sometimes...
* They can hold their breaths for up to 12 minutes. Good enough?
**It depends on the penguin. Adélie's--like Tux--can hold their breaths for 15 minutes. I seriously doubt he would be underwater for that long. You probably won't be making a level as long as "Moving On," (an EXTREMELY long--7000+ length, level made by a friend) all the way below the surface of the water. --[[User:Julius Freezer|Julius_Freezer]] 04:32, 25 June 2009 (UTC)
== Proposal 1 ==

My idea of a cool swimming mode would be that as soon as Tux is in water, he jumps to the side so he lies on his belly (that's how penguins swim if you've ever watched them in the zoo :)
You could then control his angle with the up/down keys (something between facing 45° upward and 45° downwards). The left/right keys would be used to turn Tux 180°. Pressing the jump key would accelerate Tux a bit into the direction he is facing (the water will have a high friction). We could tweak controls a bit so that an optimum forward movement is achieved if you press the button for a long enough time (if you press it shorter then Tux won't get as much acceleration) and then release the button for a long enough time (Tux will only react to a 2nd push after some time has passed). For getting out of the water you would dive a bit deeper face upwards and accelerate so much that Tux springs out of the water onto the land, we could have an animation there we Tux lands on his belly on the land and then stands up. This would add an interesting touch to the game and not feel like more jumping and running. And it would feel like real penguins swimming.

The only problem here is that implementation isn't so easy :) We would have to think about the following points:
* We would need some new collision detection code to check collisions on rotated rectangles (it's not that hard actually, but would need some API redesign to support this and would need more smart thinking on how to push out objects from collisions)
* We would need a several new animations: Tux landing in water and switching to swim mode, Tux pushing water away with his feet, Tux gliding in water, Tux landing on his belly on the land and going into normal mode again. This would also bring us to the old problem, that we currently would have to do all animation twice for big and small Tux...
* We could even make good use of more animations: Tux getting hurt in water, Tux flapping his wings while doing a jump out of the water, Tux hitting a wall in water, Tux turning to the other side in water.

Does someone know games that have a similar concept?

:Yeah, i know a game that uses something similar, but there you *fly* using Jetpack in that way. See http://www.parallelrealities.co.uk/blobWars.php (Eek, you'll have to cheat to get jetpack fast, read through the page)
TODO: Create some sketches for this to better explain it

--[[User:MatzeB|MatzeB]] 11:24, 23 Oct 2006 (CEST)

Wario Land 2 for GB has this system:
* When Wario swims he lies on his belly
* Directional keys are used for moving
* The Action button (B) speeds up swimming, the Jump button (A) works as up+B
* Wario cannot hurt enemies when swimming
* When Wario is right under the surface of water, he floats remaining vertical with a different animation.
* Wario can jump only 1-2 tiles up when he's in water.
Shylence 14:31, 23 Oct 2006 (CEST)


How's this in water Tux swims along without stopping, and slowly sinks, direction arrows change Tux's direction or speed him up if you press the direction he is already moving. if you press down he dives, when diving Tux hurts all enemies but can only move downwards fast. Up arrow stops Tux sinking and he starts rising.
When Tux is on solid ground, pressing jump will make him kick the ground, and thus go upwards very fast. when at the surface of the water, Tux can jump out almost as high as when on land, but not quite.

The rotation angle could be uncomfortable.
I think that instead of making an actual permanent rotation, just make use of the 8 directional gamepad. I mean.. make Tux sprite *look* like 45º rotated when you press both up and right arrows and perform a up and right movement simultaneously. The last movement direction will be kept after releasing the buttons, but you could press the right arrow after that and make the Tux sprite return to the horizontal angle (although it could have a bit of vertical velocity due to the prior acceleration). There could be no need for a new collision detection code after all, you don't need to rotate rectangles, just reorganize them to fit each Tux shape (horizontal Tux, vertical Tux and +/-45º rotated Tux, no more angles needed). --[[User:Ferk|Ferk]] 13:41, 2 February 2007 (UTC)
: It's not about rotating images, but about the correct collision detection for rotated rectangles.
::That's what I did mean. wouldn't it be possible to make the Tux character be 3 rectangles placed in some diagonal way instead of rotating them? I think that being allowed to use more than one rectangle for the same entity would be more useful than being allowed to rotate them. As you could draw any shape with multiple rectangles. If it is just the 45º rotated Tux collisions what needed to be resolved, it could be made that way and you would not need to care about actual rotation.

[[Category:Action]]