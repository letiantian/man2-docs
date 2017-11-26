## 通过ADB命令获取当前 activity
```plain
adb shell dumpsys activity activities | sed -En -e '/Running activities/,/Run #0/p'
```

## 当前设备列表
```plain
adb devices
```

## 进入shell环境
```plain
adb shell
```

## 安装apk
```plain
adb install <path to apk>
```

```plain
adb -s <device id> install <path to apk>
```

## 打印日志
```plain
adb logcat
```

## 打印指定APP的日志
如APP包名是`com.example.demo`：
```plain
adb logcat | grep "com.example.demo"
```