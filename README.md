# How to use AudioHelper in Unity

JAR file, demo apk are in /resource.    
Note: Regarding JAR file creation and usage, please refer to [the Guideline](http://static.appstore.picovr.com/docs/JarUnity/index.html)

## Introduction
This demo provides a method for recording audio via mic.

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
