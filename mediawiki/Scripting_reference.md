__NOTOC__

Since May 2005, SuperTux sports a Squirrel scripting interface useful for level designers who want to add some interactive pep to their levels. This document poses as a reference article for those who want to explore the various objects of the SuperTux scripting model.

== What is Squirrel? ==
One of your first questions might be, "What does a rodent have to do with a penguin?" [http://www.squirrel-lang.org/ Squirrel] is a language with a syntax not much unlike other C-like languages (C, C++, Java, ...). In the current implementation, it is integrated as elements in the SuperTux level and worldmap files. The [[Console]] is a full-fledged Squirrel interpreter as well.

== Squirrel, S-expr and SuperTux ==
I have no clue if the developers simply chose Squirrel just because the name so nicely integrates into the series of words "SuperTux" and "[[S-expr]]". Currently, the Squirrel code is integrated in string arguments of Scheme elements in SuperTux level files. (Whew.) This is an example code block inside a level:
<pre>(supertux-level
  (version 2)
  (name (_ "Go Blind"))
  (author "Team")
  (sector
    (name "main")
    (music "Annoying_penguin_gawking_sounds.ogg")

    ;; tilemaps, objects, whatever. (optional)
    ;...

    (init-script "
Effect.fade_out(2.5);
")

    ;; more tilemaps, objects, and whatever. (optional)
    ;...

  )
)</pre>

When this level loads, the screen fades out completely during two and a half seconds right after the level is loaded. (Mind you, this would be a frustrating experience for the player if you add a horde of badguys near the spawn point...)

== Object reference ==
If you are interested in an object and what cans of worms you can open with it, this section is for you.

"(NYI)" after the function name symbolises functions that haven't been implemented yet. Calling them will result in a line being printed to standard output informing anybody who reads it that the script is using a function that actually doesn't exist.

=== Classes ===

{| class="objectlist"
|colspan="2" class="title"| Classes
|-
! [[ScriptingGlobals|Globals]]
| This section contains all globally defined constants and functions
|-
! [[ScriptingPlayer|Player]]
| An object that is controlled by a (human) player
|-
! [[ScriptingDisplayEffect|DisplayEffect]]
| An object that does graphical effects on the whole screen
|-
! [[ScriptingCamera|Camera]]
| Control over the camera (what the player sees)
|-
! [[ScriptingLevel|Level]]
| Control over the status the game keeps about the current level.
|-
! [[ScriptingLevelTime|Level time]]
| Scripting interface to level time object
|-
! [[ScriptingScriptedObject|ScriptedObject]]
| Object in a level than can be manipulated from scripts
|-
! [[ScriptingText|Text]]
| Display text in the top-center of the screen
|-
! [[ScriptingFloatingImage|FloatingImage]]
| Display an image floating in front of anything on-screen
|-
! [[ScriptingPlatform|Platform]]
| Scripting interface to [[Moving platform|Platform]] object
|-
! [[ScriptingTilemap|Tilemap]]
| Scripting interface to [[Tilemap]] object
|-
! [[ScriptingWind|Wind]]
| Scripting interface to [[Wind]] object
|-
! [[ScriptingCandle|Candle]]
| Scripting interface to Candle object
|-
! [[ScriptingThunderstorm|Thunderstorm]]
| Scripting interface to [[Thunderstorm]] object
|-
! [[ScriptingAmbientSound|AmbientSound]]
| Scripting interface to AmbientSound object
|-
! [[ScriptingWill-o-wisp|Will-o-wisp]]
| Scripting interface to [[Will-o-wisp]] object
|-
! [[ScriptingSector|Sector]]
| Scripting interface to the [[Sector]] itself.
|-
|}

TODO: Improve format maybe?

[[Template:Navbox Scripting reference]]
[[Category:Scripting Reference]]