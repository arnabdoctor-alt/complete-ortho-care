# Operative Logbook – Android app

## Easiest: build the APK online (no Android Studio)
1. Create a free account at github.com and make a new PRIVATE repository.
2. Upload everything in this folder (keep the .github folder) and commit to the main branch.
3. Open the repo > Actions > "Build Android APK" > wait about 5 minutes for the green tick.
4. Open the finished run, download the "operative-logbook-apk" artifact, unzip it.
5. Copy app-debug.apk to your phone, tap it, and allow "Install unknown apps" when asked.

## Or build locally
Needs Node 18+, JDK 17 and Android Studio.
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android    (then Build > Build APK)

Data stays on the phone (IndexedDB). Export CSV or backup opens the Android share sheet.
