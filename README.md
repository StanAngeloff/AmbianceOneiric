AmbianceOneiric
===============

This is the stock Ubuntu Precise 12.04 Ambiance theme with light menus reverted.

Why?
----

The design team at Canonical has decided to refresh the default theme in Ubuntu
for its LTS release to feature light menus from light sources and dark menus
from dark sources.

While the idea sounds good at first, there are several immediate issues with it:

* It doesn't play well with other apps. E.g., Firefox and Thunderbird can be
  'themed' resulting in, possibly, the wrong menu being 'given off'.
* Even within Ubuntu the convention is violated - menus from window titlebars
  and toolbars, such as those in Nautilus, are light (these UI elements are dark
  by default).
* The context menu on the desktop doesn't take into account the brightness of the
  wallpaper. While we are now used to chameleonic behaviour for the Dash and
  notifications, this behaviour doesn't carry across for menus.

There is a [long discussion on Launchpad][discussion] with many affected Users
which you should read if you want the full story.

  [discussion]: https://bugs.launchpad.net/ubuntu/+source/light-themes/+bug/925895

How?
----

There is one known workaround which advises that `light-themes` `0.1.8.29` is
installed in Precise. While this will work for most, it throws away all other
improvements in the theme since its Oneiric release. One of the most notable
changes is making elements in non-active windows less prominent.

This version compares the stock theme (found in `/usr/share/themes/Ambiance`)
against `r167` from [`lp:light-themes`][lightthemes] instead. Only changes
related to light menus have been reverted, both for Gtk2 and Gtk3 apps.

  [lightthemes]: http://bazaar.launchpad.net/~ubuntu-art-pkg/light-themes/trunk/files/167

Installation
------------

[Download this repository][download] and extract it in `~/.themes/`. Use
`gnome-tweak-tools` or `ubuntu-tweak` to change the theme to 'AmbianceOneiric'.
Note it will not show up in the list of available themes in the 'Appearance'
settings panel.

  [download]: https://github.com/StanAngeloff/AmbianceOneiric/zipball/master

Issues
------

Any theme glitches should be reported against the master [Light Themes][master]
project. Those related to wrong menu colouring should be reported in here.

  [master]: https://code.launchpad.net/~ubuntu-art-pkg/light-themes/trunk
