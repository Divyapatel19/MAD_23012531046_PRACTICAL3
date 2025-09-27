📱 Android Intent Demonstration Application


 AIM

This Android application serves as a practical demonstration of using both Implicit and Explicit Intents to perform various common actions and navigate between activities.



📖 Description

The project highlights how Intents are used in Android to interact with system applications or other components. Explicit Intents are used to navigate between activities within the app (e.g., opening LoginActivity), while Implicit Intents are used to request actions from system apps (e.g., opening the camera, gallery, or call log).



⚡ Functionalities Implemented

Make a Call: Initiates a phone call to a user-specified number.

Open URL: Launches a web browser to display a user-specified webpage.

Open Call Log: Displays the device's call history.

Open Gallery: Allows the user to view images using a gallery app.

Set Alarm: Opens the alarm clock app to set or view alarms.

Open Camera: Launches the camera app to capture an image.

Open Login Activity: Navigates to a dedicated LoginActivity within the application.



 📘 Core Concepts Demonstrated (Study Points)

This project demonstrates several important Android concepts:

* **Intent**: A messaging object used to request an action from another component (start an activity, service, or broadcast).

* **Types of Intents**:

  * **Explicit Intent**: Directly specifies the target component (e.g., `LoginActivity`). Used within the same app.
  * **Implicit Intent**: Specifies a general action, and the system decides which app can handle it (e.g., open a URL, make a call).

* **Intent Actions**: Predefined constants that describe actions, such as:

  * `Intent.ACTION_VIEW` → Open content like a web page or gallery.
  * `Intent.ACTION_DIAL` → Open dialer with a number.
  * `MediaStore.ACTION_IMAGE_CAPTURE` → Open camera.
  * `AlarmClock.ACTION_SET_ALARM` → Set an alarm.

* **Intent.setData()**: Sets data for the intent in the form of a `Uri` (e.g., `tel:` for numbers, `http:` for websites).

* **Intent.setType()**: Defines the data type (MIME type), such as `"image/*"` for images or `CallLog.Calls.CONTENT_TYPE` for call logs.

* **UI Components Used**:

  * **Button** → Triggers actions when clicked.
  * **EditText** → Allows user input (e.g., phone number, URL).
  * **ConstraintLayout** → Flexible layout for designing UIs.
  * **CoordinatorLayout** → Provides advanced control for UI interactions (optional in layouts).

* **Starting Activities**: `startActivity(intent)` is used to launch another activity.

* **Handling Missing Apps**: Use `resolveActivity()` or a `try-catch` block to avoid crashes if no app can handle an intent.

* **URI Parsing**: `Uri.parse()` converts a string into a usable `Uri` for intents.

* **Content Types (Examples)**:

  * `tel:` → Telephone number.
  * `"image/*"` → Any image file.
  * `CallLog.Calls.CONTENT_TYPE` → Call log entries.

* **Permissions (Concepts)**:

  * **Manifest Permissions**: Declared in `AndroidManifest.xml` (e.g., `CALL_PHONE` for direct calls).
  * **Runtime Permissions**: Required in Android 6.0+ for sensitive actions.
  * **ContextCompat.checkSelfPermission()** → Checks if permission is granted.
  * **ActivityCompat.requestPermissions()** → Requests permission from user.

👉 Note: Many common intents (dialer, browser, gallery, camera, alarm) don’t require direct permissions because the target app manages them.





📂 Project Structure

The project follows the standard Android app structure. The main functionality is implemented in MainActivity, while navigation with explicit intents is demonstrated using LoginActivity and RegisterActivity. Layout files are stored under the res/layout folder, and shared resources like strings, colors, and styles are under res/values. The AndroidManifest.xml file defines all declared activities and permissions.

MainActivity.kt: Entry point of the app, contains buttons to trigger implicit/explicit intents.

LoginActivity.kt: Activity for demonstrating explicit intent navigation.

RegisterActivity.kt: Activity linked from LoginActivity for a simple login/registration flow.

res/layout/activity_main.xml: UI layout for the main screen.

res/layout/activity_login.xml: UI layout for the login screen.

res/layout/activity_register.xml: UI layout for the register screen.

AndroidManifest.xml: Declares activities and permissions.



📷 Demonstration Screenshots

1.Main Screen: 

Acts as the central hub with buttons to access all intent actions.


<img width="200" height="280" alt="image" src="https://github.com/user-attachments/assets/1e403abe-e82a-4b96-999c-5d2baff7d0be" />




2.Opening a URL: 

Allows the user to enter a link and open it in the web browser.


<img width="200" height="280" alt="browse" src="https://github.com/user-attachments/assets/8ebd4fb7-7c06-4493-a0d0-31ee8c101a56" />





3.Making a Phone Call: 

Lets the user enter a number and open the dialer to call.

<img width="200" height="280" alt="call" src="https://github.com/user-attachments/assets/2a9626da-4bea-48ba-8d30-863033d28bfc" />




4.Opening Gallery:

Opens the gallery app to view stored images and media.


<img width="200" height="280" alt="gallary" src="https://github.com/user-attachments/assets/4f252751-2899-43a4-976a-0f29deabbf6e" />


5.Launching Camera:

Starts the device camera to capture photos.

<img width="200" height="280" alt="camero" src="https://github.com/user-attachments/assets/e87620db-ad11-49b9-9c78-11d4c82e3cfc" />



6.Setting Alarm:

Opens the clock app to set or view alarms.

<img width="200" height="280" alt="alarm" src="https://github.com/user-attachments/assets/8f949747-78c5-4f60-8af1-355e8b0dbc0d" />


7.Navigating to LoginActivity: 

Demonstrates explicit intent by opening the login screen.

<img width="200" height="280" alt="login" src="https://github.com/user-attachments/assets/7b10c538-a083-4cb0-b89e-d46bb0a46e13" />


8.RegisterActivity Navigation:

From the login screen, users can move to the register screen.

<img width="200" height="280" alt="register" src="https://github.com/user-attachments/assets/c9c0604f-d3b6-4499-9168-da4a5c4515a9" />



🎓 Learning Outcomes

By working on this application, you will:

Understand the differences between explicit and implicit intents.

Learn how to construct intents with actions, data, and types.

Explore launching system apps such as dialer, browser, gallery, and camera.

Practice navigating between activities in your own app.

Gain experience in UI design using layouts, buttons, and input fields.

Understand permission handling and app crash prevention when intents cannot be resolved.



✅ Conclusion

This project serves as a foundational example of inter-component communication in Android development, demonstrating both system-level interactions and in-app navigation.
