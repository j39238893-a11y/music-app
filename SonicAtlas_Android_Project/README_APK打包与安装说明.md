# SonicAtlas · 音乐流派与大师百科 (Spotify 风格 Android APK 工程)

本项目包含完整的 Android 原生包装工程（Kotlin + 硬件加速 WebView + 内置合成器音频引擎），支持以下三种方式在安卓手机上安装运行：

## 方式一：本地 Android Studio 一键生成 APK
1. 解压本压缩包，使用 **Android Studio (Hedgehog 或更新版本)** 打开工程目录。
2. 等待 Gradle 同步完成后，点击顶部菜单 **Build → Build Bundle(s) / APK(s) → Build APK(s)**。
3. 编译生成的安装包位于：`app/build/outputs/apk/debug/app-debug.apk`，发送至手机即可安装。

## 方式二：GitHub Actions 云端免配置自动编译 APK（无需本地安装 Android Studio）
1. 在 GitHub 新建一个仓库，将解压后的全部文件上传至仓库。
2. 点击仓库顶部的 **Actions** 标签页，内置的 `.github/workflows/build_apk.yml` 会自动运行云端编译。
3. 编译完成后，在 Actions 页面底部 **Artifacts** 区域点击 `SonicAtlas-Spotify-Style-APK` 即可直接下载编译好的 `.apk` 安装包。

## 方式三：手机浏览器直接安装到桌面 (WebAPK)
1. 直接将 `app/src/main/assets/index.html`（或在线预览版 HTML 文件）发送到安卓手机。
2. 用 Chrome 或 Edge 打开后，点击右上角菜单选择 **“添加到主屏幕”**，即可获得全屏沉浸式桌面应用体验。
