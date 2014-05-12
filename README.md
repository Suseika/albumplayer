What is this?
------------

The most convenient way to listen to music if you:

- Listen to whole albums instead of single compositions or custom playlists
- Have your audio collection nicely arranged so paths to compositions contain at least album name, or even better — performer's name, year and so on.
- Prefer typing to clicking


Usage
-----

- `albumplayer` searches all files in your system with a query to `locate`
- finds a directory with its path containing all words from a query
- and starts `mplayer` with all songs from the selected album queued.

For example, 

	albumplayer in the court of crims kin

would start playing King Crimson's album "In The Court Of The Crimson King" (of course, only if you have a directory with such name in your system).
	
Queries may include anything that is related to an album and is in path to its directory: year, band name, parent directory etc. Order of words is not important:

	albumplayer red crimson 1974 king

would still start King Crimson's 1974 album "Red". located at `/home/me/Music/King Crimson/1974 - Red`

To pause an already running player, run 

	albumplayer --pause

To unpause, run the same command again

To type a query in a GUI dialog instead of CLI arguments (so it's convenient to bind it to a system-wide key combination), run 
	
	albumplayer 

without any arguments. You need `zenity` installed for this to work.


Installation
------------

- Copy `albumplayer` somewhere in your `$PATH`, rename it if you want

Known bugs
==========

Doesn't find audiofiles in directories that are symlinks (symlinking audiofiles themselves works fine).

