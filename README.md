# codemagic_sample

Codemagicの運用テスト

## release.jks の 設定

```
codemagic_sample % keytool -genkey -v -keystore android/release.jks \
-storepass codemagic -alias androidreleasekey -keypass codemagic \
-keyalg RSA -keysize 2048 -validity 10000

姓名は何ですか。
[Unknown]:  Yuya Yamamura

組織単位名は何ですか。
[Unknown]:  CO

組織名は何ですか。
[Unknown]:  BestRise

都市名または地域名は何ですか。
[Unknown]:  Shibuya

都道府県名または州名は何ですか。
[Unknown]:  Tokyo

この単位に該当する2文字の国コードは何ですか。
[Unknown]:  JP

CN=Yuya Yamamura, OU=CO, O=BestRise, L=Shibuya, ST=Tokyo, C=JPでよろしいですか。

[いいえ]:  y

10,000日間有効な2,048ビットのRSAのキー・ペアと自己署名型証明書(SHA256withRSA)を生成しています
ディレクトリ名: CN=Yuya Yamamura, OU=CO, O=BestRise, L=Shibuya, ST=Tokyo, C=JP
[android/release.jksを格納中]
```