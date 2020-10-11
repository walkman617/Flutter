
# Chapter 06: Packages & plugins 
## 1. What are the advantages of the shared packages contributed by other developers?
Answer: Flutter supports using shared packages contributed by other developers to the Flutter and Dart ecosystems. This allows quickly building an app without having to develop everything from scratch.

Existing packages enable many use cases for example, making network requests (http), custom navigation/route handling (fluro), integration with device APIs (url_launcher and battery), and using third-party platform SDKs like Firebase (FlutterFire).

## 2. Where to search for shared packages?
Answer: Packages are published to pub.dev.
- The Flutter landing page on pub.dev displays top packages that are compatible with Flutter (those that declare dependencies generally compatible with Flutter), and supports searching among all published packages.
- The Flutter Favorites page on pub.dev lists the plugins and packages that have been identified as packages you should first consider using when writing your app. 

## 3. How to add a package dependency to an app?
Answer: To add the package, css_colors, to an app:
### Depend on it
- Open the pubspec.yaml file located inside the app folder, and add css_colors: under dependencies.
### Install it
- From the terminal: Run flutter pub get.<br>
OR
- From Android Studio/IntelliJ: Click Packages get in the action ribbon at the top of pubspec.yaml.
From VS Code: Click Get Packages located in right side of the action ribbon at the top of pubspec.yaml.
### Import it
- Add a corresponding import statement in the Dart code.
### Stop and restart the app, if necessary
- If the package brings platform-specific code (Kotlin/Java for Android, Swift/Objective-C for iOS), that code must be built into your app. Hot reload and hot restart only update the Dart code, so a full restart of the app might be required to avoid errors like MissingPluginException when using the package.

### 4. What package types are in Flutter?
Answer: 
- Dart packages: General packages written in Dart, for example the path package. Some of these might contain Flutter specific functionality and thus have a dependency on the Flutter framework, restricting their use to Flutter only, for example the fluro package.
- Plugin packages: A specialized Dart package that contains an API written in Dart code combined with one or more platform-specific implementations.
Plugin packages can be written for Android (using Kotlin or Java), iOS (using Swift or Objective-C), web, macOS, Windows, or Linux, or any combination thereof.
### 5. What are the package versions?
Answer: All packages have a version number, specified in the package’s pubspec.yaml file. The current version of a package is displayed next to its name.

### 6. How to update package dependencies?
Answer: When running flutter pub get (Packages get in IntelliJ or Android Studio) for the first time after adding a package, Flutter saves the concrete package version found in the pubspec.lock lockfile. This ensures that you get the same version again if you, or another developer on your team, run flutter pub get.

To upgrade to a new version of the package, for example to use new features in that package, run flutter pub upgrade (Upgrade dependencies in IntelliJ or Android Studio) to retrieve the highest available version of the package that is allowed by the version constraint specified in pubspec.yaml. 

### 7. What metrics are using in Flutter Favorite packages for high quality standards?
Answer: 
- Overall package score
- Permissive license, including (but not limited to) Apache, Artistic, BSD, CC BY, MIT, MS-PL and W3C
- GitHub version tag matches the current version from pub.dev, so you can see exactly what source is in the package
- Feature completeness—and not marked as incomplete (for example, with labels like “beta” or “under construction”)
- Verified publisher
- General usability when it comes to the overview, docs, sample/example code, and API quality
- Good runtime behavior in terms of CPU and memory usage
- High quality dependencies

