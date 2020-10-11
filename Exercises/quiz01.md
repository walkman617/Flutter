# Chapter 01: Get Started

## 1. What is Flutter?
Answer: Flutter is Google’s portable UI toolkit for crafting beautiful, natively compiled applications for mobile, web, and desktop from a single codebase. Flutter works with existing code, is used by developers and organizations around the world, and is free and open source.

## 2. What does Flutter do?
Answer: 
- For users, Flutter makes beautiful app UIs come to life.

- For developers, Flutter lowers the bar to entry for building apps. It speeds up development of apps and reduces the cost and complexity of app production across platforms.

- For designers, Flutter helps deliver the original design vision, without loss of fidelity or compromises. It also acts as a productive prototyping tool.


## 3. What's the hot reload?
Answer: Flutter offers a fast development cycle with Stateful Hot Reload, the ability to reload the code of a live running app without restarting or losing app state. 

## 4. What devices you'll use for a Flutter app?
Answer: You can run a Flutter app by using any of the following devices:
- A physical device (Android or iOS) connected to your computer and set to developer mode
- The iOS simulator (requires installing Xcode tools)
- The Android emulator (requires setup in Android Studio)
- A browser (Chrome is required for debugging)

## 5. What's a Material app?
Answer: Material is a visual design language that is standard on mobile and the web. Flutter offers a rich set of Material widgets. 

## 6. How to pull the package into your project in the pubspec.yaml?
Answer: 
- While viewing the pubspec.yaml file in Android Studio’s editor view, click Pub get. This pulls the package into your project. 
- You should see the following in the console:
<code>flutter pub get</code>

## 7. What are the Stateless widgets and Stateful widgets?
Answer:
- Stateless widgets are immutable, meaning that their properties can’t change—all values are final. 
- Stateful widgets maintain state that might change during the lifetime of the widget. 

## 8. What kinds of build modes are in the Flutter tooling?
Answer: The Flutter tooling supports three modes when compiling your app, and a headless mode for testing. 
- Use debug mode during development, when you want to use hot reload.
- Use profile mode when you want to analyze performance.
- Use release mode when you are ready to release your app.
