x11
===

Modified version of Slackware's modular X11 SlackBuild.


PURPOSE
===
For anyone who wants to playing around with (X)WAYLAND in Slackware.
You can get SlackBuilds for wayland, mesa, libinput, libxkbcommon, pam,
and weston on: <a href="https://github.com/w41l/wlsbuild">wlsbuild repo</a>

To build xorg-server-xwayland:
1. Install wayland, mesa (with wayland support), libinput, libxkbcommon, pam,
   and weston.
2. Build/upgrade fontsproto: ./x11.SlackBuild proto fontsproto
3. Build/upgrade xorg-server: ./x11.SlackBuild xserver
4. Build/upgrade x11 drivers: ./x11.SlackBuild driver

To weston compositor with xwayland support:
  $ weston-launch -- --modules=xwayland.so


WARNING
===

This is NOT OFFICIAL X11 SlackBuild for Slackware!


ChangeLog
===
* fontsproto: Upgraded to version 2.1.3
* xserver: Upgraded to version 1.16.3
* xf86-input-synaptics: Upgraded to version 1.8.1
* xf86-video-ati: Upgraded to version 7.5.0
