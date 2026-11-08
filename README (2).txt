Padel Tournaments - Android project
===================================

Build the APK (Android Studio, easiest)
1. Install Android Studio (free): https://developer.android.com/studio
2. File > Open, choose this PadelTournaments folder. Let it finish syncing
   (it downloads what it needs, so be online the first time).
3. Build > Build Bundle(s) / APK(s) > Build APK(s).
4. Click "locate" in the pop-up. The file is app-debug.apk
   (app/build/outputs/apk/debug/app-debug.apk).

Install on your phone
1. Copy app-debug.apk to the phone (USB, Drive, WhatsApp to yourself, email).
2. Tap it. If asked, allow "Install unknown apps" for the app you opened it from.
3. Open "Padel Tournaments".

Notes
- Tournaments are saved on the phone and work with no internet.
- The Barlow fonts load from Google when online; offline the app uses system fonts.
- The app is app/src/main/assets/index.html (one file). Edit it to change the app.

Build in the cloud with GitHub (no Android Studio needed)
1. Make a free account at github.com and create a new repository (any name).
2. In the repository click Add file > Upload files. Drag in everything inside
   this PadelTournaments folder, including the hidden .github folder, then Commit.
   If .github did not upload: Add file > Create new file, type
   .github/workflows/build.yml as the name, paste in the contents of build.yml, Commit.
3. Open the Actions tab. "Build APK" runs by itself (about 3-5 minutes).
   If it does not, click it, then Run workflow.
4. Open the finished run and download PadelTournaments-apk from Artifacts.
   Unzip it to get app-debug.apk, copy that to your phone and tap it to install.
