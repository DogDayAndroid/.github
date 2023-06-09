<div align = center>

<img src="https://avatars.githubusercontent.com/u/100076963?s=400&u=7aa8fe633f7b7c185c9400ed1a5cc925cb514f22&v=4" width="200" height="175" alt="banner">

<h1>DogDay 🌭 热狗</h1>

![License](https://img.shields.io/static/v1?label=License&message=BY-NC-SA&logo=creativecommons&color=green)
![Language](https://img.shields.io/github/languages/top/DogDayAndroid/Android-Kernel-Builder)
![Issues](https://img.shields.io/github/issues/DogDayAndroid/Android-Kernel-Builder)
![Pull Requests](https://img.shields.io/github/issues-pr/DogDayAndroid/Android-Kernel-Builder)
<br>

这里应该是一段项目介绍……
<br>

---

**[<kbd> <br>  Configure  <br> </kbd>](#configuration-file-syntax)** 
**[<kbd> <br>  Quick Start  <br> </kbd>](#how-to-use)** 
**[<kbd> <br>  Local testing  <br> </kbd>](#local-testing)**

---
</div>

## 如何自定义首次启动的引导界面

### 测试原版的 SetupWizard

首先我们需要进入 `adb` 环境，在终端执行如下指令:

```
adb shell
```

进入到手机的 `adb` 环境后，首先利用 `su` 进行提权，随后启动原生的引导界面程序即可，具体指令如下:

```
su
am start -n com.google.android.setupwizard/.SetupWizardTestActivity
```
