# TweakPatcher
Script to patch a Cydia Substrate tweak and it's required dependencies to load on a jailed iOS device.

Tested with OS X 10.11.4, Xcode 7.3, iOS 9.2.1/9.3/9.3.1.

#####Supported tweaks:

* SnapPlus for Snapchat v1.5r-86 (tested with Snapchat v9.27.5.0)

More tweaks may be added in the future.


#####Thanks to
* [andugu](https://github.com/andugu) and [dado3212](https://github.com/dado3212) for giving me permission to use the IPA patching code from the [ScreenChat](https://github.com/andugu/ScreenChat) project.
* Giovanni Di Grezia, whose [code](http://www.xgiovio.com/blog-photos-videos-other/blog/resign-your-ios-ipa-frameworks-and-plugins-included/) served as the basis for the patchapp.sh revisions.
* [alexzielenski](https://github.com/alexzielenski) for optool.
* [BishopFox](https://github.com/BishopFox) for theos-jailed.
* [SJ_UnderWater](http://www.tonymacx86.com/general-help/86205-patcho-simple-hex-binary-patcher.html) for patcho.
* [phonegap](https://github.com/phonegap/ios-deploy) for ios-deploy.


Tutorial:
============

###Requirements

* iOS device
* Free Apple Developer account
* Xcode
* Decrypted/cracked Snapchat IPA (Google is your friend)
* (optional, precompiled version already included) [DocsDylibLoader](https://github.com/Defying/DocsDylibLoader)


###Steps

* Uninstall Snapchat from the iOS device
* There are two methods to running this script.
* 1) Run `./tweakpatcher.sh patch snapplus /path/to/Snapchat.ipa` if you don't already have a provisioning profile. It will generate one to use.
* 2) Run `./tweakpatcher.sh patch snapplus /path/to/Snapchat.ipa BUNDLE_ID` if you already have a provisioning profile and don't want to flood your Apple ID.
* Follow the on screen instructions.
* You should now have SnapPlus installed onto your jailed iOS device!
