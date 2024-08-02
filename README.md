### README.md

# Shake Detection Android App

This is a simple Android app that detects when the device is shaken and displays a message. The app uses the accelerometer sensor to detect shake events.

## Screenshots 
![Sensor jpg](https://github.com/user-attachments/assets/56fb369b-e2de-414d-b3a7-692241955d18)

## Features

- Shake Detection: Detects when the device is shaken.
- Display Message: Shows a toast message "Shaken, not stirred!" when a shake is detected.

## Prerequisites

- Android Studio
- Android SDK
- Java JDK

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Step 1: Create a New Android Project

1. Open Android Studio.
2. Click on `File > New > New Project`.
3. Select `Empty Activity` and click `Next`.
4. Name your project, choose a save location, select Java as the language, and set the minimum SDK.
5. Click `Finish`.

### Step 2: Add Permissions (`AndroidManifest.xml`)

Add the required permissions for accessing the accelerometer sensor in your `AndroidManifest.xml`:
xml
<uses-permission android:name="android.permission.WAKE_LOCK" />
<uses-permission android:name="android.permission.VIBRATE" />


### Step 3: Test Your App

1. Connect your Android device or start an emulator.
2. Click on the `Run` button in Android Studio.
3. Select your device/emulator and click `OK`.
4. Shake the device, and you should see a toast message saying "Shaken, not stirred!" when a shake is detected.

## Project Structure

```
├── app
│   ├── src
│   │   ├── main
│   │   │   ├── java
│   │   │   │   └── com
│   │   │   │       └── example
│   │   │   │           └── shakedetector
│   │   │   │               └── MainActivity.java
│   │   │   ├── res
│   │   │   │   ├── layout
│   │   │   │   │   └── activity_main.xml
│   │   │   ├── AndroidManifest.xml
├── build.gradle
└── README.md

## Insights

- This project demonstrates the use of the accelerometer sensor to detect shake events.
- It includes handling of runtime permissions, which is crucial for accessing sensitive device data.
- The project is a great starting point for building more complex sensor-based applications, such as motion-based games, fitness trackers, or gesture-controlled interfaces.
