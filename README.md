<h1>A collection of offline HTML games.</h1>

<p>A repo filled with 352 offline games that can each run on a single file. This is a good option if you are having internet connectivity issues, or you're at some place with <i>restricted internet</i>.</p>

Most of these games are from the [Ultimate Game Stash](https://docs.google.com/document/u/4/d/1_FmH3BlSBQI7FGgAQL59-ZPe8eCxs35wel6JUyVaG8Q) but turned offline.

**Usage:** Under the Code button, select Download ZIP. It may take a while to download. After, extract the zip by right clicking on it and selecting Extract All. Now you have the repo containing the games all in a folder. You can also clone the repository using git.


The downside of inlining everything is the file size. If you're running the files via a code editor, it's better to use **single-file.html**. It lets you fetch the files from the web or import your own.


<br>

# For **Chromebooks** - See [chromeOS.md](methods/chromeOS.md)



## Build an offline Android APK

This repository contains many large self-contained HTML games, so the Android build packages **one game per APK**. This keeps each APK installable and within GitHub artifact limits while preserving fully offline play.

1. Open the **Actions** tab and select **Build offline game APK**.
2. Click **Run workflow** and enter a file such as `offline/2048.html` or `offline/google-dino.html`.
3. Download the `offline-game-apk` artifact from the completed workflow run and install the APK on Android. Enable installation from the browser/file manager when Android asks.

The APK has no network permission and loads the selected game from bundled app assets. The workflow accepts only files under `offline/` with an `.html` or `.htm` extension.
