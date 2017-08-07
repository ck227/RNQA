# RNQA

## 记录项目开发中碰到的问题

Q：Command failed: /usr/libexec/PlistBuddy -c Print:CFBundleIdentifier build/Build/Products/Debug-iphonesimulator/QuHeart.app/Info.plist
Print: Entry, ":CFBundleIdentifier", Does Not Exist

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
尝试了使用低版本创建应用，配置了xcode,下载rncahce手动放入.rncache目录，尝试了升级xcode到8.3版本，升级了mac系统，还是不行。。。。
7.使用create_react-native-app 命令创建，进入项目目录运行yarn start，yarn run ios ，可以运行，启动模拟器卡住，放弃了。

在xcode上运行出来后没有这个问题了，版本0.46.1
```

Q：怎么在自己的设备上调试RN项目
```
还不能直接运行，装了Expo客户端，以后再说
npm update --global yarn 升级yarn
yarn代替npm install命令，用yarn add 某第三方库名代替npm install --save 某第三方库名

在xcode上运行出来后什么问题都没有，需要设置下项目的签名就可以，搞这么久，我是猪啊
```
Q：Attempt to register RCTBridgeModule class for the name 'SplashScreen',but name was already registered by class RCTSplashScreen
```
no answer yet
```
Q：添加导航器
`````
yarn add react-navigation
``````


