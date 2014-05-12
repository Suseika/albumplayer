What is this?
------------

The most simple way to listen to music for people who:

- Listen to whole albums instead of single compisitions or custom playlists
- Have their audio collection nicely arranged so paths to compositions contain at least album name, or even better — performer's name, year and so on.
- Prefer typing to clicking


Usage
-----

`albumplayer` searches all files in your system with a query to `locate`, finds a directory with its path contining all words from query, and starts `mplayer` with all songs from the selected album queued.

For example, 

	albumplayer in the court of crims kin

would start playing King Crimson's album "In The Court Of The Crimson King" (of course, only if you have a directory with such name in your system).
	
Queries may include anything that is related to an album an is in path to its directory: year, band name, parent directory etc.

To pause an already running player, run 

	albumplayer pause

To unpause, run the same command again


Installation
------------

- Copy `albumplayer` somewhere in your `$PATH`, rename it if you want
