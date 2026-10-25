# Salary Gayeb - Android build

## Easiest: get the APK with GitHub (no Android Studio)
1. Create a new GitHub repo and upload everything in this folder (keep the .github folder).
2. Open the repo > Actions tab > "Build APK" > wait about 5 minutes.
3. Open the finished run, download "salary-gayeb-apk" (a zip containing app-debug.apk).
4. Copy app-debug.apk to your phone and install it (allow "Install unknown apps").

## Or build locally (Android Studio + Node 20 + JDK 17)
npm install && npx cap add android && npx cap sync android && npx cap open android
Then Build > Build APK(s).

The app UI lives in www/index.html. Replace parseSmsForAmount() there when you add real SMS reading.
