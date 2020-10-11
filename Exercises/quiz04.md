
# Chapter 04: Data & backend 
## 1. What's the different between ephemeral state and app state?
Answer: 
- Ephemeral state (sometimes called UI state or local state) is the state you can neatly contain in a single widget.
- State that is not ephemeral, that you want to share across many parts of your app, and that you want to keep between user sessions, is what we call application state (sometimes also called shared state).

## 2. Show some examples of ephemeral state.
Answer: This is, intentionally, a vague definition, so here are a few examples.
- current page in a PageView
- current progress of a complex animation
- current selected tab in a BottomNavigationBar

## 3. Show some examples of application state.
Answer: 
- User preferences
- Login info
- Notifications in a social networking app
- The shopping cart in an e-commerce app
- Read/unread state of articles in a news app

## 4. How to declare their use of the internet in Android?
Answer: Android apps must declare their use of the internet in the Android manifest (AndroidManifest.xml).
```xml
<manifest xmlns:android...>
 ...
 <uses-permission android:name="android.permission.INTERNET" />
 <application ...
</manifest>
```
## 5. What's the encoding and decoding?
Answer: Encoding and serialization are the same thing—turning a data structure into a string. Decoding and deserialization are the opposite process—turning a string into a data structure. However, serialization also commonly refers to the entire process of translating data structures to and from a more easily readable format.

## 6. Which JSON serialization method is right for me?
Answer: There are two general strategies for working with JSON:
- Use manual serialization for smaller projects
- Use code generation for medium to large projects

## 7. What's the Firebase?
Answer: Firebase is a Backend-as-a-Service (BaaS) app development platform that provides hosted backend services such as a realtime database, cloud storage, authentication, crash reporting, machine learning, remote configuration, and hosting for your static files.
