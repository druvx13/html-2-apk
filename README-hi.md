<div align="center">

# html-2-apk

**अपने HTML ऐप को एक वर्किंग एंड्रॉइड ऐप में बदलने का सबसे आसान तरीका।**

</div>

---

## 📖 परिचय

बहुत से फ्रंटएंड इंजीनियर अपने HTML ऐप को एंड्रॉइड ऐप में बदलना चाहते हैं, लेकिन ज़्यादातर मौजूदा तरीके बहुत झंझट वाले हैं — कुछ के लिए तो पेड सॉफ़्टवेयर खरीदना भी पड़ता है।

इस तरीके से आपको **इनमें से कुछ भी इंस्टॉल करने की ज़रूरत नहीं** है:

- ❌ JDK
- ❌ Android SDK
- ❌ Eclipse, Android Studio, या PhoneGap
- ❌ कोई भी पेड सॉफ़्टवेयर

सबसे अच्छी बात यह है कि यह तरीका बहुत सरल और तेज़ है — आप पूरी प्रक्रिया **10 मिनट** में पूरी कर सकते हैं। चलिए शुरू करते हैं।

---

## 🛠️ टूल

आपको सिर्फ़ एक टूल की ज़रूरत होगी: अपने मोबाइल फ़ोन में इंस्टॉल किया गया **AIDE**।

1. अपने मोबाइल का ऐप स्टोर खोलें
2. **"AIDE"** सर्च करें
3. उसे इंस्टॉल करें

![AIDE इंस्टॉल करें](https://github.com/ymrdf/html-2-apk/raw/master/pic/02.png)

---

## 🆕 नया ऐप बनाएं

**1. AIDE खोलें**

![AIDE खोलें](https://github.com/ymrdf/html-2-apk/raw/master/pic/03.png)

**2. "For Experts" पर टैप करें**

![For Experts](https://github.com/ymrdf/html-2-apk/raw/master/pic/04.png)

**3. "New Android App" पर टैप करें**

![New Android App](https://github.com/ymrdf/html-2-apk/raw/master/pic/05.png)

**4. "CREATE" पर टैप करें**

![Create](https://github.com/ymrdf/html-2-apk/raw/master/pic/06.png)

अब आपने एक नया एंड्रॉइड प्रोजेक्ट बना लिया है। इस प्रोजेक्ट की होम डायरेक्टरी आपके फ़ोन में यहाँ है:

```
/AppProjects/MyApp
```

---

## ✏️ फ़ाइलें बदलें

**1. इस रिपॉज़िटरी को क्लोन करें** अपने कंप्यूटर पर, या सीधे फ़ोन में डाउनलोड करें:

```bash
git clone https://github.com/ymrdf/html-2-apk
```

**2. मैनिफ़ेस्ट फ़ाइल बदलें**

अपने फ़ाइल ब्राउज़र में `/AppProjects/MyApp/app/src/main` खोलें, और `AndroidManifest.xml` को रिपॉज़िटरी की उसी नाम वाली फ़ाइल से बदल दें।

**3. मेन ऐक्टिविटी फ़ाइल बदलें**

बदलें:
```
/AppProjects/MyApp/app/src/main/java/com/mycompany/myapp/MainActivity.java
```

**4. लेआउट फ़ाइल बदलें**

बदलें:
```
/AppProjects/MyApp/app/src/main/res/layout/main.xml
```

**5. अपना वेब ऐप कॉपी करें**

`assets` फ़ोल्डर को यहाँ कॉपी करें:
```
/AppProjects/MyApp/app/src/main
```

रिपॉज़िटरी के `assets/www` में एक सैंपल HTML ऐप दिया गया है — आप इसे अपने ऐप से बदल सकते हैं।

> **⚠️ ध्यान दें:** एंट्री फ़ाइल का नाम **ज़रूर** `index.html` होना चाहिए।

---

## ▶️ टेस्ट करें

अब आप नतीजा देख सकते हैं।

**1. वापस AIDE में जाएं और ▶ (रन) बटन पर टैप करें**

![रन करें](https://github.com/ymrdf/html-2-apk/raw/master/pic/07.png)

**2. "Install" पर टैप करें**

आपको अपने डिवाइस में एक नया इंस्टॉल हुआ ऐप दिखेगा:

![इंस्टॉल हुआ ऐप](https://github.com/ymrdf/html-2-apk/raw/master/pic/13.png)

🎉 बधाई हो! आपने अपने HTML ऐप को एंड्रॉइड ऐप में सफलतापूर्वक बदल दिया है, और इसे अपने डिवाइस में इंस्टॉल भी कर लिया है।

आपकी `.apk` फ़ाइल यहाँ मिलेगी:
```
/AppProjects/MyApp/app/build/bin/
```

---

## 📦 रिलीज़ के लिए APK बनाएं

अब समय है अपने एंड्रॉइड ऐप को डिप्लॉय करने और उसे अपने यूज़र्स तक पहुँचाने का।

**1. वापस AIDE में जाएं, मेन्यू बटन पर टैप करें**

![मेन्यू](https://github.com/ymrdf/html-2-apk/raw/master/pic/09.png)

**2. "Project" पर टैप करें**

![प्रोजेक्ट](https://github.com/ymrdf/html-2-apk/raw/master/pic/14.png)

**3. "Publish Project" पर टैप करें**

![प्रोजेक्ट पब्लिश करें](https://github.com/ymrdf/html-2-apk/raw/master/pic/15.png)

निर्देशों का पालन करें, और आपको एक साइन की हुई, रिलीज़-रेडी APK फ़ाइल मिल जाएगी।
