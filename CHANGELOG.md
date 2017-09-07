## 1.3.0 (2017-09-07)

#### Added
- Allow users to deactivate the delete warning ([#25](https://github.com/MBuchalik/mb_app/issues/25))
- Swipe-to-delete :smiley: ([#23](https://github.com/MBuchalik/mb_app/issues/23))
- Send read receipt when reading an email ([#20](https://github.com/MBuchalik/mb_app/issues/20))
- Refactored settings page

##### Info
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
