<div align="center">

# html-2-apk

**The simplest method for converting your HTML app into a working Android app.**

</div>

---

## 📖 Overview

Lots of frontend engineers want to convert their HTML app into an Android app, but most existing methods are too troublesome — some even require purchasing software.

With this method, you do **not** need to install:

- ❌ JDK
- ❌ Android SDK
- ❌ Eclipse, Android Studio, or PhoneGap
- ❌ Any paid software

Best of all, it's quick and simple — you can complete the whole process in **10 minutes**. Let's begin.

---

## 🛠️ Tool

The only tool you need is **AIDE**, installed on your mobile phone.

1. Open your mobile app store
2. Search for **"AIDE"**
3. Install it

![Install AIDE](https://github.com/ymrdf/html-2-apk/raw/master/pic/02.png)

---

## 🆕 Create a New App

**1. Open AIDE**

![Open AIDE](https://github.com/ymrdf/html-2-apk/raw/master/pic/03.png)

**2. Tap "For Experts"**

![For Experts](https://github.com/ymrdf/html-2-apk/raw/master/pic/04.png)

**3. Tap "New Android App"**

![New Android App](https://github.com/ymrdf/html-2-apk/raw/master/pic/05.png)

**4. Tap "CREATE"**

![Create](https://github.com/ymrdf/html-2-apk/raw/master/pic/06.png)

You've now created a new Android project. Its home directory is:

```
/AppProjects/MyApp
```

on your phone.

---

## ✏️ Modify Files

**1. Clone this repository** to your computer or download it directly to your phone:

```bash
git clone https://github.com/ymrdf/html-2-apk
```

**2. Replace the manifest**

Open `/AppProjects/MyApp/app/src/main` in your file browser and replace `AndroidManifest.xml` with the file of the same name from this repo.

**3. Replace the main activity**

Replace:
```
/AppProjects/MyApp/app/src/main/java/com/mycompany/myapp/MainActivity.java
```

**4. Replace the layout**

Replace:
```
/AppProjects/MyApp/app/src/main/res/layout/main.xml
```

**5. Copy in your web app**

Copy the `assets` folder into:
```
/AppProjects/MyApp/app/src/main
```

A sample HTML app is included at `assets/www` — replace it with your own.

> **⚠️ Note:** Your entry file **must** be named `index.html`.

---

## ▶️ Test

Now you can see the result.

**1. Back in AIDE, tap the ▶ (run) button**

![Run](https://github.com/ymrdf/html-2-apk/raw/master/pic/07.png)

**2. Tap "Install"**

You should see a new app installed on your device:

![Installed app](https://github.com/ymrdf/html-2-apk/raw/master/pic/13.png)

🎉 You've successfully converted your HTML app to an Android app and installed it on your device.

Your `.apk` file is located at:
```
/AppProjects/MyApp/app/build/bin/
```

---

## 📦 Building the APK for Release

It's time to deploy your Android app and get it into your users' hands.

**1. Back in AIDE, tap the Menu button**

![Menu](https://github.com/ymrdf/html-2-apk/raw/master/pic/09.png)

**2. Tap "Project"**

![Project](https://github.com/ymrdf/html-2-apk/raw/master/pic/14.png)

**3. Tap "Publish Project"**

![Publish project](https://github.com/ymrdf/html-2-apk/raw/master/pic/15.png)

Follow the prompts to generate a signed, release-ready APK.
