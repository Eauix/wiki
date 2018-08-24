A '''Path''' is a series of points that can be followed by some objects. This way controlled movement can be implemented, like opening doors, moving platforms, traps, etc.

== Synopsis == 

 (path
   (mode "circular")
   (node
     (x 800)
     (y 96)
     (time 0.3)
   )
   (node
     (x 832)
     (y 96)
     (time 1.0)
   )
 )

== Syntax ==

A path consists of a ''mode'' setting and one or more ''nodes''.

=== Mode ===

The ''mode'' specifies the behavior at the end of the path when automatic movement is activated, i.e. the object is going to all nodes in order one by one (rather than being told to go to a specific node and stay there). It takes one string argument with the following possible values:

* '''circular'''<br />After reaching the last node go directly back to the first node, forming a circle.
* '''pingpong'''<br />After reaching the last node go back the path, visiting all nodes in reverse order. This is especially useful for moving platforms that go back and forth a specific path.
* '''oneshot'''<br />When reaching the last node, stay there.<br />''(FIXME: I have no idea if this is correct)''
* '''unordered'''<br />Travels to a random node and never stops. Goes directly to given node when not running.

'''Example:'''
 (mode "circular")

=== Nodes ===

Nodes are points in the level along which the associated object moves. They have the following attributes:

* '''x'''<br />x-coordinate of the point in ''pixels''.
* '''y'''<br />y-coordinate of the point in ''pixels''.
* '''time''' ''(optional)''<br />Time it takes to move to the ''next'' point in seconds. Defaults to one second.

'''Example:'''
 (node
   (x 42)
   (y 23)
   (time 1.337)
 )

== Scripting ==

Objects a path is associated with usually provide the following methods:

{| class="objectlist"
! class="method"| goto_node(int node_no)
| advance until at given node, then stop. Nodes are numbered from 0 to ''n''&nbsp;−&nbsp;1.
|-
! class="method"| start_moving()
| start advancing automatically
|-
! class="method"| stop_moving()
| stop advancing automatically
|}

== Used by ==

* [[ScriptingCamera|Camera]] (''autoscroll'' mode)
* [[ScriptingPlatform|Platform]]
* [[ScriptingTilemap|Tilemap]]
* [[ScriptingWill-o-wisp|Will-o-wisp]]

[[Template:Navbox Scripting reference]]
[[Category:Scripting Reference]]