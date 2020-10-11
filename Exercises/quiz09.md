
# Chapter 09: Testing & Performance 
## 1. What tools are available for debugging Flutter applications?
Answer: Here are some of the available tools:

- DevTools, a suite of performance and profiling tools that run in a browser.
- Android Studio/IntelliJ, and VS Code (enabled with the Flutter and Dart plugins) support a built-in source-level debugger with the ability to set breakpoints, step through code, and examine values.
- Flutter inspector, a widget inspector available in DevTools, and also directly from Android Studio and IntelliJ (enabled with the Flutter plugin). The inspector allows you to examine a visual representation of the widget tree, inspect individual widgets and their property values, enable the performance overlay, and more.

## 2. What features does DevTools support?
Answer: DevTools runs in a browser and supports a variety of features:

- source-level debugger
- widget inspector that displays a visual widget tree, and “widget select” mode where you select a widget in the app and it drills down to that widget in the tree
- memory profiler
- timeline view that supports tracing, and importing and exporting trace information
- logging view

## 3. How to measure app startup time?
Answer: To gather detailed information about the time it takes for your Flutter app to start, you can run the flutter run command with the trace-startup and profile options.
```
$ flutter run --trace-startup --profile
```

## 4. What can the debug mode make?
Answer: In debug mode, the app is set up for debugging on the physical device, emulator, or simulator.

Debug mode for mobile apps mean that:
- Assertions are enabled.
- Service extensions are enabled.
- Compilation is optimized for fast development and run cycles (but not for execution speed, binary size, or deployment).
- Debugging is enabled, and tools supporting source level debugging (such as DevTools) can connect to the process.

Debug mode for a web app means that:
- The build is not minified and tree shaking has not been performed.
- The app is compiled with the dartdevc compiler for easier debugging.

## 5. What can the release mode make?
Answer: Use release mode for deploying the app, when you want maximum optimization and minimal footprint size. 

For mobile, release mode (which is not supported on the simulator or emulator), means that:
- Assertions are disabled.
- Debugging information is stripped out.
Debugging is disabled.
- Compilation is optimized for fast startup, fast execution, and small package sizes.
- Service extensions are disabled.

Release mode for a web app means that:
- The build is minified and tree shaking has been performed.
- The app is compiled with the dart2js compiler for best performance.

## 6. What can the profile mode make?
Answer: In profile mode, some debugging ability is maintained—enough to profile your app’s performance. Profile mode is disabled on the emulator and simulator, because their behavior is not representative of real performance. 

On mobile, profile mode is similar to release mode, with the following differences:
- Some service extensions, such as the one that enables the performance overlay, are enabled.
- Tracing is enabled, and tools supporting source-level debugging (such as DevTools) can connect to the process.

Profile mode for a web app means that:
- The build is not minified but tree shaking has been performed.
- The app is compiled with the dart2js compiler.

## 7. What categories does automated testing falls into?
Answer: Automated testing falls into a few categories:
- A unit test tests a single function, method, or class.
- A widget test (in other UI frameworks referred to as component test) tests a single widget.
- An integration test tests a complete app or a large part of an app.

## 8. How to reduce app size?
Answer: When building a release version of your app, consider using the --split-debug-info tag. This tag can dramatically reduce code size. Some of the other things you can do to make your app smaller are:
- Remove unused resources
- Minimize resource imported from libraries
- Compress PNG and JPEG files
