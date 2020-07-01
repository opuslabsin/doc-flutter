
---
title: "Flutter Template Installation Documentation"
keywords: 
sidebar: 
hide_sidebar: true 
search: false
permalink: index.html
summary: These instructions will help you in setup flutter template.
---

{% include note.html content="Video guide for getting Debug SHA1 fingerprint is available, checkout [https://www.youtube.com/watch?v=OQl6Me2_gEA](https://www.youtube.com/watch?v=OQl6Me2_gEA)" %}

# Introduction
This document will guide you through the process of Installtion.

# Setup

1. ### Android Setup

    **Get the Flutter SDK** [https://flutter.dev/docs/get-started/install/windows#get-the-flutter-sdk](https://flutter.dev/docs/get-started/install/windows#get-the-flutter-sdk)
    **Update your path** [https://flutter.dev/docs/get-started/install/windows#update-your-path](https://flutter.dev/docs/get-started/install/windows#update-your-path)
    **Run flutter doctor** [https://flutter.dev/docs/get-started/install/windows#run-flutter-doctor](https://flutter.dev/docs/get-started/install/windows#run-flutter-doctor)

     -  Install Android Studio 
          - Download and install [Android Studio](https://developer.android.com/studio).
         - Start Android Studio, and go through the ‘Android Studio Setup Wizard’. This installs the latest Android SDK, Android SDK Command-line Tools, and Android SDK Build-Tools, which are required by Flutter when developing for Android.
      
    -   Set up your Android device
        - To prepare to run and test your Flutter app on an Android device, you need an Android device running Android 4.1 (API level 16) or higher.
        - Enable **Developer options** and **USB debugging** on your device. Detailed instructions are available in the [Android documentation](https://developer.android.com/studio/debug/dev-options).
        - Windows-only: Install the [Google USB Driver](https://developer.android.com/studio/run/win-usb).
        - Using a USB cable, plug your phone into your computer. If prompted on your device, authorize your computer to access your device.
        - In the terminal, run the flutter devices command to verify that Flutter recognizes your connected Android device. By default, Flutter uses the version of the Android SDK where your adb tool is based. If you want Flutter to use a different installation of the Android SDK, you must set the ANDROID_SDK_ROOT environment variable to that installation directory.

    -   Set up the Android emulator
        - To prepare to run and test your Flutter app on the Android emulator, follow these steps:
        - Enable [VM acceleration](https://developer.android.com/studio/run/emulator-acceleration) on your machine.
        - Launch **Android Studio > Tools > Android > AVD Manager** and select **Create Virtual Device**. (The **Android** submenu is only present when inside an Android project.)
        - Choose a device definition and select Next.
        - Select one or more system images for the Android versions you want to emulate, and select Next. An x86 or x86_64 image is recommended.
        - Under Emulated Performance, select Hardware - GLES 2.0 to enable [hardware acceleration](https://developer.android.com/studio/run/emulator-acceleration).
        - Verify the AVD configuration is correct, and select Finish.

    -   For details on the above steps, see Managing AVDs.
         - In Android Virtual Device Manager, click Run in the toolbar. The emulator starts up and displays the default canvas for your selected OS version and device.

2. ### Install Flutter and Dart plugins
  - To install these:
      - Start Android Studio.
      - Open plugin preferences (Configure > Plugins as of v3.6.3.0 or later).
      - Select the Flutter plugin and click Install.
      - Click Yes when prompted to install the Dart plugin.
      - Click Restart when prompted. 

3. ### Run the app
   - Open Android Studio
      - Go to **File** menu
      - Click on **Open**
      - Then select the flutter project and click on open.
      - Go to lib folder in project
      - Locate the main [Android Studio toolbar](https://flutter.dev/assets/tools/android-studio/main-toolbar-857fe8c36d38020e27b502ec643ea8b1716edbe150cc6e39e3560f8fb7bda5b2.png)
      - In the **target selector**, select an Android device for running the app. If none are listed as available, select **Tools> Android > AVD Manager** and create one there. For details, see [Managing AVDs](https://developer.android.com/studio/run/managing-avds).
      - Click the run icon in the toolbar, or invoke the menu item **Run > Run**.
  

***Warning: When launching your app from a Mac, if you see ERROR: Could not connect to lockdownd, error code -17, make sure that you have trusted your computer.**
      
After the app build completes, you’ll see the app on your device.

**Note: If you are unable to understand any topic or find any topic needs more elaboration. 
Please raise an issue ticket at this link [https://opuslabs.freshdesk.com](https://opuslabs.freshdesk.com)**
