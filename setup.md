# Set up an editor
Follow the steps below to add an editor plugin for [Android Studio](https://flutter.dev/docs/get-started/editor?tab=androidstudio), [IntelliJ](https://flutter.dev/docs/get-started/editor?tab=androidstudio), [VS Code](https://flutter.dev/docs/get-started/editor?tab=vscode), or [Emacs](https://flutter.dev/docs/get-started/editor?tab=emacs).
##  Android Studio and IntelliJ
### 1. Install the IDE
- [Android Studio](https://developer.android.com/studio), version 3.0 or later
- [IntelliJ IDEA Community](https://www.jetbrains.com/idea/download/), version 2017.1 or later
- [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea/download/), version 2017.1 or later
### 2. Install the Flutter and Dart plugins
- Start Android Studio.
- Open plugin preferences (<strong>Configure > Plugins</strong> as of v3.6.3.0 or later).
- Select the Flutter plugin and click <strong>Install</strong>.
- Click <strong>Yes</strong> when prompted to install the Dart plugin.
- Click <strong>Restart</strong> when prompted.

### 3. Create the app
Do you want to run your Flutter app on the web? The web version of Flutter is available on the beta channel. To try it out, check out the [Write your first Flutter app for the web](https://flutter.dev/docs/get-started/web) codelab.
- Open the IDE and select <strong>Start a new Flutter project</strong>.
- Select <strong>Flutter Application</strong> as the project type. Then click <strong>Next</strong>.
- Verify the Flutter SDK path specifies the SDK’s location (select <strong>Install SDK…</strong> if the text field is blank).
- Enter a project name (for example, <strong>myapp</strong>). Then click <strong>Next</strong>.
- Click <strong>Finish</strong>.
- Wait for Android Studio to install the SDK and create the project.<br/><br/>
The above commands create a Flutter project directory called myapp that contains a simple demo app that uses [Material Components](https://material.io/design).

### 5. Run the app
- Locate the main Android Studio toolbar.
- In the <strong>target selector</strong>, select an Android device for running the app. If none are listed as available, select <strong>Tools> Android > AVD Manager</strong> and create one there. 
- Click the run icon in the toolbar, or invoke the menu item <strong>Run > Run</strong>.


## VS Code
### 1. Install VS Code
[VS Code](https://code.visualstudio.com/)  is a lightweight editor with Flutter app execution and debug support.

### 2. Install the Flutter and Dart plugins
- Start VS Code.
- Invoke <strong>View > Command Palette…</strong>.
- Type “install”, and select <strong>Extensions: Install Extensions</strong>.
- Type “flutter” in the extensions search field, select <strong>Flutter</strong> in the list, and click <strong>Install</strong>. This also installs the required Dart plugin.

### 3. Validate your setup with the Flutter Doctor
- Invoke  <strong>View > Command Palette… </strong>.
Type “doctor”, and select the  <strong>Flutter: - Run Flutter Doctor </strong>.
- Review the output in the OUTPUT pane for any issues. Make sure to select Flutter from the dropdown in the different  <strong>Output </strong> Options.

### 4. Create the app
Do you want to run your Flutter app on the web? The web version of Flutter is available on the beta channel. To try it out, check out the [Write your first Flutter app for the web](https://flutter.dev/docs/get-started/web) codelab.
- Invoke <strong>View > Command Palette</strong>.
- Type “flutter”, and select the <strong>Flutter: New Project</strong>.
- Enter a project name, such as <strong>myapp</strong>, and press <strong>Enter</strong>.
- Create or select the parent directory for the new project folder.
- Wait for project creation to complete and the <strong>main.dart</strong> file to appear.<br/><br/>
The above commands create a Flutter project directory called myapp that contains a simple demo app that uses [Material Components](https://material.io/design).

### 5. Run the app
- Locate the VS Code status bar.
- Select a device from the <strong>Device Selector</strong> area. For details, see Quickly switching between Flutter devices.
- Invoke <strong>Run > Start Debugging</strong> or press F5.
- Wait for the app to launch — progress is printed in the <strong>Debug Console</strong> view.