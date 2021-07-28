# How to use AudioHelper in Unity

- If you have any questions/comments, please visit [**Pico Developer Answers**](https://devanswers.pico-interactive.com/) and raise your question there.

JAR file, demo apk are in /resource.    
Note: Regarding JAR file creation and usage, please refer to [the Guideline](http://static.appstore.picovr.com/docs/JarUnity/index.html)

## Introduction
This demo provides a method for recording audio via mic.
The file is saved in this path(/sdcard/Record/) and named according to the created time.

## Class name
```
com.picovr.library.AudioHelper
```

## Permission
```
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>    
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO" />
```

## Interface
```
public void startRecordByMIC()
public void stopRecordByMIC()
```

## Sample Code
```
AndroidJavaObject audioHelper = new AndroidJavaObject("com.picovr.library.AudioHelper");

audioHelper.Call("startRecordByMIC");
audioHelper.Call("stopRecordByMIC");
```
