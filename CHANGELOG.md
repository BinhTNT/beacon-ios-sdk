# Installation & Update

To install Beacon, see the [documentation](https://developer.helpscout.com/beacon-2/).

## 2.0.0 Beta 2 Release (May 26, 2020)

##### Bug Fixes

* Many bugs with the new Chat feature have been fixed.

## 2.0.0 Beta 1 Release (April 16, 2020)

##### Enhancements

* Live chat - Now customers can start a chat from your app on their iOS device, accessing great support no matter where they are.

## 1.0.5 Release (March 13, 2020)

##### Bug Fixes

* Fixed the root cause of [issue 40](https://github.com/helpscout/beacon-ios-sdk/issues/40) where the Reply modal was not presented when attempting to respond via your Conversation history
* Push notifications will now successfully register for any messages delivered across all iOS versions

## 1.0.4 Release (March 5, 2020)

##### Bug Fixes

* Attachments can now be added to replies from the previous messages screen on iPad ([Issue 52](https://github.com/helpscout/beacon-ios-sdk/issues/52))
* Update our use of UIWebView to WKWebView ([Issue 37](https://github.com/helpscout/beacon-ios-sdk/issues/37))
* Improved error messaging in cases where we failed to load the Beacon configuration ([Issue 38](https://github.com/helpscout/beacon-ios-sdk/issues/38))
* Chat replies are now presented ([Issue 40](https://github.com/helpscout/beacon-ios-sdk/issues/40))

## 1.0.3 Release (January 8, 2020)

##### Bug Fixes

* Prevent the prefill method from being called multiple times ([Issue 42](https://github.com/helpscout/beacon-ios-sdk/issues/42))
* Dismissing Beacon now prompts the user correctly on iOS 13 ([Issue 43](https://github.com/helpscout/beacon-ios-sdk/issues/43))
* Fixed image picker warnings on the main thread ([Issue 46](https://github.com/helpscout/beacon-ios-sdk/issues/46))
* Text prefill does not prevent message submission ([Issue 47](https://github.com/helpscout/beacon-ios-sdk/issues/47))

## 1.0.2 Release (November 14, 2019)

##### Bug Fixes

* Fixes a crash reported in HSBeaconPreviousMessagesController. ([Issue 33](https://github.com/helpscout/beacon-ios-sdk/issues/33))
* Improves prefill behavior when opening a contact form subsequent times. ([Issue 34](https://github.com/helpscout/beacon-ios-sdk/issues/34))
* Fixes a crash when calling reset on a form with attachments. ([Issue 35](https://github.com/helpscout/beacon-ios-sdk/issues/35))
* Fixes not being able to select an image from the Photo Library on iOS 13. ([Issue 39](https://github.com/helpscout/beacon-ios-sdk/issues/39) & [Issue 41](https://github.com/helpscout/beacon-ios-sdk/issues/41))
* Fixes an issue that prevented some apps from supporting dark mode. ([Issue 32](https://github.com/helpscout/beacon-ios-sdk/issues/32))

## 1.0.1 Release (May 23, 2019)

##### Enhancements

* Added a `tintColorOverride` setting to allow for customization of the color of buttons and labels throughout the SDK

##### Bug Fixes

* Fixes for the Get In Touch & Messaging Enabled settings
* Fixes for CSS issues with nested `ol` tags

## 1.0.0 Release (March 15, 2019)

* New `reset` method on `HSBeacon` to clear the current state
* New `suggestWithItems` method that also allows for URL-based custom suggestions
* New `HSBeaconDelegate` methods for intercepting Beacon open and close events
* Improved VoiceOver support - translations for button accessibility labels and the navigation tabs now respond correctly in VoiceOver mode
* The `HSBeaconSettings` object is now available on the `HSBeaconContactForm` object when calling `prefill`.
* Fixes for layout bugs on iPad where UI elements would render offscreen.
* The `color` attribute of `HSBeaconSettings` is now a strong reference.
* The name and email fields are now always shown on the contact form unless the `login` method is called. This allows users who have manually entered these values to correct mistakes when sending a new email.

## 1.0.0 beta (build 73) (January 16, 2019)

* We've fixed the message history for secure mode users that broke in build 0.69. Sorry for the trouble!

## 1.0.0 beta (build 72) (December 19, 2018)

##### Enhancements

* Added a new method `suggest` for custom suggestions
* Added `dismissBeacon` method to make sure Beacon isn't in the way of other code in your app
* Carthage support is back!
* A continued restructuring of [our developer documentation](https://developer.helpscout.com/beacon-2/ios/)

## 1.0.0 beta (build 71) (December 7, 2018)

##### Bug Fixes

* The main Beacon controller now implements `preferredStatusBarStyle` to try to resolve [issue #19](https://github.com/helpscout/beacon-ios-sdk/issues/19)
* Article viewed activities will now link to the article in you Help Scout Beacon note, rather than the application in the App Store. Search activities will no longer show a link. This also resolves a crash with a missing `CFBundleName`. Long term, we'll add the Beacon name & platform to the note so you can more easily identify the source.

## 1.0.0 beta (build 69) (December 6, 2018)

##### Bug Fixes

* Fixed user attribute upload for unsecure users
* Fixed a crash condition with the `navigate` method

## 1.0.0 beta (build 67) (November 27, 2018)

##### Enhancements

* New methods on `HSBeacon` - `search`, `openArticle`, and `navigate`.
* Our developer site now includes [Jazzy](https://github.com/realm/jazzy) generated API documentation.

##### Bug Fixes

* More translation fixes documented [here](https://github.com/helpscout/beacon-ios-sdk/issues/8#issuecomment-434243479) and [here](https://github.com/helpscout/beacon-ios-sdk/pull/11/files).


## 1.0.0 beta (build 58) (October 24, 2018)

##### Bug Fixes

* The text for "We usually respond in..." was not getting translated with the `useLocalTranslationOverrides` option enabled ([reported issue](https://github.com/helpscout/beacon-ios-sdk/issues/8))


## 1.0.0 beta (build 57) (October 23, 2018)

##### Enhancements

* New local overrides added to `HSBeaconSettings`
  * Color
  * Docs enabled
  * Custom fields enabled
  * Show name
  * Show subject
  * Allow attachments
  * Show get in touch
  * Show prefilled custom fields
* User attribute limit increased to 30
* Attachment preview now uses QuickLook instead of `UIDocumentInteractionController` to address App Store rejections

##### Bug Fixes

* Status bar color is restored when exiting Beacon

## 1.0.0 beta (build 52) (September 21, 2018)

##### Bug Fixes

* Fixed a crash on previous messages with an empty subject reported [here](https://github.com/helpscout/beacon-ios-sdk/issues/6)

## 1.0.0 beta (build 49) (September 19, 2018)

##### Enhancements

* Added a flag for disabling the contact form
* Added a blank state in cases where Docs and Messaging are both disabled
* UI enhancements related to overlapping & loading content

##### Bug Fixes

* Dynamic Type will no longer need an app restart to take effect
* Fixed scrolling issues for articles with large tables

## 1.0.0 beta (build 44) (August 7, 2018)

##### Enhancements

* Beacon is now distributed as a static framework
* Added up & down arrows to navigate between form fields
* Custom fields and agent avatars are now cached between loads
* Dynamic Type is supported in multiple areas
* Form field length limits are now more tightly enforced
* The contact form can now be prefilled to provide attachments and field values automatically

##### Bug Fixes

* Fix a case where related article links would not always work from search
* Ensure that the search results back button will adhere to the Beacon color

## 1.0.0 beta (build 41) (July 17, 2018)

##### Enhancements

* Added state restoring when opening the same Beacon after it has been closed
* Improvements to network error handling
* Updated the visual appearance of custom fields
* Updated the contact button when viewing empty search results

##### Bug Fixes

* Fixed crashes around attachment uploading
* Fixed articles failing to load correctly

## 1.0.0 beta (build 37) (June 18, 2018)

##### Enhancements

* Improve error handling in the Previous Messages flow
* Prevent sending duplicate messages when replying to a thread or starting a new one

##### Bug Fixes

* Attachments with zero length are now rejected

## 1.0.0 beta (build 36) (June 13, 2018)

##### Enhancements

* Use `WKWebView` for rendering articles

##### Bug Fixes

* Fix an issue with article cards where the status bar would overlap the article
* Fix an issue where the article content may never appear after loading

## 1.0.0 beta (build 35) (June 12, 2018)

##### Enhancements

* Initial framework release

##### Bug Fixes

* Initial framework release
