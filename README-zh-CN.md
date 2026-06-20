<div align="center">

# html-2-apk

**将你的 HTML 应用转换为可运行的 Android 应用的最简单方法。**

</div>

---

## 📖 概述

很多前端工程师都想把自己的 HTML 应用转换成 Android 应用，但现有的方法大多过于繁琐，有些甚至需要购买软件。

使用这种方法，你**不需要**安装：

- ❌ JDK
- ❌ Android SDK
- ❌ Eclipse、Android Studio 或 PhoneGap
- ❌ 任何付费软件

最重要的是，整个过程简单快捷——你可以在 **10 分钟**内完成。现在，让我们开始吧。

---

## 🛠️ 工具

你唯一需要的工具是手机上安装的 **AIDE**。

1. 打开手机应用商店
2. 搜索 **"AIDE"**
3. 安装它

![安装 AIDE](https://github.com/ymrdf/html-2-apk/raw/master/pic/02.png)

---

## 🆕 创建新应用

**1. 打开 AIDE**

![打开 AIDE](https://github.com/ymrdf/html-2-apk/raw/master/pic/03.png)

**2. 点击 "For Experts"**

![For Experts](https://github.com/ymrdf/html-2-apk/raw/master/pic/04.png)

**3. 点击 "New Android App"**

![New Android App](https://github.com/ymrdf/html-2-apk/raw/master/pic/05.png)

**4. 点击 "CREATE"**

![Create](https://github.com/ymrdf/html-2-apk/raw/master/pic/06.png)

现在，你已经创建了一个新的 Android 项目。该项目的主目录位于你手机上的：

```
/AppProjects/MyApp
```

---

## ✏️ 修改文件

**1. 克隆本仓库**到你的电脑，或直接下载到手机上：

```bash
git clone https://github.com/ymrdf/html-2-apk
```

**2. 替换 manifest 文件**

在文件管理器中打开 `/AppProjects/MyApp/app/src/main`，用本仓库中同名的文件替换 `AndroidManifest.xml`。

**3. 替换主活动文件**

替换：
```
/AppProjects/MyApp/app/src/main/java/com/mycompany/myapp/MainActivity.java
```

**4. 替换布局文件**

替换：
```
/AppProjects/MyApp/app/src/main/res/layout/main.xml
```

**5. 复制你的网页应用**

将 `assets` 文件夹复制到：
```
/AppProjects/MyApp/app/src/main
```

仓库中 `assets/www` 目录下提供了一个示例 HTML 应用，你可以用自己的应用替换它。

> **⚠️ 注意：** 入口文件**必须**命名为 `index.html`。

---

## ▶️ 测试

现在你可以查看效果了。

**1. 回到 AIDE，点击 ▶（运行）按钮**

![运行](https://github.com/ymrdf/html-2-apk/raw/master/pic/07.png)

**2. 点击 "Install"（安装）**

你应该会在设备上看到一个新安装的应用：

![已安装的应用](https://github.com/ymrdf/html-2-apk/raw/master/pic/13.png)

🎉 你已经成功将 HTML 应用转换为 Android 应用，并安装到了你的设备上。

你的 `.apk` 文件位于：
```
/AppProjects/MyApp/app/build/bin/
```

---

## 📦 构建发布版 APK

现在该把你的 Android 应用部署出去，交到用户手中了。

**1. 回到 AIDE，点击菜单按钮**

![菜单](https://github.com/ymrdf/html-2-apk/raw/master/pic/09.png)

**2. 点击 "Project"（项目）**

![项目](https://github.com/ymrdf/html-2-apk/raw/master/pic/14.png)

**3. 点击 "Publish Project"（发布项目）**

![发布项目](https://github.com/ymrdf/html-2-apk/raw/master/pic/15.png)

按照提示操作，即可生成已签名、可供发布的 APK 文件。
