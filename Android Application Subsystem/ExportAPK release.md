
**NOTE: Leave out the alias part as it may not work**

1) Build -> Generate Signed APK

2) Create Keystore

3) Set password for keystore

3.1) Set key  

3.2 ) Set password for key

4) Fill organization name : Sample

5) Fill organization : Sample

Next -> finish

**NOTE: You can also use the same key that you used for debug in the release version but not recommended due to security reasons!**

**Idea:** In android view (left window/pane/side bar) by default.

Switch to Project from android view.

In project:

app -> src -> debug -> res -> values -> google_maps_api.xml

Use the same key in

app -> src -> debug -> res -> values -> google_maps_api.xml

**SECURE VERSION: This is NOT Secure version this is MANDATORY - ignore the previous note** 

Oracle JDK path on my system: In Program Files (x86) not program files!!

cd to 

C:\Program Files (x86)\Java\jdk 1.8 (press tab)\bin

Use this command with your credentials...

keytool -list -v -keystore C:\Users\MG\Desktop\test.jks -alias test

Get sha1 & use it in your google maps api developers console (after signing in to google maps api dev console -> restrict app)

This is for your release key :)

LESSON:

1) You can use the same key for debug and release in case of Google Maps Activity - but you have to add the SHA - 1 key from keystore to your app in case of release apk

2) If can't install apk on phone - uninstall the previous version of the application.

3) For release, the api key needs to be hardcoded in the android manifest file.

4) 


