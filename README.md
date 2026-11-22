# 弧光乒乓 · 俱乐部物语（Android）

把单文件网页游戏包装成 Android WebView 应用，通过 GitHub Actions 云端构建 APK。

## 下载

https://github.com/lvjunrui/arc-pingpong/releases/latest/download/ArcPingPong.apk

## 构建

推送到 `main` 或手动运行 `Build APK` workflow。仓库 secrets：

- `KEYSTORE_B64`：PKCS12 签名密钥的 base64
- `KEYSTORE_PASSWORD`：密钥密码
- `KEY_ALIAS`：密钥别名

没有密钥时会退回调试签名构建。

## 工程

- `app/src/main/assets/index.html`：完整游戏（离线）
- `app/src/main/java/.../MainActivity.java`：WebView 壳
- 包名：`com.lvjunrui.arcpingpong`
- 目标 SDK 34，最低 SDK 23，竖屏
