<div align="center">

# 🎓 Student Profile App

### A clean, minimal Student Profile Screen built with Flutter

<p>
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/status-completed-brightgreen?style=for-the-badge" />
</p>

</div>

---

## 📱 About

This project was built as part of the **ZenvyroLabs App Development
Internship** — a hands-on exercise in Flutter widgets, layout design, and
clean UI practices. It renders a Student Profile Screen with a profile
picture, personal/academic details, an "About Me" section, and an edit
action, all built from core Flutter widgets (no external UI kits).

<!--
  📸 Add a screenshot of the running app here once you have one:
  ![App Screenshot](assets/images/screenshot.png)
-->

## ✨ Features

- 🖼️ Circular profile picture (`CircleAvatar`)
- 🪪 Full name, university, department, and semester display
- 📧 Email and phone contact info with icons
- 📝 "About Me" bio section
- ✏️ "Edit Profile" action button
- 📐 Clean spacing, alignment, and card-based layout
- 📱 Responsive, scrollable single-screen design

## 🛠️ Built With

| Widget | Purpose |
|---|---|
| `MaterialApp` / `Scaffold` | App shell and screen structure |
| `AppBar` | Top title bar |
| `Column` / `Row` | Layout arrangement |
| `Container` | Cards, spacing, decoration |
| `CircleAvatar` | Profile picture |
| `Text` / `Icon` | Content and visual cues |
| `ElevatedButton` | Edit Profile action |
| `Padding` / `SizedBox` | Spacing and alignment |

## 🚀 Getting Started

### Prerequisites
- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- [Android Studio](https://developer.android.com/studio) with the Flutter
  and Dart plugins installed

### Run it locally

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
flutter pub get
flutter run
```

Or open the project folder directly in Android Studio, let Gradle sync
finish, pick a device/emulator, and hit ▶️ Run.

## 📂 Project Structure

```
student_profile_app/
├── android/              # Android platform project
├── assets/images/        # Local image assets (profile picture, etc.)
├── lib/
│   └── main.dart         # Student Profile Screen UI
├── pubspec.yaml           # Dependencies & asset config
└── README.md
```

## 🖊️ Customize

All profile info (name, university, department, contact details, bio) is
defined directly in `lib/main.dart` — update the values there to make it
your own. To swap the profile photo for a local image, see the
`assets:` section in `pubspec.yaml` and the `CircleAvatar` widget in
`main.dart`.

## 👤 Author

**Muhammad Abdullah Abrar**

📧 [mabdullahabrar21@gmail.com](mailto:mabdullahabrar21@gmail.com)

<p>
  <a href="mailto:mabdullahabrar21@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

## 📄 License

This project was created for educational purposes as part of an
internship task. Feel free to fork and build on it.

---

<div align="center">
Made with 💙 and Flutter
</div>
