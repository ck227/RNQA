# RNQA

## 记录项目开发中碰到的问题

#### `Q：Command failed: /usr/libexec/PlistBuddy -c Print:CFBundleIdentifier build/Build/Products/Debug-iphonesimulator/QuHeart.app/Info.plist`
#### `Print: Entry, ":CFBundleIdentifier", Does Not Exist`
```
1.尝试降级react-native 到0.44失败，项目不能运行了，删除项目
2.升级react-native 到0.46，github项目clone下来运行npm install失败
3.在项目目录运行npm cache clean --force，运行npm install 成功
4.运行之后卡住
Building using "xcodebuild -project QuHeart.xcodeproj -configuration Debug -scheme QuHeart -destination id=E7AB60E1-0330-4224-8299-B2E8865CF533 -derivedDataPath build"
User defaults from command line:
IDEDerivedDataPathOverride = /Users/cnbs5/RNProject/QuHeart/ios/build

使用xcode打开项目后可以运行，提示Print: Entry, ":CFBundleIdentifier", Does Not Exist
5.命令行升级react-native版本，没有什么卵用   react-native-git-upgrade

6.react-native init ProjectName --version 0.44.2
使用低版本创建应用，还是不行
```

