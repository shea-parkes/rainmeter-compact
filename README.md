## Custom Rainmeter skin

This is a simple, minimal Rainmeter skin.  Customized to be just the way I like it.

Default Rainmeter skin location is `%UserProfile%\Documents\Rainmeter\Skins` (but can be altered via `Rainmeter.ini`).  Basically just clone this repository into there.

Then, editing `Rainmeter.ini` controls how this is displayed.  Here's an example to iterate from:

```ini
[rainmeter-compact\Mega]
Active=1
WindowX=1%R
WindowY=34%B
AnchorX=0%R
AnchorY=0%B
AlphaValue=200
ClickThrough=0
Draggable=0
SnapEdges=1
KeepOnScreen=1
AlwaysOnTop=2
HideOnMouseOver=1
```

### Top Proc Glitches

Showing the Top Proc currently uses the (depreciated) AdvancedCPU plugin.  As noted in its [docs](https://docs.rainmeter.net/manual/plugins/deprecated/advancedcpu/), it's possible for the Windows database of "counters" to get corrupted.  If so, you need to run these commands (as an admin) and restart Rainmeter:
```
cd c:\windows\system32
lodctr /R
cd c:\windows\sysWOW64
lodctr /R
```
