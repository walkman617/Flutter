
# Chapter 08: Tools & techniques
## 1. How to update the plugins in Android Studio & IntelliJ?
Answer: 
- Open preferences (Android Studio > Check for Updates on macOS, Help > Check for Updates on Linux).
- If dart or flutter are listed, update them.

## 2. How to create a new project in Android Studio & IntelliJ?
Answer: To create a new Flutter project from the Flutter starter app template:
- In the IDE, click Create New Project from the Welcome window or File > New > Project from the main IDE window.
- Select Flutter in the menu, and click Next.
- Enter your desired Project name and Project location.
- If you might publish this app, set the company domain.
- Click Finish.

## 3. How to update the extension in Visual Studio Code?
Answer: To install updates manually:
- Click the Extensions button in the Side Bar.
- If the Flutter extension is shown with an available update, click the update button and then the reload button.
- Restart VS Code.

## 4. How to create a new project in Visual Studio Code?
Answer: To create a new Flutter project from the Flutter starter app template:

- Open the Command Palette (Ctrl+Shift+P (Cmd+Shift+P on macOS)).
- Select the Flutter: New Project command and press Enter.
- Enter your desired Project name.
- Select a Project location.

## 5. How to Run and debug in Android Studio & IntelliJ?
Answer: You can debug your app in a few ways.
- Using DevTools, a suite of debugging and profiling tools that run in a browser and include the Flutter inspector. DevTools replaces the previous browser-based profiling tool, Observatory.
- Using Android Studio’s (or IntelliJ’s) built-in debugging features, such as the ability to set breakpoints.
- Using the Flutter inspector, directly available in Android Studio and IntelliJ.

## 7. How to Run and debug in Visual Studio Code?
Answer: You can debug your app in a couple of ways.

- Using DevTools, a suite of debugging and profiling tools that run in a browser. DevTools replaces the previous browser-based profiling tool, Observatory, and includes functionality previously only available to Android Studio and IntelliJ, such as the Flutter inspector.
- Using VS Code’s built-in debugging features, such as setting breakpoints.

## 8. How to run app with breakpoints in Android Studio & IntelliJ?
Answer: 
### If desired, set breakpoints in your source code.
### Click the Debug icon in the toolbar, or invoke Run > Debug.
- The bottom Debugger pane shows Stack Frames and Variables.
- The bottom Console pane shows detailed logs output.
- Debugging is based on a default launch configuration. To customize this, click the drop-down button to the right of the device selector, and select Edit configuration.

## 9. How to run app with breakpoints in Visual Studio Code?
Answer: 
### If desired, set breakpoints in your source code.
### Click Run > Start Debugging in the main IDE window, or press F5.
- The left Debug Sidebar shows stack frames and variables.
- The bottom Debug Console pane shows detailed logging output.
- Debugging is based on a default launch configuration. To customize, click the cog at the top of the Debug Sidebar to create a launch.json file. You can then modify the values.

## 10. What is DevTools?
Answer: DevTools is a suite of performance and debugging tools for Dart and Flutter. It’s currently in beta release, but is under active development.
![dart-devtools](images/devtools.gif)

## 11. What can I do with DevTools?
Answer: Here are some of the things you can do with DevTools:

- Inspect the UI layout and state of a Flutter app.
- Diagnose UI jank performance issues in a Flutter app.
- CPU profiling for a Flutter or Dart app.
- Network profiling for a Flutter app.
- Source-level debugging of a Flutter or Dart app.
- Debug memory issues in a Flutter or Dart command-line app.
- View general log and diagnostics information about a running Flutter or Dart command-line app.
- Analyze code and app size.

## 12. What's the Flutter inspector?
Answer: The Flutter widget inspector is a powerful tool for visualizing and exploring Flutter widget trees. The Flutter framework uses widgets as the core building block for anything from controls (such as text, buttons, and toggles), to layout (such as centering, padding, rows, and columns).

## 13. How can the inspector helps you?
Answer: The inspector helps you visualize and explore Flutter widget trees, and can be used for the following:
- understanding existing layouts
- diagnosing layout issues

## 14. How to perform a hot reload?
Answer: To hot reload a Flutter app:

- Run the app from a supported Flutter editor or a terminal window. Either a physical or virtual device can be the target. Only Flutter apps in debug mode can be hot reloaded.
- Modify one of the Dart files in your project. Most types of code changes can be hot reloaded; for a list of changes that require a hot restart, see Special cases.
- If you’re working in an IDE/editor that supports Flutter’s IDE tools, select Save All (cmd-s/ctrl-s), or click the hot reload button on the toolbar.
