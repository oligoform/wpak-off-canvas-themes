**Wpak Off-Canvas are demo themes for iOS and Android mobile apps implementing an off-canvas menu.** They are designed to work with WP-AppKit, a WordPress plugin to create mobile apps connected to WordPress (more on that at http://getwpappkit.com).

# Installation
* Download WP-AppKit: https://github.com/uncatcrea/wp-appkit
* Install WP-AppKit as you would do for any other WordPress plugins (ie. drop the plugin folder in */wp-content/plugins*)
* Activate WP-AppKit using the _Plugins_ WordPress admin panel. (Browse the *Installed Plugins* list and click the *Activate* link of WP-AppKit.)
* Now you should have a brand new */wp-content/themes-wp-appkit* folder (yes, this is where app themes are stored)
* Download the themes from this repository and drop their folders in */wp-content/themes-wp-appkit*
* In WordPress, use the *WP-AppKit* admin panel to create a new app and choose one of the themes in the *Appearance* box
* From there you're free to test in your browser (using the Chrome's Emulation Mode) or directly try to compile

If new to WP-AppKit, you might want to read this article: http://uncategorized-creations.com/1212/compiling-app-using-wp-appkit-phonegap-build/.

![Screenshot of the iOS version](https://cloud.githubusercontent.com/assets/6179747/8889515/93f21a90-32dd-11e5-9273-b2dc250c5026.png)

![Screenshot of the Android version](https://cloud.githubusercontent.com/assets/6179747/8889517/a4516a94-32dd-11e5-9e4d-f31df89e2b4a.png)

# Theme's Overview
##What's implemented
At the moment, Wpak Off-Canvas themes implement:
* Obviously the off-canvas menu
* Archive template (eg. post list)
* Single template (eg. a post) with the most common HTML elements (eg. strong, em, blockquote...)
* The refresh process
* Offline cache (meaning that you can read loaded posts offline)
* Post thumbnails support
* The iOS back button
* The iOS status bar 
* A responsive interface

## For iOS and Android
iOS and Android versions are fairly similar even they match their respective OS design guidelines.

Differences you may notice:
* The iOS version implements a back button when displaying the single view (ie. a post) and the Android version does not (as you will use the phone's back button)
* The iOS version implements an in app browser and the Android version will open external links in the default system browser (eg. Chrome)
* The iOS version customized the iOS status bar to match the theme

We tried to keep the source code of both themes as similar as possible. You'll see differences in *functions.js*, *custom.css* and *layout.html*.

## Cordova Plugins
...