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



🧩 Core Concepts Demonstrated (Study Points)

Intent: Messaging object to request an action from another component.




Types of Intent:

Explicit Intent: Starts a specific component by name (e.g., LoginActivity).

Implicit Intent: Declares a general action and lets the system resolve an app to handle it.



Types of Intent Actions: Predefined constants such as ACTION_VIEW, ACTION_DIAL, MediaStore.ACTION_IMAGE_CAPTURE, AlarmClock.ACTION_SET_ALARM.

Intent.setData(): Sets data for the intent, usually a Uri.

Intent.setType(): Specifies MIME type for the intent’s data.

UI Components Used:

Button for actions.

EditText for user input (URL/phone number).

ConstraintLayout / CoordinatorLayout for layout design.

Starting Activities: Using startActivity(intent) to launch activities.

Handling Missing Apps: Prevent crashes by checking with resolveActivity() or using try-catch.

URI Parsing: Uri.parse() for converting strings into usable URIs.

Permissions (Conceptual):

Manifest Permissions (e.g., CALL_PHONE for direct calls).

Runtime Permissions for Android 6.0+ when required.



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

Main Screen: Acts as the central hub with buttons to access all intent actions.


<img width="492" height="773" alt="image" src="https://github.com/user-attachments/assets/1e403abe-e82a-4b96-999c-5d2baff7d0be" />


Opening a URL: Allows the user to enter a link and open it in the web browser.

Making a Phone Call: Lets the user enter a number and open the dialer to call.

Opening Gallery: Opens the gallery app to view stored images and media.

Launching Camera: Starts the device camera to capture photos.

Setting Alarm: Opens the clock app to set or view alarms.

Navigating to LoginActivity: Demonstrates explicit intent by opening the login screen.

RegisterActivity Navigation: From the login screen, users can move to the register screen.

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
