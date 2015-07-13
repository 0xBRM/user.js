<h1 align="center">Firefox hardening</h1>

<h1 align="center">Sane security conscious settings</h1>

To use, place user.js in one of the following folders:
* GNU/Linux (hidden folder): ~/.mozilla/firefox/<profile folder> 
* Windows: C:\Users\<Username>\AppData\Roaming\Mozilla\Firefox\Profiles\<Profile>\


Notes:
* You're going to have to create the strings ````user_pref("general.appname.override", "Netscape");
user_pref("general.appversion.override", "5.0 (Windows)");
user_pref("general.buildID.override", "20150305021524");
user_pref("general.navigator.appVersion", "5.0 (Windows)");
user_pref("general.navigator.buildID", "20150305021524");
user_pref("general.navigator.geckoVersion", "31.0");
user_pref("general.navigator.platform", "Win32");
user_pref("general.navigator.system", "Windows NT 6.1; WOW64");
user_pref("general.navigator.version", "31.0");
user_pref("general.oscpu.override", "Windows NT 6.1; WOW64");
user_pref("general.platform.override", "Win32");
user_pref("general.productSub.override", "20100101");
user_pref("general.useragent.override", "Mozilla/5.0 (Windows NT 6.1; rv:31.0) Gecko/20100101 Firefox/31.0");```` manually. You can thank mozilla for that;
* DOM storage's size has been reduced, but has not been disabled for compatibility purposes;
* Smooth scrolling flags have been altered to match my preferences, as well as performance sensitive settings to increase the latter;
* webGL is turned on for my convenience;
* Apparently the scrolling settings aren't affected by user.js either, which is annoying, but I'll keep them there just because;
* Fonts used:

    Serif: Tinos, Sans-serif: Arimo, Monospace: Cousine.

Extensions:
* [BetterPrivacy](https://addons.mozilla.org/en-US/firefox/addon/betterprivacy/)
* [HTTPS Finder](https://github.com/kevinjacobs/HTTPS-Finder)
* [HTTPS-Everywhere](https://github.com/EFForg/https-everywhere)
* ~~Policeman~~ [uMatrix](https://github.com/gorhill/uMatrix/) (in default-deny mode)
* [uBlock by Gorhill](https://github.com/gorhill/ublock/)


======================


![Firefox](https://i.imgur.com/MhuXZFK.png)

![Chromium](https://i.imgur.com/ygirUof.png)


Note how Firefox HTTP_ACCEPT headers actually convey less bits of identifying information, despite being slightly less common as a whole than its Chromium counterpart, spoofing (much like Firefox mind you, but not natively) the UA, HTTP_ACCEPT headers, and blocking access to plugins and what not.

Flash users, disable font enumeration if possible (mms.cfg).


=====================


TODO list:
* Find a more common UA/"UA/rest" combination;
* Describe what each about:config entry does.




For a user.js with more emphasis on security (occasionally at the cost of functionality, like when you completely disable DOM storage, for instance), and less emphasis on blending in, check [pyllyukko's user.js](https://github.com/pyllyukko/user.js).


**Note:** This is my full FF profile (this user.js plus defaults), complete with lower latency smooth scrolling, different fonts (with better hinting, refer to [this](https://wiki.archlinux.org/index.php/Croscore_Fonts)), network related tweaks to squeeze some performance out of it, general performance based settings, amongst other things. 
