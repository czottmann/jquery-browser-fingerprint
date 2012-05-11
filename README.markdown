### jquery.browser-fingerprint.js

Browser fingerprinting is a technique to "mark" anonymous users using JS
(or other things).  To build an "identity" of sorts the browser is queried
for a list of its plugins, the screen size and several other things, then
hashes them.  The idea is that these bits of information produce an unique
"fingerprint" of sorts; the more elaborate the list of data points is, the
more unique this fingerprint becomes.  And you wouldn't even need to set a
cookie to recognize this user when she visits again.

For more information on this topic consult
[Ars Technica](http://arstechnica.com/tech-policy/news/2010/05/how-your-web-browser-rats-you-out-online.ars)
or the [EFF](http://panopticlick.eff.org/).  There is a lot of potential
for undesirable shenanigans, and I strictly oppose using this technique for
marketing and ad-related tracking purposes.

Anyways, I needed a really simple fingerprinting library, so I wrote a
quick and dirty jQuery plugin.  This is by no means a complete and
watertight implementation -- it is merely the scratch for a particular itch
I was having.  YMMV.

This library was written by Carlo Zottmann, carlo@municode.de, has its home
@ [Github](http://github.com/carlo/jquery-browser-fingerprint) and is
WTF-licensed (see LICENSE.txt).

Documentation (docco-generated) can be found in the `docs/` folder.
