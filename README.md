# 24012011221_Raju_Practical_6_MAD

A native Android application demonstrating **Frame-by-Frame Animations**, **Tween Animations**, and custom UI layout designs built with **Kotlin** and **Android Jetpack / Material Components**.

---

## 📌 Project Overview

This project implements **Practical 6** for Mobile Application Development (MAD). It demonstrates the usage of Android animation APIs:
- **Frame-by-Frame Animation** (`AnimationDrawable`) to reveal complex graphics step-by-step and create clock/heart animations.
- **Tween Animation** (XML `<set>` with `<rotate>`, `<scale>`, `<translate>`, and `<alpha>`) for smooth vector transformations.
- **Custom XML Shape Gradients** for modern splash screen styling.
- **Activity Lifecycle Handling** for synchronized start/stop of screen animations.

---

## 🚀 Key Features

### 1. Splash Screen (`SplashActivity`)
- **Custom Linear Gradient Background**: Smooth top-to-bottom color transition (`#87A9FF` light blue → `#B4A4EA` lavender → `#EEA2CB` pink).
- **Sequential Logo Build (Frame Animation)**: Logo components (`uvpce_logo_1` through `uvpce_logo`) appear step-by-step.
- **360° Rotation (Tween Animation)**: Once the entire logo is assembled, it rotates 360 degrees around its center pivot point before navigating to the main screen.

### 2. Main Screen (`MainActivity`)
- **Alarm Clock Animation**: Frame-by-frame animation cycling through clock states.
- **Heartbeat Pulse Animation**: Cyclic frame-by-frame heart icon animation.
- **Live Digital Clock**: Real-time 12-hour formatted time and date (`hh:mm:ss a dd MMM yyyy`) via `TextClock`.
- **Interactive UI Card**: Material3 card container with elevation and corner rounding containing action buttons (`Create Alarm`, `Cancel Alarm`).

---

## 🛠️ Tech Stack & Requirements

- **Language**: Kotlin
- **Build System**: Gradle (Kotlin DSL `build.gradle.kts`)
- **Min SDK**: 24 (Android 7.0)
- **Target SDK**: 37
- **UI Components**: AndroidX AppCompat, Material Components (`MaterialCardView`), ConstraintLayout

---

## 📂 Project Structure

```text
app/src/main/
├── java/com/example/a24012011221_raju_practical_6_mad/
│   ├── SplashActivity.kt          # Splash screen logic (Frame + Tween animation sequence)
│   └── MainActivity.kt            # Main activity controlling card & clock animations
├── res/
│   ├── anim/
│   │   ├── twin_animation.xml     # Tween rotation XML animation set
│   │   └── twin_animation.xml     # Property animation definitions
│   ├── drawable/
│   │   ├── rectangle_gradient.xml # Linear top-to-bottom gradient background
│   │   ├── uvpce_animation_list.xml# Frame animation list for splash logo
│   │   ├── alarm_animation_list.xml# Frame animation list for alarm clock
│   │   └── heart_animation_list.xml# Frame animation list for heart icon
│   └── layout/
│       ├── activity_splash.xml    # Splash screen layout
│       └── activity_main.xml      # Main screen layout
└── AndroidManifest.xml
```

---

## ⚙️ How to Build and Run

1. Open the project folder in **Android Studio**.
2. Perform a Gradle Sync (`File -> Sync Project with Gradle Files`).
3. Connect an Android device or start an Android Virtual Device (AVD).
4. Click **Run** (`Shift + F10`) or execute `./gradlew app:assembleDebug` in terminal.

---

## 👤 Author

- **Name**: Raju
- **Enrollment No**: 24012011221
- **Course**: SEM V MAD Practical 6
