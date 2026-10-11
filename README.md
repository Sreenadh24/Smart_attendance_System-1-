# Smart Attendance System

A Flutter and Dart attendance-management demonstration for college projects.
It uses Material Design 3, seeded local sample data, and in-memory state only.
It does not connect to a backend or Firebase, and it does not collect biometric
data or authenticate real students.

## Features

- Demo sign-in as Admin / Teacher or as one of the sample students.
- Admin overview, student management, attendance marking, searchable attendance
  records, and a sample report with a present-versus-absent chart.
- Student dashboard with attendance percentage, attended/missed class counts,
  and recent records.
- Ten preloaded students and six sample class days; changes made during the
  session remain in memory until the app is closed.
- A visible notice that all data is for demonstration only.

## Requirements

- Flutter SDK and Dart SDK supported by the `environment` entry in
  `pubspec.yaml`.
- Android Studio with an Android emulator, or a USB-connected Android device
  with developer options and USB debugging enabled.

## Dependencies

The app's direct package dependencies are:

- `provider: ^6.1.5+1` — in-app state management.
- `intl: ^0.20.3` — date formatting.
- Flutter SDK's Material and widget libraries.

## Run from a terminal

From this project directory (`smart_attendance_system`):

```sh
flutter pub get
flutter devices
flutter run
```

Start an Android emulator before running `flutter run`, or connect an Android
device. No internet connection is needed after Flutter has resolved the
dependencies.

## Run from VS Code

1. Open the `smart_attendance_system` folder in VS Code and install the Flutter
   and Dart extensions.
2. Start an Android emulator or connect a configured Android device.
3. Run `Flutter: Get Packages` from the Command Palette.
4. Select the device in the status bar and press **F5** (or use **Run > Start
   Debugging**).

## Run from Android Studio

1. Open the `smart_attendance_system` folder as a Flutter project.
2. Wait for package resolution, or run `flutter pub get` in the terminal.
3. Start an Android emulator or connect a configured Android device.
4. Select the device and run the `lib/main.dart` configuration.

On the login screen, choose **Admin / Teacher** to access the management
dashboard, or choose **Student** and select a sample student. There are no
passwords or real accounts. Attendance and roster edits are intentionally
session-only and reset when the app is restarted.