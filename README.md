# Student Profile App (Flutter)

A Student Profile Screen built for the ZenvyroLabs App Development
Internship task, using `MaterialApp`, `Scaffold`, `AppBar`, `Column`,
`Row`, `Container`, `CircleAvatar`, `Text`, `Icon`, `ElevatedButton`,
`Padding`, and `SizedBox`.

This zip includes a full Android project (the `android/` folder, Gradle
files, manifest, launcher icons, etc.) so you can open it directly in
Android Studio — you do **not** need to run `flutter create` yourself.

## Before you open it: two one-time things Android Studio needs

These two files are always machine-specific, so no zip (from me or anyone
else) can ship them pre-filled — Android Studio creates/fixes them
automatically the first time you open the project, as long as the
**Flutter** and **Dart** plugins are installed in Android Studio.

1. **`android/local.properties`** — points to your local Android SDK and
   Flutter SDK paths. Android Studio writes this file for you on first
   sync. If it doesn't, create `android/local.properties` yourself:
   ```
   sdk.dir=/path/to/your/Android/sdk
   flutter.sdk=/path/to/your/flutter
   ```
2. **Gradle wrapper jar** — if Android Studio shows a "wrapper jar
   missing/corrupt" prompt during sync, click **"Try Again"** / **"OK"**
   when it offers to regenerate it (it does this automatically). If it
   doesn't prompt, open a terminal in `android/` and run `gradle wrapper`
   once (requires Gradle installed), or simplest of all: run
   `flutter pub get` from the project root first — that alone fixes it
   in most cases.

## Step-by-step: open and run in Android Studio

1. **Install prerequisites** (skip anything you already have):
   - [Flutter SDK](https://docs.flutter.dev/get-started/install)
   - [Android Studio](https://developer.android.com/studio) with the
     **Flutter** and **Dart** plugins (Settings → Plugins → search
     "Flutter", install — it pulls in Dart automatically).
   - Run `flutter doctor` in a terminal and resolve any items it flags.

2. **Unzip** `student_profile_app.zip` anywhere on your computer.

3. **Open in Android Studio**:
   - Android Studio → **File → Open** → select the unzipped
     `student_profile_app` folder → **OK**.
   - Wait for "Gradle sync" / "Indexing" to finish (bottom status bar).
     First sync can take a few minutes since Gradle downloads
     dependencies.

4. **Get Flutter packages** — Android Studio usually does this
   automatically on open. If not: open the terminal panel in Android
   Studio (or a regular terminal, `cd` into the project) and run:
   ```
   flutter pub get
   ```

5. **Pick a device**: at the top toolbar, open the device dropdown and
   either select a running emulator (Android Studio → Device Manager to
   create one) or plug in a physical Android phone with USB debugging
   enabled.

6. **Run it**: click the green ▶️ Run button, or from a terminal:
   ```
   flutter run
   ```

7. **Push to GitHub**:
   ```
   git init
   git add .
   git commit -m "Student Profile Screen - Flutter internship task"
   git branch -M main
   git remote add origin <your-empty-github-repo-url>
   git push -u origin main
   ```

## If Gradle sync complains about versions

This project targets Android Gradle Plugin 8.1.0, Kotlin 1.9.10, and
Gradle 8.3, which work with recent Flutter/Android Studio releases. If
your installed Android Studio is older and Gradle sync fails on a version
mismatch, the fastest fix is to run this from inside the project folder:
```
flutter create .
```
This regenerates `android/` (and adds `ios/`, `web/`, etc.) using version
numbers matched to *your* installed Flutter SDK, without touching
`lib/main.dart` or `pubspec.yaml`.

## Notes

- The profile picture uses a network placeholder image
  (`https://i.pravatar.cc/300`) via `CircleAvatar` + `NetworkImage`, so
  the device/emulator needs internet access when the app runs. To use a
  local image instead:
  1. Put an image at `assets/images/profile.jpg`.
  2. In `pubspec.yaml`, uncomment the `assets:` section.
  3. In `lib/main.dart`, change `NetworkImage(...)` to
     `AssetImage('assets/images/profile.jpg')`.
- All sample data (name, university, department, etc.) is hardcoded in
  `lib/main.dart` — edit it to your own details before submitting.
- The "Edit Profile" button currently shows a SnackBar as a placeholder
  action.
- Only the Android platform folder is included (per your internship
  task, which asks for an Android Studio project). If you also need iOS
  or web later, run `flutter create .` in the project folder to add
  those platform folders too.
