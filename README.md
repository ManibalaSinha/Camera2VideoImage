
# Android Camera App (Camera2VideoImage)

A simple Android camera application demonstrating the use of the **Camera2 API** to capture **images and video** using low-level camera controls. This project shows how to initialize a camera, display preview, and record media directly within an Android app. The focus is on understanding Android’s Camera2 pipeline rather than a full UI product.

##  Project Overview

Android’s **Camera2 API** provides comprehensive control over camera hardware compared to the older, deprecated camera API. This project uses Camera2 capabilities such as:

- Opening camera devices
- Starting camera preview
- Capturing still images (JPEG)
- Recording videos
- Managing camera sessions and requests

This implementation reflects real hands-on experience working directly with camera hardware and media capture flows on Android. :contentReference[oaicite:0]{index=0}

##  Features

✔ Live camera preview  
✔ Capture still images  
✔ Record video clips  
✔ Handle camera permissions at runtime  
✔ Basic session and request management  

##  Repository Structure

```

.
├── app/
├── gradle/
├── build.gradle
├── settings.gradle
├── gradlew
└── gradlew.bat

````

##  Tech Stack

- **Android Studio (Gradle)**
- **Kotlin / Java**
- **Android Camera2 API**
- Android SDK & Build Tools

##  Getting Started

### Prerequisites

Before running the app, make sure you have:

- Android Studio installed  
- An Android device or emulator with camera support  

> Camera2 API replaces the legacy camera API and is available on most modern Android devices. :contentReference[oaicite:1]{index=1}

### Build & Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/ManibalaSinha/camera2videoimage.git
````

2. **Open in Android Studio**

   * Choose **File > Open** and select the project directory.
3. **Build & Run**

   * Connect your Android device or start an emulator.
   * Click **Run** in Android Studio.

##  Notes

* This project is intended for learning and demonstration of camera control using Camera2 API.
* It does not include full production UI/UX — the goal is functionality and pipeline understanding.
* If you want to extend it with FFmpeg for encoding/transcoding or GStreamer for real-time media pipelines, feel free to reach out!

##  What You’ll Learn

By exploring this codebase, you’ll understand:

* How to interact with Android’s Camera2 hardware interfaces
* How to configure CaptureRequests and sessions
* Media recording basics in Android
* Handling runtime permissions

#  Camera2VideoImage – Android Camera2 API Video Capture App

A native Android application demonstrating the use of the Camera2 API to capture high-quality video and convert it into a sequence of images. This project serves as a practical example for developers looking to understand and implement the Camera2 API for video processing tasks.

Architecture (Language-agnostic)

Although this project is implemented using Java and the Android SDK, the architecture is applicable across platforms and languages (including Python-based media services).

The same concepts map directly to FFmpeg/GStreamer pipelines used in backend systems.
---

##  Features

* **Camera2 API Integration**: Utilizes Android's Camera2 API for advanced camera functionalities.
* **Video Capture**: Records video with manual control over focus, exposure, and white balance.
* **Image Extraction**: Converts recorded video into individual frames (images).
* **Image Storage**: Saves extracted images in a specified directory for further processing.
* **Real-Time Preview**: Displays a live camera feed during video recording.

---

##  Setup & Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/ManibalaSinha/Camera2VideoImage.git
   cd Camera2VideoImage
   ```



2. **Open the project**:
   Open `Camera2VideoImage` in **Android Studio**.

3. **Configure permissions**:
   Ensure your `AndroidManifest.xml` includes the necessary permissions:

   ```xml
   <uses-permission android:name="android.permission.CAMERA" />
   <uses-permission android:name="android.permission.RECORD_AUDIO" />
   <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
   ```



4. **Set up camera permissions**:
   Request runtime permissions for camera and storage access in your activity.

5. **Run the application**:
   Connect an Android device or use an emulator, then run the app from Android Studio.

---

##  Project Structure

```
Camera2VideoImage/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── example/
│   │   │   │           └── camera2videoimage/
│   │   │   │               ├── CameraActivity.java
│   │   │   │               ├── Camera2Helper.java
│   │   │   │               └── VideoProcessor.java
│   │   │   └── res/
│   │   │       └── layout/
│   │   │           └── activity_camera.xml
├── build.gradle
└── AndroidManifest.xml
```



---

##  How It Works

1. **Initialize Camera2 API**: Set up the camera device and configure capture sessions.
2. **Start Video Recording**: Begin recording video with manual control over camera settings.
3. **Capture Frames**: Extract frames from the video stream at specified intervals.
4. **Save Images**: Store extracted images in the device's storage.
5. **Display Preview**: Show a live preview of the camera feed during recording.

---

##  Next Steps

* **Enhance UI**: Improve the user interface for better usability.
* **Add Filters**: Implement image filters to apply effects to captured frames.
* **Optimize Performance**: Improve the efficiency of video processing and image extraction.
* **Implement Sharing**: Allow users to share captured images via social media or email.

---

##  Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Create a new Pull Request.

---

##  Contact

* **Author**: Manibala Sinha – [GitHub Profile](https://github.com/ManibalaSinha)
* **Email**: [manibalasinha1@gmail.com](mailto:manibalasinha1@gmail.com)
