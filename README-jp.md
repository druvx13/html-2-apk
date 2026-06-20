<div align="center">

# html-2-apk

**HTMLアプリを実際に動作するAndroidアプリへ変換する、最も簡単な方法。**

</div>

---

## 📖 概要

多くのフロントエンドエンジニアが自分のHTMLアプリをAndroidアプリに変換したいと考えていますが、既存の方法の多くは手間がかかりすぎたり、有料ソフトウェアの購入が必要だったりします。

この方法では、以下のものは**一切不要**です。

- ❌ JDK
- ❌ Android SDK
- ❌ Eclipse、Android Studio、PhoneGap
- ❌ 有料ソフトウェア

何より、シンプルかつ簡単で、**10分**で完了します。さっそく始めましょう。

---

## 🛠️ 必要なツール

必要なツールは、スマートフォンにインストールする **AIDE** だけです。

1. スマートフォンのアプリストアを開く
2. **「AIDE」** を検索する
3. インストールする

![AIDEをインストール](https://github.com/ymrdf/html-2-apk/raw/master/pic/02.png)

---

## 🆕 新規アプリの作成

**1. AIDEを開く**

![AIDEを開く](https://github.com/ymrdf/html-2-apk/raw/master/pic/03.png)

**2. 「For Experts」をタップ**

![For Experts](https://github.com/ymrdf/html-2-apk/raw/master/pic/04.png)

**3. 「New Android App」をタップ**

![New Android App](https://github.com/ymrdf/html-2-apk/raw/master/pic/05.png)

**4. 「CREATE」をタップ**

![Create](https://github.com/ymrdf/html-2-apk/raw/master/pic/06.png)

これで新しいAndroidプロジェクトが作成されました。プロジェクトのホームディレクトリは、スマートフォン内の以下の場所にあります。

```
/AppProjects/MyApp
```

---

## ✏️ ファイルの編集

**1. このリポジトリをクローン**します（パソコンでも、スマートフォンに直接ダウンロードしても構いません）。

```bash
git clone https://github.com/ymrdf/html-2-apk
```

**2. マニフェストファイルを置き換える**

ファイラーで `/AppProjects/MyApp/app/src/main` を開き、`AndroidManifest.xml` をダウンロードした同名のファイルに置き換えます。

**3. メインアクティビティファイルを置き換える**

次のファイルを置き換えます。
```
/AppProjects/MyApp/app/src/main/java/com/mycompany/myapp/MainActivity.java
```

**4. レイアウトファイルを置き換える**

次のファイルを置き換えます。
```
/AppProjects/MyApp/app/src/main/res/layout/main.xml
```

**5. Webアプリをコピーする**

`assets` フォルダを以下の場所にコピーします。
```
/AppProjects/MyApp/app/src/main
```

リポジトリの `assets/www` にサンプルのHTMLアプリが入っているので、そこを自分のアプリに置き換えてください。

> **⚠️ 注意：** エントリーファイルの名前は**必ず** `index.html` にしてください。

---

## ▶️ テスト

ここまでで、実際の動作を確認できます。

**1. AIDEに戻り、▶（実行）ボタンをタップ**

![実行](https://github.com/ymrdf/html-2-apk/raw/master/pic/07.png)

**2. 「Install」をタップ**

デバイス上に新しいアプリがインストールされているはずです。

![インストールされたアプリ](https://github.com/ymrdf/html-2-apk/raw/master/pic/13.png)

🎉 これでHTMLアプリをAndroidアプリへの変換し、デバイスへのインストールが完了しました。

`.apk` ファイルは以下の場所にあります。
```
/AppProjects/MyApp/app/build/bin/
```

---

## 📦 リリース用APKのビルド

いよいよAndroidアプリをデプロイし、ユーザーの手元に届ける段階です。

**1. AIDEに戻り、メニューボタンをタップ**

![メニュー](https://github.com/ymrdf/html-2-apk/raw/master/pic/09.png)

**2. 「Project」をタップ**

![プロジェクト](https://github.com/ymrdf/html-2-apk/raw/master/pic/14.png)

**3. 「Publish Project」をタップ**

![プロジェクトを公開](https://github.com/ymrdf/html-2-apk/raw/master/pic/15.png)

画面の指示に従えば、署名済みのリリース用APKが生成されます。
