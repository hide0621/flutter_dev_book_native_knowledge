# chapter11_2_2

iOSとAndroid用にスプラッシュ画面を自動生成するには以下のパッケージが必要

`flutter pub add flutter_native_splash`

上記のパッケージを導入して`pub get`しつつ、

`pubspec.yaml`に

`flutter_native_splash:  
  color: "#00FFFF" # スプラッシュ画面の背景色  
  image: icon.png # スプラッシュ画面の中央に表示する画像  
  android_12: # Android 12以上の標準スプラッシュ画面の設定    
    color: "#FF00FF"  
  android_gravity: left # Androidのアイコンの画像の位置  
  ios_content_mode: left # iOSのアイコンの画像の位置`

上記の記述をして（[詳しくはこのコミットを参照](https://github.com/hide0621/flutter_dev_book_native_knowledge/commit/8510f20d6e9443837e9572b7678b907c278c59ea)）、かつプロジェクトのrootにpngファイルを用意した後で、

`dart run flutter_native_splash:create`

このコマンドを実行して自動生成する

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
