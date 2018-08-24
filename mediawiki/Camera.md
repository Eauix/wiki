Level are typically a lot bigger than the actual screen, so we need to scroll the currently visible part around. This page collects some rules to do this in a nice way.

Analysis of some [[Cameras in Super Mario]]

== Basic movement ==

Basically these are the same rules as for Yoshi's Island. Maybe we will tweak it later or add special exceptions for new abilities.

=== Horizontal Movement ===
* Keep the middle point of Tux at 1/3rd of the screen width. If Tux moves/looks into the other direction, then slowly move the camera so that tux stands in the 1/3rd of the other side of the screen. This movement has to get faster if Tux moves into that direction. When Tux gets pushed into the other direction (but still looks forward) we don't change camera mode but just scroll when he gets pushed nearer than 1/3rd of the other side.
* We might experiment about changing the camera when Tux is running to 1/4th or so. We should test if this is desirable because then you see more stuff that's before you. On the other side a too dynamic camera movement can confuse and making it harder to control Tux exactly.

=== Vertical Movement ===
* Basically keep Tux in the middle of the screen.
* When Tux does a normal jump we don't scroll vertically until he stands on ground again or falls deeper than the hight where he started the jump. An exception to this rule are trampolines.

== Special modes ==

=== Autoscroll ===
The camera might scroll automatically so that Tux can't wait but has to hurry to not get squished by the moving camera somewhere. Ideally you can specify a path of vectors (together with speed) that the camera follows.

=== Right only scroll ===
This was used in the 0.1.1 release. It might be still used to not forget our history ;-)

== Configurable Camera ==

I worked a bit on the code and put all parameters that influence the
camera in a configuration file. You can now open data/camera.cfg and
play with the parameters yourself. This way you can test/try out fixed
camera, Yoshi Island and Kirby Camera and their parameters easily. You
can make the game reparse the Camera by typing
"sector.Camera.reload_config()" on the console.
Put [http://supertux.lethargik.org/viewvc/viewvc.cgi/branches/supertux/0_3_x/data/camera.cfg?view=markup camera.cfg] in ~/.supertux2/ .

[[Category:Game Object]]
[[Category:Game Engine]]