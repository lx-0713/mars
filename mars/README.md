#### 查看本机已经安装的 NDK 版本
```
ls ~/Library/Android/sdk/ndk
```

#### 设置 NDK 环境变量
```
export NDK_ROOT="$HOME/Library/Android/sdk/ndk/20.1.5948944"
export ANDROID_NDK_HOME="$NDK_ROOT"
export PATH="$NDK_ROOT:$PATH"
```

#### 清理 xlog 编译缓存
```
rm -rf cmake_build/Android
rm -rf libraries/mars_android_sdk/libs
rm -rf libraries/mars_android_sdk/obj
rm -rf libraries/mars_xlog_sdk/libs
rm -rf libraries/mars_xlog_sdk/obj
```

### 编译 xlog 
```
python build_android.py 
然后选择 3
```