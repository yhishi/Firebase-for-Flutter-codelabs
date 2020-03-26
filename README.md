# firebase-for-flutter-codelabs

codelab Firebase for Flutter
https://codelabs.developers.google.com/codelabs/flutter-firebase

## 学んだ内容
* FlutterアプリにFirebase機能を追加する方法
* Firestoreを使って、リアルタイムにデータを読み取り＆更新
* Firestoreデータベースをアトミックに更新する方法

## ハマった点
* iOSプロジェクトのRunnerサブディレクトリ配下にGoogleService-Info.plistを配置しても認識せず、以下のエラー
```
The file “GoogleService-Info.plist” couldn’t be opened because there is no such file.
```

Xcodeを起動し、
```
open ios/Runner.xcworkspace
```

GoogleService-Info.plistファイルを一度削除＆再配置すると、認識した。
参考：https://stackoverflow.com/a/59830697