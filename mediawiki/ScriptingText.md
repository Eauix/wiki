__NOTOC__

== Summary ==
This module provides access to methods responsible for displaying text on-screen.

== Instances ==
An eponymous instance (<tt>Text</tt>) can be accessed from scripts. The console allows a <tt>sector.Text</tt>.

== Methods ==
{| class="objectlist"
! class="method"| set_text(string text)
| Sets the text string to be displayed to <tt>text</tt>.
|-
! class="method"| set_font(string font)
| Sets the font of the text to be displayed to <tt>text</tt>. Currently valid values are <tt>gold</tt>, <tt>white</tt>, <tt>blue</tt>, <tt>gray</tt>, <tt>big</tt> and <tt>small</tt>.
|-
! class="method"| fade_in(float time)
| Fades in the specified text for the next <tt>time</tt> seconds.
|-
! class="method"| fade_out(float time)
| Just the opposite of <tt>fade_in</tt>.
|-
! class="method"| set_visible(bool visible)
| Shows or hides the text abruptly (drastic counterpart to <tt>fade_in</tt> and <tt>fade_out</tt>).
|-
! class="method"| set_centered(bool centered)
| If <tt>centered</tt> is <tt>true</tt>, the text will be centered on the screen. Otherwise, it will be left-aligned.
|-
! class="method"| set_pos(float x, float y)
| Set offset of the text relative to anchor point.
|-
! class="method"| float get_pos_x()
| Returns x offset of text relative to anchor point
|-
! class="method"| float get_pos_y()
| Returns y offset of text relative to anchor point
|-
! class="method"| set_anchor_point(int anchor)
| Set anchor point of text; one of the [[ScriptingGlobals#Constants|ANCHOR_*]] constants
|-
! class="method"| int get_anchor_point()
| Returns current anchor point of text; one of the [[ScriptingGlobals#Constants|ANCHOR_*]] constants
|}

== Constants ==

None

[[Template:Navbox Scripting reference]]
[[Category:Scripting Reference]]