# Flutter Internals: Todo Demo

A Flutter learning project demonstrating widget rebuilds and list ordering with a small set of sample todos.

## Features

- Display three sample todos with priority icons.
- Toggle alphabetical ascending and descending order.
- Explore separate examples of local checkbox state and UI rebuilds in the source.

## Requirements

- Flutter with Dart `>=2.19.2 <3.0.0`, as declared in `pubspec.yaml`.
- A configured device, emulator, or supported browser target. Run `flutter doctor` to check your environment.

## Run locally

```sh
git clone https://github.com/Shefaa-atef/to_do_flutter_app.git
cd to_do_flutter_app/to_do_app
flutter pub get
flutter run
```

Use `flutter devices` to list targets and `flutter run -d <device-id>` to select one.

## Source guide

| Path inside the app | Purpose |
| --- | --- |
| `lib/main.dart` | Launches the Flutter Internals screen. |
| `lib/keys/keys.dart` | Sample todos and sorting. |
| `lib/keys/todo_item.dart` | Todo row and priority icon. |
| `lib/keys/checkable_todo_item.dart` | Separate stateful checkbox example. |
| `lib/ui_updates_demo.dart` | Separate widget-rebuild example. |

## Development checks

Run from the directory containing `pubspec.yaml`:

```sh
flutter analyze
flutter test
```

The repository includes a test scaffold; these commands do not imply that the tests cover the app's current behavior.

## Current behavior and limitations

Use a Flutter SDK whose bundled Dart version matches the declared range. The current manifest excludes Dart 3.

The active screen uses the non-checkable `TodoItem` widget. Creating, editing, and saving tasks are not implemented. The package name is `flutter_internals`, which explains the imports in the source.
