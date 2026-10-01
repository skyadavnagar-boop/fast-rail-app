# fast-rail-app

Minimal Tatkal passenger autofill assistant with the Dart package name
`fast_rail_app`. Enter one passenger's name, age, and gender, then open
IRCTC in the embedded WebView. The lightning button attempts to fill matching
passenger fields and select the confirm-berths checkbox; review all details
on IRCTC before continuing. The WebView's network-image blocking setting is
supported on Android.

## Run

Install the [Flutter SDK](https://docs.flutter.dev/get-started/install)
(Dart 3.8 or newer), then:

```sh
cd fast-rail-app
flutter pub get
flutter run
```

Select a connected device or emulator when prompted. For the web version:

```sh
flutter run -d chrome
```

Use `flutter doctor` to check platform setup. Android requires the Android
SDK; iOS requires macOS and Xcode.

## Structure

- `lib/main.dart` — passenger form, IRCTC WebView, and autofill action
- `test/widget_test.dart` — passenger form widget test
- `pubspec.yaml` — package metadata and dependencies
- `android/`, `ios/`, `web/` — standard generated platform projects

The native identifiers use Flutter's default `com.example` organization
with `fast_rail_app`; choose your own organization before publishing.