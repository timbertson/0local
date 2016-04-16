<img src="http://gfxmonk.net/dist/status/project/0local.png">

Create a local version of a given feed.

This is useful to:
 - Test modifications to a feed locally, without having to
   publish them.
 - Override the implementation for a public feed with your
   own sources.

Usage:

	0local feed.xml

Creates feed-local.xml in the current directory (overwriting
it if present). This local feed will have only one (local)
implementation, with path &quot;.&quot;

You can also pass in a URL instead of a filename, to make a
local version of the feed at that URL.

To register (or unregister) your local feed as the preferred
implementation for the feed URI, run:

	0launch -f feed-local.xml

And follow the prompts.
