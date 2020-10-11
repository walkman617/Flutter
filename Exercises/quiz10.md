
# Chapter 10: Deployment 
## 1. What's the Obfuscating Dart code?
Answer: Code obfuscation is the process of modifying an app’s binary to make it harder for humans to understand. Obfuscation hides function and class names in your compiled Dart code, making it difficult for an attacker to reverse engineer your proprietary app.

## 2. How to obfuscate your app?
Answer: To obfuscate your app, build a release version using the --obfuscate flag, combined with the --split-debug-info flag. The --split-debug-info flag specifies the directory where Flutter can output debug files. This command generates a symbol map. The apk, appbundle, ios, and ios-framework targets are currently supported. (macos and aar are supported on the master and dev channels.)

## 3. How to read an obfuscated stack trace?
Answer: To debug a stack trace created by an obfuscated app, use the following steps to make it human readable:

- Find the matching symbols file. For example, a crash from an Android arm64 device would need app.android-arm64.symbols.

- Provide both the stack trace (stored in a file) and the symbols file to the flutter symbolize command. For example:

## 4. Before publishing, What finishing touches might you should put on your Android app?
Answer: Before publishing, you might want to put some finishing touches on your app. 
- Adding a launcher icon
- Signing the app
- Shrinking your code with R8
- Reviewing the app manifest
- Reviewing the build configuration
- Building the app for release
- Publishing to the Mobile APP Store
- Updating the app’s version number

## 5. How to create an application record on App Store Connect for an iOS app?
Answer: Register your app on App Store Connect:

- Open App Store Connect in your browser.
- On the App Store Connect landing page, click My Apps.
- Click + in the top-left corner of the My Apps page, then select New App.
- Fill in your app details in the form that appears. In the Platforms section, ensure that iOS is checked. Since Flutter does not currently support tvOS, leave that checkbox unchecked. Click Create.
- Navigate to the application details for your app and select App Information from the sidebar.
- In the General Information section, select the Bundle ID you registered in the preceding step.

## 6. How to build the web app for release?
Answer: Build the app for deployment using the flutter build web command. This generates the app, including the assets, and places the files into the /build/web directory of the project.

The release build of a simple app has the following structure:
```
/build/web
  assets
    AssetManifest.json
    FontManifest.json
    NOTICES
    fonts
      MaterialIcons-Regular.ttf
      <other font files>
    <image files>
  index.html
  main.dart.js
  main.dart.js.map
```

## 7. How to embed a Flutter app into an HTML page?
Answer: You can embed a Flutter web app, as you would embed other content, in an iframe tag of an HTML file. In the following example, replace “URL” with the location of your HTML page:
```html
<iframe src="URL"></iframe>
```