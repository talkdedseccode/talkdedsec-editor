# Üçüncü Taraf Bildirimleri / Third-Party Notices

Bu belge yasal bir bildirimdir; pazarlama metni değildir. Talkdedsec Editor bir **çatallamadır (fork)**
ve üçüncü taraf bileşenlerle birlikte dağıtılır. Aşağıdaki telif ve lisans metinleri, ilgili lisansların
gerektirdiği şekilde burada yer alır.

This document is a legal notice, not marketing copy. Talkdedsec Editor is a **fork** and is distributed
together with third-party components. The copyright and license texts below are reproduced here as
required by the respective licenses.

---

## 1. Üst proje / Upstream project — Visual Studio Code

**TR.** Talkdedsec Editor, Microsoft Corporation tarafından geliştirilen **Visual Studio Code**
projesinin MIT lisanslı kaynak deposundan (<https://github.com/microsoft/vscode>) çatallanmıştır.
Yapı, Microsoft'un kendi markalı dağıtımından değil, MIT lisanslı kaynaktan üretilir; Microsoft'un
markalı sürümüne uygulanan ayrı lisans koşulları bu ürün için geçerli değildir.

Ürün yeniden adlandırılmıştır. "Visual Studio Code", "Visual Studio", "Microsoft" adları ve logoları
Microsoft Corporation'ın markalarıdır ve bu üründe marka olarak kullanılmaz. Bu ürün Microsoft
tarafından üretilmemiş, onaylanmamış veya desteklenmemektedir. Bu bölümdeki atıf, MIT lisansının telif
bildirimini koruma yükümlülüğünü yerine getirmek içindir.

**EN.** Talkdedsec Editor is a fork of **Visual Studio Code** by Microsoft Corporation, taken from its
MIT-licensed source repository (<https://github.com/microsoft/vscode>). Builds are produced from that
MIT-licensed source, not from Microsoft's branded distribution; the separate license terms that apply to
Microsoft's branded builds do not apply to this product.

The product has been renamed. "Visual Studio Code", "Visual Studio" and "Microsoft", and their logos,
are trademarks of Microsoft Corporation and are not used as branding in this product. This product is
not produced, endorsed or supported by Microsoft. The attribution in this section exists to satisfy the
MIT license requirement to retain the original copyright notice.

```
MIT License

Copyright (c) 2015 - present Microsoft Corporation

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 2. Çalışma zamanı bileşenleri / Runtime components

**TR.** Masaüstü yapısı, üst projeden devralınan çalışma zamanı bileşenlerini içerir. Başlıcaları:

**EN.** The desktop build includes runtime components inherited from the upstream project, principally:

| Bileşen / Component | Lisans / License | Telif / Copyright |
| --- | --- | --- |
| Electron | MIT | Copyright (c) Electron contributors; Copyright (c) 2013-2020 GitHub Inc. |
| Node.js | MIT | Copyright Node.js contributors. All rights reserved. |
| Chromium | BSD 3-Clause ve diğerleri / and others | Copyright 2015 The Chromium Authors. All rights reserved. |

**TR.** Chromium, kendi içinde çok sayıda farklı lisansa tabi bileşen barındırır. Bu bileşenlerin tam
listesi ve lisans metinleri, kurulu üründe `LICENSES.chromium.html` dosyasında bulunur.

**EN.** Chromium itself bundles a large number of components under various licenses. The complete list
and license texts are available in the installed product as `LICENSES.chromium.html`.

---

## 3. Yerleşik eklentiler ve bağımlılıklar / Built-in extensions and dependencies

**TR.** Ürünle birlikte 64 yerleşik eklenti ve bunların npm bağımlılıkları dağıtılır. Her biri kendi
lisansı altındadır; bunların çoğu MIT'tir, ancak tamamı değildir. Kurulu üründe dağıtılan tam liste
`ThirdPartyNotices.txt` dosyasındadır ve bu belgeye göre önceliklidir.

**EN.** 64 built-in extensions and their npm dependencies are distributed with the product. Each is under
its own license; most are MIT, but not all. The complete list shipped with the installed product is in
`ThirdPartyNotices.txt`, which takes precedence over this document.

---

## 4. Kapsam dışı / Not covered here

**TR.**

- **Open VSX eklentileri.** Eklenti mağazası olarak Open VSX Registry (Eclipse Foundation tarafından
  işletilir) kullanılır. Oradan kurduğunuz eklentiler bu ürünle birlikte dağıtılmaz; her biri kendi
  yayıncısının lisansına tabidir ve bu bildirimin kapsamı dışındadır.
- **Gömülü ajan (Claude).** Ajan, Anthropic'in istemci yazılımı üzerinden kendi aboneliğinizle çalışır.
  Kullanımı Anthropic'in kendi koşullarına tabidir; söz konusu servis bu ürünün lisansı kapsamında
  sunulmaz.
- **Yazı tipleri ve ikonlar.** Üst projeden devralınan görsel varlıklar kendi lisanslarını korur;
  Microsoft markalı logo ve ikonlar çatallamada kullanılmaz.

**EN.**

- **Open VSX extensions.** The extension marketplace is the Open VSX Registry (operated by the Eclipse
  Foundation). Extensions you install from it are not distributed with this product; each is licensed by
  its own publisher and falls outside the scope of this notice.
- **Embedded agent (Claude).** The agent runs on your own subscription through Anthropic's client
  software. Its use is subject to Anthropic's own terms; that service is not provided under this
  product's license.
- **Fonts and icons.** Visual assets inherited from the upstream project retain their own licenses;
  Microsoft-branded logos and icons are not used in the fork.

---

## 5. Eksik veya hatalı atıf / Missing or incorrect attribution

**TR.** Bu listede eksik bıraktığımız ya da yanlış belirttiğimiz bir bileşen olduğunu düşünüyorsanız
bir issue açın; düzeltiriz. Lisans uyumu bizim için isteğe bağlı değildir.

**EN.** If you believe a component is missing from this list or attributed incorrectly, open an issue and
we will correct it. License compliance is not optional for us.
