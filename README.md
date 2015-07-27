**Wpak Off-Canvas are demo themes for iOS and Android mobile apps implementing an off-canvas menu.** They are designed to work with WP-AppKit, a WordPress plugin to create mobile apps connected to WordPress (more on that at http://getwpappkit.com).

![wp-appkit-off-canvas-screenshots-1 5](https://cloud.githubusercontent.com/assets/6179747/8889585/5846e28e-32e0-11e5-9afa-0b9440fd6a62.png)

You might want to check these other fine themes: [Wpak Tabs](https://github.com/uncatcrea/wpak-tabs-themes)

# Installation
* Download WP-AppKit: https://github.com/uncatcrea/wp-appkit
* Install WP-AppKit as you would do for any other WordPress plugins (ie. drop the plugin folder in */wp-content/plugins*)
* Activate WP-AppKit using the _Plugins_ WordPress admin panel. (Browse the *Installed Plugins* list and click the *Activate* link of WP-AppKit.)
* Now you should have a brand new */wp-content/themes-wp-appkit* folder (yes, this is where app themes are stored)
* Download the themes from this repository and drop their folders in */wp-content/themes-wp-appkit*
* In WordPress, use the *WP-AppKit* admin panel to create a new app and choose one of the themes in the *Appearance* box
* From there you're free to test in your browser (using the Chrome's Emulation Mode) or directly try to compile

If new to WP-AppKit, you might want to read this article: http://uncategorized-creations.com/1212/compiling-app-using-wp-appkit-phonegap-build/.

# Theme's Overview

Take a look at these videos to get a glimpse of the themes:
* [Android Demo Video](https://www.youtube.com/watch?v=BHYoV1h89Ow)
* [iOS Demo Video](https://www.youtube.com/watch?v=xSryx6hUyaU)

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
WP-AppKit themes rely on Cordova plugins to:
* Customize the iOS status bar: https://build.phonegap.com/plugins/505
* Handle properly whether hyperlinks open an in app browser (iOS) or not (Android): https://build.phonegap.com/plugins/1169

WP-AppKit export function adds these plugins automatically to your *config.xml* file. If you don't use the export, make sure to add them in order the themes to be able to work properly.

## Responsive Images
Themes hook into the WP-AppKit web services to modify the source code of images in the post content. It eases the way to style the responsive images later. See *modify-image-code.php* in the *php* folder of the themes.