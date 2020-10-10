## Status Bar is White

  `<item name="android:statusBarColor">@android:color/transparent</item>`
Remove above line of code in `values/styles/styles.xml(v21)`


## DataBinding doesn't generate the Binding classes
  
  Enable Databinding in app manifest, 
  Make the layouts as dataBinding layouts,
  Clean & Rebuild the project
  
## MainApplication class is not found the project

  Create a custom class `AppX` extends from Application()
  In the Manifest file, under `<Application>` tag, add `android:name=".AppX"`

## When Project is moved to a different location, you get "App installation failed Error"
  
  Goto: Android Studio - Preferences (In OSX)
  Then to: Build,Execution,Deployment - Instant run
  And: Un-check (Enable Instant Run to hot swap code)

## 'Start Rollout to Production' is disable in the Google Play Console
  
  All the required steps must be completed
    - App Content
    - App Release
    - Store Listing
    - Content Rating
    - Pricing and distribution
    
## When you want to rename the package of an android project

  In Android Studio's left Project pane, tap on the gear icon and unselect `Compact Empty Middle Packages`
  Then,right click on the package name, Refactor and rename
  
## Android App Release process
  
  The aab/apk that you want to release to appstore must be signed with a cryptographic key. For that, you need a key store and secure key. For the first time when you want to create a release APK, You can create one witht the help of Android Studio. 
  - Tap `Build > Generate Signed Bundle/APK`
  - Under key store path, select `Create New KeyStore`
  - Choose path where you want to store the key store and create a secure password
  - Then a create secure password for the Key and provide additional details, then select OK
  - Then in the following page, Choose APK destination folder, and build type to release. Finishing will generate release APK/AAB based on your selection. You can use it to release on APP Store or for a private testing
  
  ## Required icons and images
  
   You need a proper App icon with different DPI levels, a frame graphic and an appstore icon. Each of the resolution details are mentioned below.
    
    |  Name  | DPI | Multiplier | Resolution |
    |--------|-----|------------|------------|
    | mdpi   | 160 | 1x         | 48 * 48    |
    | hdpi   | 240 | 1.5x       | 72 * 72    |
    | xhdpi  | 320 | 2x         | 144 * 144 |
    | xxhdpi  | 480 | 3x         | 192 * 192 |
    | xxxhdpi | 640 | 4x | 512 * 512 |
    | frame graphic | x | x | 1024 * 500 |
    

## Worker Manager
https://towardsdatascience.com/working-with-android-workmanager-using-kotlin-36167a143579


