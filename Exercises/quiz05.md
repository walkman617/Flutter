
# Chapter 05: Accessibility & internationalization 
## 1. How can the developers make their apps more accessible?
Answer: Flutter is committed to supporting developers in making their apps more accessible, and includes first-class framework support for accessibility in addition to that provided by the underlying operating system, including:

- Large fonts: Render text widgets with user-specified font sizes
- Screen readers: Communicate spoken feedback about UI contents
- Sufficient contrast: Render widgets with colors that have sufficient contrast

## 2. Show an accessibility release checklist.
Answer: Here is a non-exhaustive list of things to consider as you prepare your app for release.

- <strong>Active interactions.</strong> Ensure that all active interactions do something. Any button that can be pushed should do something when pushed. For example, if you have a no-op callback for an onPressed event, change it to show a SnackBar on the screen explaining which control you just pushed.
- <strong>Screen reader testing.</strong> The screen reader should be able to describe all controls on the page when you tap on them, and the descriptions should be intelligible. Test your app with TalkBack (Android) and VoiceOver (iOS).
- <strong>Contrast ratios.</strong> We encourage you to have a contrast ratio of at least 4.5:1 between controls or text and the background, with the exception of disabled components. Images should also be vetted for sufficient contrast.
- <strong>Context switching.</strong> Nothing should change the user’s context automatically while typing in information. Generally, the widgets should avoid changing the user’s context without some sort of confirmation action.
- <strong>Tappable targets.</strong> All tappable targets should be at least 48x48 pixels.
- <strong>Errors.</strong> Important actions should be able to be undone. In fields that show errors, suggest a correction if possible.
- <strong>Color vision deficiency testing.</strong> Controls should be usable and legible in colorblind and grayscale modes.
- <strong>Scale factors.</strong> The UI should remain legible and usable at very large scale factors for text size and display scaling.

## 3. How to set up an internation­alized app?
Answer: By default, Flutter only provides US English localizations. To add support for other languages, an application must specify additional MaterialApp properties, and include a separate package called flutter_localizations. 

## 4. How to track the locale?
Answer: The Locale class and the Localizations widget.
- The Locale class identifies the user’s language. 
- The Localizations widget defines the locale for its child and the localized resources that the child depends on. 


## 5. How to load and retrieve localized values?
Answer: The Localizations widget is used to load and lookup objects that contain collections of localized values. Apps refer to these objects with Localizations.of(context,type). 
