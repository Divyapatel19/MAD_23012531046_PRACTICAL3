
Practical-3:


 AIM:Create an Android application that demonstrates the use of **Implicit** and **Explicit Intents** in Android.

* Description
This project showcases how to use Intents in Android applications to perform common system actions and navigate between activities.

- Intent: Used to launch a specific activity within the app (e.g., navigating to **LoginActivity**).
- Implicit Intent: Used to request an action from another application or system service (e.g., opening the camera, gallery, call log, or making a call).

The application provides buttons for each functionality, allowing users to easily explore how Intents work in real-world Android apps.

*Features Implemented

1. Make Call to Specific Number
   * Opens the dialer or directly initiates a phone call to a given number.

2. Open Specific URL
   * Launches the web browser with a provided website URL.

3. Open Call Log
   * Displays the phone’s call history.

4. Open Gallery
   * Opens the gallery to view images and videos stored on the device.

5. Set Alarm
   * Creates an alarm in the device’s default clock application.

6. Open Camera
   * Launches the device’s camera application for capturing photos or videos.

7. Open Login Activity (Explicit Intent)
   * Demonstrates **Explicit Intent** by navigating to a custom **LoginActivity** inside the app.

Technologies Used

* Language: Kotlin / Java (as per implementation)
* IDE: Android Studio
* Android Components:

  * `Intent` (Implicit & Explicit)
  * `Button`, `EditText`
  * `ConstraintLayout` / `CoordinatorLayout`
  * 
# How It Works

* Each button in the main activity is mapped to a specific intent.
* When the user clicks a button, the corresponding intent is triggered.

* For example:
  * Clicking **"Open Camera"** launches the system camera app.
  * Clicking **"Login Activity"** navigates to another activity within the app.

# Project Structure

Practical3-Intents/
app
java/com.example.intentsdemo/

MainActivity.java / MainActivity.kt

LoginActivity.java / LoginActivity.kt

res/

layout/activity_main.xml

layout/activity_login.xml

values/strings.xml

values/colors.xml

values/styles.xml

AndroidManifest.xml

README.md

# Screenshots (Optional to Add)

# Learning Outcomes
* Understood the concept of **Intents** in Android.
* Learned the difference between **Implicit** and **Explicit** Intents.
* Implemented real-world use cases such as opening system apps and navigating between activities.
