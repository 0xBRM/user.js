<h1 align="center">Firefox hardening</h1>

<h1 align="center">Sane security conscious settings</h1>

Notes:
* DOM storage's size has been reduced, but has not been disabled for compatibility purposes;
* Smooth scrolling flags have been altered to match my preferences, as well as performance sensitive settings to increase the latter;
* webGL is turned on for my convenience.

Extensions:
* BetterPrivacy 
* Blender (uncheck "force HTTP_ACCEPT headers")
* HTTPS Finder
* HTTPS-Everywhere 
* Policeman (in default-deny mode)
* uBlock by Gorhill


======================


![Firefox](https://i.imgur.com/HfLNk11.png)

![Chromium](https://i.imgur.com/Q9oqM6E.png)


Note how Firefox HTTP_ACCEPT headers actually convey less bits of identifying information, despite being slightly less common as a whole than its Chromium counterpart, spoofing (much like Firefox mind you, but not natively) the UA, HTTP_ACCEPT headers, and blocking access to plugins and what not.

Flash users, disable font enumeration if possible (mms.cfg).


=====================


TODO list:
* Find a more common UA/"UA/rest" combination;
* Describe what each about:config entry does.




For a user.js with more emphasis on security (occasionally at the cost of functionality, like when you completely disable DOM storage, for instance), and less emphasis on blending in, check [pyllyukko's user.js](https://github.com/pyllyukko/user.js).
