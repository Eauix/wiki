__TOC__

== What? ==

The main idea of this concept is to improve supertux with multiplayer like "New Super Mario Bros. Wii" on the Wii or something alike. For now idea limits to two 
players: Tux and Penny. Both players are playing inside one world in single-screen mode.

To make game interesting to play in pair, i introduced new type of monsters (or new ability to all monsters) - carry bonus (see Bonuses) and split ability to "fire" to two different types of attack (see Players).

Oh, of course, main points of concept i wanted to achieve:

* Both players should be approximately equal in playing difficulty.
:Firstly, to make game interesting to all. If you will want to replay level with Penny after finishing level with Tux and vice-versa - then this point is done well. If there will be lots of holy wars over who is most difficult - then this point done well. If not - we have to change some details in concept or fix the balance.

* Players are designed to help each other.
:This makes game more addictive (as i think). You don't only play, you also help your friend and he helps you. If we don't follow this - what for we are creating multiplayer at all?!

== Players ==
Both players have same abilities as original tux with following differences:
{| border="1"
! Property !! Penny !! Tux
|-
|Fires with ...  || Ice (iceball) || Fire (fireball)
|-
|Bonus for increase power of bullets. || Ice bonus - you can get it from enemy. Increases enemy freezing time. Every type of enemy has it's freezing-coefficient (float-point number) describing how strong will feel this hit. For example 0 means "completely immune to cold", 1 means "sensitive to cold", 1.5 means "extra-sensitive to cold" and so on. || Fire bonus - you can get it from enemy. Enemy has floating-point life and shots has floating-point damage. Bonus will increase damage of shot.
|-
|When bullet reaches enemy, then... || Enemy freezes for some seconds. Time depends on "coldness of ice" which may be increased with appropriate bonus (ice bonus). While enemy is frozen, both tux and beastie can stuck it by jumping on it. Enemy dies. If enemy contains bonus, bonus is dropped nearby. Bonus can be picked up by Tux or Beastie.  || Enemy gets hit. If number of hits is enough to kill him, enemy dies. Number of necessary hits depends on "hotness of fire" (may be improved by fire bonus). You can't get bonus from enemy if you kill him.
|-
| What will be in single player? (or how this helps to achieve point 2) || Okay, you can get all bonuses from monsters. But there are enemies without bonuses. Killing them is expensive: freeze and be fast to stomp him. Tux will be useful in that situation. Play together with Tux. || Okay, you can kill any enemy. But you will not get fire bonuses from enemies. So killing enemies will be expensive: you need to fire a lot to kill big enemy (i.e. without fire bonus you don't have enough "fire hotness"). Play together with Penny, to get bonuses.
|}

== Bonuses ==

The first thing about bonuses - they may be placed inside enemies. Bonuses in blocks are still exist. Such an enemy may be (or should be always?) marked with some symbol, describing type of bonus, or describing random bonus.

The only way to extract bonus from enemy is to freeze enemy (Tux can do that) and then stuck it by jumping on it (both players can do).

There is a list of new bonuses (of course may be more than two, but if you add some - keep your eye on the balance.):
{| border="1"
!Bonus !! Applies to !! Meaning
|-
|Ice Bonus || Penny (multiplayer)/Both (singleplayer) || Increases freezing time for Penny's ice bullet.
|-
|Fire Bonus  ||	Tux (multiplayer)/Both (singleplayer) || Increases power for Tux's ice bullet.
|}

In single player there will be two types of flowers (from classical supertux) - ice flower and fire flower. As you can see, Tux can become "Pennyish" by gathering ice flower and then get bonuses from monsters. Or Penny can become "Tuxy" by gathering fire flower.

Notes:
"Pennyish" Tux cannot do ice-attack, so he kills enemies and improves fire from blocks.
"Tuxy" Penny cannot do fire-attack, so she freezes enemies and have to stuck them in order to kill and optionally gather bonus.

== Problems or what is to be done next ==

All enemy lives, powers of bullets, and freezing times should be balanced to make both players close (or better - equal) in play difficulty. Maybe these values should be configurable in something like Options->Difficulty Settings menu. For now I just can assume some sane values, but i haven't any ready-to-work balancing map.

Of course, we should paint sprites for Penny, bonuses, monster-has-bonus marks, different bullets...