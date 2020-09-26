## 2.0.0 (2020-09-26)

#### Added
- It is now possible to edit the address book (users can add new contacts and edit existing ones).
- Thanks to Ionic, the UI design now adapts to look more like native iOS or Android.
- Email folders now update automatically when a new email arrives.
- Much better error handling (e.g. by showing a "try again" button in various places when the connection to the server fails).
- When writing an email, you can now open the address book to select recipients.

#### Changed
- The email folder list is now properly indented (previously, all folders were just shown in a plain list).
- The email multi selection menu has been completely revamped.
- The file downloads page has been completely revamped.

#### Info

This is a complete rewrite of the app with much more modern tools/libraries! The app is now built using Angular, Ionic and a local Cordova installation. So, in the end, we build the app using Android Studio (or Xcode) and are not depending on any 3rd party cloud service anymore.

The server plugin has also been changed in many places to be more type safe.

## 1.6.1 (2019-09-24)

#### Fixed

- Due to a bug, it was not possible to close the app on Android when clicking on the confirm button of the "close app" dialog.

#### Changed

- The app now fulfills the new App Store requirements.

## 1.6.0 (2019-09-02)

#### Added

- It is now possible to set "cc" and "bcc" recipients when writing an email. ([#22](https://github.com/MBuchalik/mb_app/issues/22))
- When forwarding an email, the attachments are now also included. ([#38](https://github.com/MBuchalik/mb_app/issues/38))

#### Changed

- The app is now compatible with the 64 bit PlayStore requirement.

#### Info

On Android, the minimum OS version is now 5.0 (Lollipop, SDK version 21).

The size of the .apk file decreases from ~28 MB to ~5MB. The size of the installed Android app decreases from ~80 MB to ~12 MB.

## 1.5.0 (2018-09-20)

#### Changed
- b1gmail 7.4 is now fully supported :smiley: Please note this plugin is **not compatible with b1gmail 7.3** anymore.
- On iOS, we are now using the http2 push gateway. Please check whether your server supports this method. This new method also allows overriding of old push notifications.
- On Android, we are now using FCM instead of GCM.
- On Android, other aspect ratios are now supported. ([#34](https://github.com/MBuchalik/mb_app/issues/34))

#### Fixed
- Crashes on iOS when saving an image to the camera roll. ([#33](https://github.com/MBuchalik/mb_app/issues/33))

#### Info
Please remember only to install this update when using b1gmail 7.4.

## 1.4.0 (2018-05-26)

#### Added
- mb_app now supports iPhone X and iOS 11.
- Request a read receipt when writing an email. ([#21](https://github.com/MBuchalik/mb_app/issues/21))
- Show a warning when leaving the email compose view. ([#30](https://github.com/MBuchalik/mb_app/issues/30))
- Email compose: Make the list of recipients more user-friendly. ([#31](https://github.com/MBuchalik/mb_app/issues/31))
- Allow users to add their signature. ([#32](https://github.com/MBuchalik/mb_app/issues/32))

#### Fixed
- Push notifications: No sound played on Android ([#26](https://github.com/MBuchalik/mb_app/issues/26))

#### Info
AdMob for iOS currently isn't working. It has been disabled in this version.

Please note that the project structure has been changed. Also, two info files were added to the download archive. You should carefully read them before creating new versions of your app!

## 1.3.0 (2017-09-07)

#### Added
- Allow users to deactivate the delete warning ([#25](https://github.com/MBuchalik/mb_app/issues/25))
- Swipe-to-delete :smiley: ([#23](https://github.com/MBuchalik/mb_app/issues/23))
- Send read receipt when reading an email ([#20](https://github.com/MBuchalik/mb_app/issues/20))
- Refactored settings page

#### Info
- This version includes a new "license" page. From now on, make sure you are always using the latest license page shipped with the version you are using.
- JavaScript is now written in strict mode.
- A new icon set is used (it should behave like the old one but include more icons).

## 1.2.0 (2017-04-25)

#### Added
- Restore emails when deleting them using a "single action" (the mass action isn't supported at the moment) ([#19](https://github.com/MBuchalik/mb_app/issues/19))
- Pinch-to-zoom html mails ([#18](https://github.com/MBuchalik/mb_app/issues/18))
- Allow users to empty the trash ([#17](https://github.com/MBuchalik/mb_app/issues/17))

#### Fixed
- A hidden unread badge in an email folder used to show an outline shadow on lighter main colors ([#16](https://github.com/MBuchalik/mb_app/issues/16))
- On some Android 7 devices, the app crashed right after starting it due to a problem with the splash screen image.
- On some Android devices, there were problems with the network connectivity after running the app in the background for some time.

#### Info
Apps for Android can't be built using version 1.1.0 (or lower) anymore. They simply won't start since older versions of the push plugin don't seem to be compatible with the latest Android SDK. Apps that were built before (and worked) aren't affected.

## 1.1.0 (2017-01-15)

#### Added
- Support for iOS :smiley: ([#14](https://github.com/MBuchalik/mb_app/issues/14))
- Image preview when writing an email ([#12](https://github.com/MBuchalik/mb_app/issues/12))
- Unread badge on the "refresh" and "folder" icon ([#11](https://github.com/MBuchalik/mb_app/issues/11))
- Forwarding of mail text ([#10](https://github.com/MBuchalik/mb_app/issues/10))
- Unread badge on many Android phones (as well as on iOS) ([#8](https://github.com/MBuchalik/mb_app/issues/8))
- Share files to Android ([#7](https://github.com/MBuchalik/mb_app/issues/7))
- Note about energy saving on Huawei phones ([#6](https://github.com/MBuchalik/mb_app/issues/6))
- (Better) error handling when starting the application ([#2](https://github.com/MBuchalik/mb_app/issues/2))
- Debugging tool for push notifications in the ACP

#### Changed
- Display the recipient's name in the outbox ([#5](https://github.com/MBuchalik/mb_app/issues/5))
- Sort the addressbook content correctly ([#4](https://github.com/MBuchalik/mb_app/issues/4))
- The whole layer system has been rewritten to support iOS
- The app waits for all modules to be loaded until it displays the login page (or logs the user in automatically)

#### Info
A lot of improvements and changes were made to support Android and iOS on the same code base. Furthermore, a cool new tool was introduced to simplify app creation. Also, a list of changed files is now included in the download archive.

There were so many small improvements that it is hard to list all of them here. This release really is a great improvement to the application.

## 1.0.1 (2016-09-06)

#### Changed
- Use another ads plugin without traffic sharing ([#9](https://github.com/MBuchalik/mb_app/issues/9))

#### Info
You should only update if your are using ads. No other changes were made.


## 1.0.0 (2016-05-22)

#### Changed
- Use English as fallback language ([#1](https://github.com/MBuchalik/mb_app/issues/1))

#### Info
This is the very first stable release :-)
