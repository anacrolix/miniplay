About
=====

I wrote this originally in C sometime in 2009. It creates a system tray icon that runs music in random order from the chosen directory. Right click the system tray icon to change options. Left click to pause.

Build
=====

On Ubuntu requires libglib2.0-dev libgtk2.0-dev libgstreamer0.10-dev libnotify-dev. Run:

	autoreconf -i
	./configure
	make

Operation
=========

On recent Ubuntus (until possibly 13.04), the system tray is no longer supported, and miniplay must be whitelisted. On 12.10 I've found setting com.canonical.unity.panel.systray-whitelist to "['all']" to work. This is alleged not to work anymore on 13.04.
