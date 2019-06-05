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
