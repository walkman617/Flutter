
# Chapter 11: Practice 

## 1. How experienced of a programmer/developer do I have to be to use Flutter?
Answer: 
- Flutter is approachable to programmers familiar with object-oriented concepts (classes, methods, variables, etc) and imperative programming concepts (loops, conditionals, etc).

- No prior experience is required in order to learn and use Flutter.

- We have seen people with very little programming experience learn and use Flutter for prototyping and app development.

## 2. What kinds of apps can I build with Flutter?
Answer: 
- Flutter is optimized for 2D mobile apps that want to run on both Android and iOS. Flutter is also great for interactive apps that you want to run on your web pages or on the desktop. (Note that web support is in beta, and desktop support is in alpha.)

- Apps that need to deliver brand-first designs are particularly well suited for Flutter. However, apps that need to look like stock platform apps can also be built with Flutter.

- You can build full-featured apps with Flutter, including camera, geolocation, network, storage, 3rd-party SDKs, and more.

## 3. What is inside the Flutter SDK?
- Heavily optimized, mobile-first 2D rendering engine with excellent support for text
- Modern react-style framework
- Rich set of widgets implementing Material Design and iOS-style.
- APIs for unit and integration tests
- Interop and plugin APIs to connect to the system and 3rd-party SDKs
- Headless test runner for running tests on Windows, Linux, and Mac
- Dart DevTools for testing, debugging, and profiling your app
- Command-line tools for creating, building, testing, and compiling your apps

## 4. Does Flutter work with any editors or IDEs?
Answer: We support plugins for Android Studio, IntelliJ IDEA, and VS Code.

## 5. Where can I deploy my Flutter app?
Answer: You can compile and deploy your Flutter app to iOS, Android, web (in beta), and desktop (macOS is in alpha, Linux and Windows are in development). While some folks are already deploying Flutter web apps, you might want to wait for web and desktop support to migrate to the stable channel.

## 6. What operating systems can I use to build a Flutter app?
Answer: Flutter supports development on Linux, Mac, and, Windows.

## 7. What language is Flutter written in?
Answer: We looked at a lot of languages and runtimes, and ultimately adopted Dart for the framework and widgets. The underlying graphics framework and the Dart virtual machine are implemented in C/C++.

## 8. How is hot reload different from hot restart?
Answer: Hot reload works by injecting updated source code files into the running Dart VM (Virtual Machine). This doesn’t only add new classes, but also adds methods and fields to existing classes, and changes existing functions. Hot restart resets the state to the app’s initial state.