<h1 align="center">Firefox hardening</h1>

<h1 align="center">Sane security conscious settings</h1>

Notes:
* DOM storage's size has been reduced, but has not been disabled for compatibility purposes;
* Smooth scrolling flags have been altered to match my preferences, as well as performance sensitive settings to increase the latter;
* webGL is turned on for my convenience.

Extensions:
* [BetterPrivacy](https://addons.mozilla.org/en-US/firefox/addon/betterprivacy/)
* [HTTPS Finder](https://github.com/kevinjacobs/HTTPS-Finder)
* [HTTPS-Everywhere](https://github.com/EFForg/https-everywhere)
* ~~Policeman~~ [uMatrix](https://github.com/gorhill/uMatrix/) (in default-deny mode)
* [uBlock by Gorhill](https://github.com/gorhill/ublock/)


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


**Note:** This is my prefs.js file. Rename it to user.js and remove some of the entries unless you want my full FF profile, which is only ok to do if you're using the same set of extensions, complete with lower latency smooth scrolling, different fonts (with better hinting, refer to [this](https://wiki.archlinux.org/index.php/Croscore_Fonts)), network related tweaks to squeeze some performance out of it, general performance based settings, amongst other things.
