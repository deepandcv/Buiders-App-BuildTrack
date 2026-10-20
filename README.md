# Build Steps

# LOCAL BUILD [Windows/Mac]
npm install
npx cap add android
npx cap sync
npx cap open android  -> Click Run/Build > Build APK in Android Studio

# CLOUD BUILD [No Android Studio Needed]
1. Create GitHub repo, upload this folder
2. Go to Actions tab -> Build APK -> Download APK artifact
3. Install on phone

# PLAY STORE RELEASE
android/app/build.gradle -> versionCode 3, versionName "3.0"
Generate signed bundle: Build > Generate Signed Bundle/APK in Android Studio
