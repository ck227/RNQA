# RNQA

## 记录项目开发中碰到的问题

#### Q：Command failed: /usr/libexec/PlistBuddy -c Print:CFBundleIdentifier build/Build/Products/Debug-iphonesimulator/QuHeart.app/Info.plist
#### Print: Entry, ":CFBundleIdentifier", Does Not Exist

```
1.尝试降级react-native 到0.44失败，项目不能运行了
2.升级react-native 到0.46，github项目clone下来运行npm install失败
3.在项目目录运行npm cache clean --force，运行npm install 成功
```

