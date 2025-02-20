# **RTSP Video Stream App (Kotlin)**  

This is an Android app for streaming **RTSP video** using **ExoPlayer (Media3)**.  

## **Setup & Installation**  

1. Clone the repository:  
   ```sh
   git clone https://github.com/Anas-AppDev/RTSP-Video-Stream-App.git
   ```
2. Open the project in **Android Studio**.  
3. Add the following dependencies in `build.gradle.kts`:  
   ```kotlin
   implementation("androidx.media3:media3-exoplayer:1.2.0")
   implementation("androidx.media3:media3-exoplayer-rtsp:1.2.0")
   implementation("androidx.media3:media3-ui:1.2.0")
   ```
4. Sync Gradle and **build the project**.  
5. Run the app on an **Android device** (minSdk 24+).  

## **How to Use**  

1. **Launch the app** on your Android device.  
2. **Enter an RTSP stream URL** in the input field.  
3. Tap **Play** to start streaming.  
4. Use **play/pause controls** to manage playback.  

## **Common Issues & Fixes**  

### **Issue: `useController` not found**  
**Fix:** Ensure `media3-ui` is added and use `app:use_controller="true"`.  

### **Issue: RTSP stream not loading**  
**Fix:** Verify the **RTSP URL format** and check if the source is accessible.  

## **Future Improvements**  
- Support for **RTMP & HLS** streams.  
- **Background streaming** support.  
- **Recording & snapshots** feature.  
