# chapter11_2_1

**flutter_launcher_icons**の導入

`flutter pub add --dev flutter_launcher_icons`

その後、iOSとAndroid用のアプリアイコンのpngファイルを用意して

pubspec.yamlに

`flutter_launcher_icons:
  image_path: "icon.png" # アイコン画像のパス
  ios: true # iOSのアイコンを生成し、デフォルトのものと置き換えるか
  android: true # Androidのアイコンを生成し、デフォルトのものと置き換えるか`

上記の記述をしたら、

`flutter pub run flutter_launcher_icons`

上記コマンドを実行して、Flutterアプリのデフォルトのアプリアイコンを用意したアイコンに変更する

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
