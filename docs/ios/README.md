# DocWallet iOS — App Store preparation

Existing Expo SDK ~51 / React Native 0.74.5 project. Current iOS bundle ID in app.json: `com.docwallet.app`. Verify this is the actual app shipped on Android and that the Apple Developer account owns the bundle identifier before distribution.

This draft PR only checks the iOS JavaScript bundle. It does not create a native iOS app, sign a build, upload to TestFlight or modify production.

## Native release gates

- [ ] Confirm this repository is the correct current production DocWallet mobile codebase.
- [ ] Review Expo SDK 51 compatibility with current Xcode and App Store requirements; upgrade in a separately validated PR if needed.
- [ ] Review whether the app offers sufficient native functionality beyond an embedded website.
- [ ] Test secure session handling, document upload/download, share sheet, offline/error UI, privacy policy and account deletion.
- [ ] Validate iOS app icon, native permission descriptions, supported device screenshots and accessibility.
- [ ] Compile unsigned native iOS app, install and launch it in an iPhone simulator.
- [ ] Prepare Apple Developer team, signing, App Store Connect listing, TestFlight and human QA.

Android release paths and existing users must remain unaffected.
