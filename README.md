# Experiment 4: Linking Activities using Intents

## Student Details

**Name:** Mohammed Kaif ulla 
**USN:** 25MCAR0226  
**Experiment No.:** 4

---

## Aim

To develop an Android application to demonstrate linking activities using Intents.

---

## Objective

The objective of this experiment is to understand how Android Activities can be linked with each other using Intents and how navigation can be performed from one Activity to another.

---

## Concept / Technology Used

### Intent

An Intent is a messaging object used in Android to request an action from another application component.

In this experiment, an **Explicit Intent** is used to navigate from `MainActivity` to `SecondActivity`.

An Explicit Intent specifies the exact Activity that needs to be started.

Example:

```kotlin
val intent = Intent(this, SecondActivity::class.java)
startActivity(intent)
```

The `finish()` method can be used to close the current Activity and return to the previous Activity.

```kotlin
finish()
```

---

## Scenario

The application contains two Activities:

1. **MainActivity**
   - Acts as the first screen of the application.
   - Contains a button to open the second Activity.
   - Displays the main application interface.

2. **SecondActivity**
   - Opens when the user clicks the navigation button.
   - Displays the second screen of the application.
   - Provides navigation back to the previous Activity.

### Application Flow

```text
MainActivity
     |
     | Click Button
     ↓
Explicit Intent
     |
     ↓
SecondActivity
     |
     | Click Back
     ↓
MainActivity
```

---

## Software Requirements

- Android Studio
- Kotlin
- Android SDK
- Gradle
- Android Emulator or Physical Android Device

---

## Technologies Used

- Kotlin
- Android Activities
- Explicit Intent
- XML Layouts
- Android Manifest
- Android SDK

---

## Project Folder and File Structure

```text
MADExperiment4/
│
├── app/
│   │
│   ├── src/
│   │   │
│   │   └── main/
│   │       │
│   │       ├── java/
│   │       │   └── com/example/madexperiment4/
│   │       │       ├── MainActivity.kt
│   │       │       └── SecondActivity.kt
│   │       │
│   │       ├── res/
│   │       │   ├── drawable/
│   │       │   ├── layout/
│   │       │   │   ├── activity_main.xml
│   │       │   │   └── activity_second.xml
│   │       │   ├── mipmap/
│   │       │   └── values/
│   │       │
│   │       └── AndroidManifest.xml
│   │
│   └── build.gradle.kts
│
├── gradle/
│   └── wrapper/
│
├── build.gradle.kts
├── gradle.properties
├── settings.gradle.kts
├── gradlew
├── gradlew.bat
├── screenshot.png
└── README.md
```

---

## Important Files and Their Purpose

### MainActivity.kt

`MainActivity.kt` is the first Activity of the application. It contains the main user interface and provides a button to open `SecondActivity`.

### SecondActivity.kt

`SecondActivity.kt` represents the second screen of the application. It is opened from `MainActivity` using an Explicit Intent.

### activity_main.xml

This XML file defines the user interface of the main Activity.

### activity_second.xml

This XML file defines the user interface of the second Activity.

### AndroidManifest.xml

The Android Manifest contains the application configuration and Activity declarations required by the Android system.

### build.gradle.kts

This file contains the Android application build configuration and required dependencies.

---

## Working / Implementation

### 1. MainActivity

The application starts from `MainActivity`.

When the user clicks the button, an Explicit Intent is created to open `SecondActivity`.

```kotlin
val intent = Intent(this, SecondActivity::class.java)
startActivity(intent)
```

### 2. SecondActivity

After the Intent is executed, `SecondActivity` is displayed.

The user can return to the previous Activity using:

```kotlin
finish()
```

### 3. Activity Linking

The application demonstrates Activity-to-Activity navigation using an Explicit Intent.

```text
MainActivity
      ↓
Explicit Intent
      ↓
SecondActivity
```

---

# Test Cases

## Test Case 1: Application Launch

### Test Objective

To verify that the Android application launches successfully.

### Test Steps

1. Run the application.
2. Launch the application on an emulator or physical Android device.
3. Observe the first screen.

### Expected Result

`MainActivity` should open successfully.

### Actual Result

`MainActivity` opened successfully.

### Status

**PASS ✅**

---

## Test Case 2: Navigate to Second Activity

### Test Objective

To verify that the application successfully links `MainActivity` with `SecondActivity` using an Explicit Intent.

### Test Steps

1. Launch the application.
2. Click the button provided on `MainActivity`.
3. Observe the screen.

### Expected Result

`SecondActivity` should open successfully.

### Actual Result

`SecondActivity` opened successfully using an Explicit Intent.

### Status

**PASS ✅**

---

## Test Case 3: Verify Student Name and USN

### Test Objective

To verify the student's name and USN.

### Test Data

**Name:** Tejas Sunil Waske  
**USN:** 25MCAR0189

### Test Steps

1. Launch the application.
2. Navigate to the screen containing the student information.
3. Verify the student's name.
4. Verify the USN.

### Expected Result

The correct student name and USN should be displayed.

### Actual Result

The student's name and USN were verified successfully.

### Status

**PASS ✅**

---

# Output

The application successfully demonstrates linking two Android Activities using an Explicit Intent.

### Output Screenshot

<img width="732" height="1600" alt="MAD 4" src="https://github.com/user-attachments/assets/7573d074-9057-402a-8a9a-f03a20163d4d" />
<img width="1080" height="2358" alt="mad exp 4 b" src="https://github.com/user-attachments/assets/c770c918-b74f-46a8-96b5-487c955dab87" />

---

# Steps to Run the Project

1. Open the project in Android Studio.
2. Allow Gradle synchronization to complete.
3. Connect an Android device or start an Android Emulator.
4. Select the application from the Run Configuration.
5. Click the **Run ▶** button.
6. The application will launch on the selected device.
7. Click the navigation button to open `SecondActivity`.

---

# Requirements

## Hardware Requirements

- Laptop/Desktop
- Android Device or Android Emulator
- USB Cable if using a physical Android device

## Software Requirements

- Android Studio
- Kotlin
- Android SDK
- Gradle

---

# Learning Outcomes

After completing this experiment, the following concepts were understood:

- Android Activities
- Intent
- Explicit Intent
- Activity-to-Activity navigation
- `startActivity()`
- `finish()`
- AndroidManifest.xml
- XML Layouts
- Android application navigation

---

# Result

The Android application was successfully developed and executed to demonstrate linking Activities using Explicit Intents.

---

# Conclusion

The experiment successfully demonstrated how two Android Activities can be linked using an Explicit Intent.

The application navigates from `MainActivity` to `SecondActivity` using `startActivity()`. The user can also return to the previous Activity using `finish()`.

Thus, the objective of implementing an Android application to demonstrate linking Activities using Intents was successfully achieved.

---

# Student Information

**Name:** Mohammed Kaif ulla
**USN:** 25MCAR0226

---

# GitHub Repository

**Repository Name:** MAD LAB EXP 4

**GitHub Link:**  
https://github.com/MohdKaifUlla/MAD-LAB-EXP-4

---

# Reference

- Android Developers – Activities
- Android Developers – Intents
- Android Developers – Activity Navigation

---

## Author

**Mohammed Kaif ulla**  
**USN:** 25MCAR0226
