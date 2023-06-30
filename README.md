# Opera-appimage
Unofficial AppImage for Opera Web Browser

### Known issues

----------------

#### ◆ Language
As already suggested on [this page](https://forums.opera.com/topic/58114/can-t-change-ui-language-no-option-display-opera-in-that-language/12) run the AppImage fith the flag "--lang=$YOULANGUAGE" to made it work.

Instead, by installing this AppImage via "[AM](https://github.com/ivan-hc/AM-Application-Manager)" or "[AppMan](https://github.com/ivan-hc/AppMan)" the binary in $PATH is a script that launches the following command:

    opera --lang=$(echo $LANG | cut -c -2) %U
And this definitelly solves the issue.

----------------

#### ◆ Can't play videos on many sites
More banally, Ubuntu is switching all its packages to Snap, Opera developers are using an old ffmpeg in their deb package and none have updated it... so none cares about the deb version of Opera. All workaround seems to point to external third-party sources (see issue https://github.com/ivan-hc/Opera-appimage/issues/1).

However, until the deb package has no fixes, I can't update a "pure" AppImage. We need additional third-party libraries.

Those included in this AppImage are provided by https://github.com/swanux/opera_codecs

NOTE: Opera, Vivaldi, Brave, Google Chrome... are all browsers based on Chromium. Alternativelly use another web browser, like Brave or Vivaldi, they are multiplatform, privacy oriented and more supported than Opera (at least on the Linux-side). 

My version of Vivaldi is built in the same way of Opera, but everything works without issues, see [Vivaldi-appimage](https://github.com/ivan-hc/Vivaldi-appimage).


