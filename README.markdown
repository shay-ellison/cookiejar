Ruby CookieJar
==============

  **Git**:	[http://github.com/dwaite/cookiejar](http://github.com/dwaite/cookiejar)

  **Original Author**:	David Waite 

Synopsis
--------

The Ruby CookieJar is a library to help manage client-side cookies in pure Ruby. It enables parsing and setting of cookie headers, alternating between multiple 'jars' of cookies at one time (such as having a set of cookies for each browser or thread), and supports persistence of the cookies in a JSON string.

Both Netscape/RFC 2109 cookies and RFC 2965 cookies are supported.

Fork Purpose
------------
To enable the default `parse_set_cookie` as well as the RFC-2965 compliant `parse_set_cookie2` to expect and process the Cookie param `Max-Age`. Gems using `set_cookie` as the default call to a `Jar`, like `Faye`, get breaking behavior if `Max-Age` is received.

[rfc6265]: http://tools.ietf.org/html/rfc6265
COPYRIGHT
---------
The Ruby CookieJar is Copyright &copy; 2009-2014 David Waite, with [additional contributions from various authors][contributions]. Licensing terms are given within the [LICENSE file][LICENSE].

[contributions]: ./contributors.json
[LICENSE]: ./LICENSE
