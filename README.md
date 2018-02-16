# PWA-based Windows Store App
Prototype Windows Store app using PWA 

## Goal
Using PWA concepts and the newly announced Windows Store/Edge consumption of PWAs create a Store-ready app of the live Homely website.

## References
Blog post explaining the new functionality of Edge and the Windows Store.
https://blogs.windows.com/msedgedev/2018/02/06/welcoming-progressive-web-apps-edge-windows-10/

PWA Builder - Wizard-style setup and testing of manifest files and service workers. Also can output packages for submitting a PWA to various app stores.
https://www.pwabuilder.com/generator

Favicon/touch icon generator - Handy for generating the plethora different sizes
https://realfavicongenerator.net/

## Findings
If we piggyback off standard PWA concepts, namely a service worker and manifest file, we can quite easily submit a fully functioning app to the Windows Store.

It was simple to prepare the AppX (Windows Store) package using the PWA Builder and once we plugged in my Windows Developer ID and switched Windows into Developer Mode (search "developers" in Cortana) it was a simple matter of running the generated test_install.ps1

Prototype PWA installed as Windows Store app
![](https://github.com/Homely/Homely.HackDays.WindowsPWA/raw/master/WindowsPWA.JPG)

Windows Store app/PWA without service worker - offline message
![](https://github.com/Homely/Homely.HackDays.WindowsPWA/raw/master/WindowsPWAOfflineNoServiceWorker.jpg)

## Bonus Findings
The PWA Builder mentioned in references not only has the ability to output an AppX package (Windows Store) but also a Google Play Store package. This means we can submit our PWA to the Play Store in place of a native Android app.
