BRAINSTORM BRAWL - Android app project
=======================================

OPTION A - Build the APK on GitHub (no installs needed)
1. Go to github.com and create a NEW repository (e.g. "brainstorm-brawl"). Public or private is fine.
2. Unzip BrainstormBrawl-android.zip on your computer.
3. In the new repo, click "uploading an existing file" and drag EVERYTHING inside the
   BrainstormBrawl folder (including the ".github" folder) into the page. Click "Commit changes".
   * If the .github folder does not upload: click Add file > Create new file, type the name
     .github/workflows/build-apk.yml and paste the contents of that file from the zip.
4. Open the "Actions" tab. A run called "Build APK" starts by itself (about 3-5 minutes).
5. When it shows a green check, open the run, scroll down to "Artifacts",
   and download "BrainstormBrawl-APK". Unzip it to get app-debug.apk.
6. Send app-debug.apk to your phone and open it. Allow "Install unknown apps" when asked.

OPTION B - Build in Android Studio
1. Open Android Studio > Open > select the BrainstormBrawl folder. Wait for Gradle sync.
2. Build > Build App Bundle(s) / APK(s) > Build APK(s).
3. Click "locate" in the popup to find app-debug.apk.

NOTES
- The app works offline. Progress is saved on the phone.
- Online battle works when both phones have internet (it uses the free PeerJS server).
- The phone Back button goes back a screen, pauses a match, or exits from the home screen.
- Game files are in app/src/main/assets. To update the game, replace index.html / img there and rebuild.
