<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedsec-editor/main/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedsec-editor/main/assets/banner-light.svg" width="100%" alt="Talkdedsec editor — boots in 0.41 s, 9 processes, 64 extensions, 0 telemetry, 0 source maps.">
</picture>

<p align="center">
  <a href="https://code.talkdedsec.com"><b>code.talkdedsec.com</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/releases/latest"><b>download</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/discussions"><b>forum</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-themes"><b>themes</b></a>
</p>

<br>

## What this is

A code editor for Windows, built on an open-source editor core with the parts I never used taken out.

Telemetry didn't get a setting, it got removed from the source. There's no update server to point at,
because there isn't one. Thirty-four built-in extensions are gone. Nothing contacts a server when you
open it, which is another way of saying it behaves the same offline as online.

It installs into your user folder. It never asks for administrator rights, and it doesn't touch your
existing editor's settings — the two run side by side on the same project.

<br>

## Install

Download the installer from [Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest)
and run it. Windows SmartScreen will warn you the first time; the package isn't code-signed yet, so
choose **More info → Run anyway** if you're comfortable with that.

```
%LOCALAPPDATA%\Programs\Talkdedsec\Talkdedsec.exe
```

Settings, extensions and session history live in a `.talkdedsec` folder of their own. Extensions come
from [Open VSX](https://open-vsx.org). A few Marketplace-only ones — C#, Pylance, the Remote-* family —
aren't published there and won't be available.

There is no auto-update. When a new version ships, you download it and install over the top; your
settings survive.

<br>

## Themes

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedsec-editor/main/assets/themes-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedsec-editor/main/assets/themes-light.svg" width="100%" alt="Five built-in themes — Dark, Midnight, Matrix, Ember, Light — with their real backgrounds and terminal palettes">
</picture>

Five ship with the editor. Each one covers 183 color keys and a full 16-colour terminal palette, so
switching doesn't leave the panels, git marks and terminal looking like the theme you just left.

Switch with <kbd>Ctrl</kbd>+<kbd>K</kbd> then <kbd>Ctrl</kbd>+<kbd>T</kbd>. To make your own, run
**Generate Color Theme From Current Settings** from the command palette and
[send it to the themes repo](https://github.com/talkdedseccode/talkdedsec-themes) — a pull request is
all it takes, no account signup.

<br>

## The agent

An agent runs inside the editor core. Nothing to install, no second app to switch to. Press
<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>J</kbd> to open a session; agent sessions also get their own window.

You connect with your own account. There's no seat fee, no token markup and no service sitting in the
middle. That also means the requests go to your provider under your own terms, which is a thing you're
choosing to do rather than something the editor does behind your back.

<br>

## Where to go

| | |
|:---|:---|
| Something's broken | [Issues](https://github.com/talkdedseccode/talkdedsec-editor/issues) |
| A question | [Discussions → Q&A](https://github.com/talkdedseccode/talkdedsec-editor/discussions/categories/q-a) |
| A theme you made | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) |
| A security problem | [Security advisory](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new) — please don't open a public issue |

<br>

## License

The editor is closed source and ships under [terms of use](LICENSE): free for personal use, a license
key for commercial use, no redistribution.

It's built on an open-source editor core. That project's copyright notice and MIT license text are
reproduced in full in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md), along with everything else
bundled in the package.

<br>

<details>
<summary><b>Türkçe</b></summary>

<br>

### Nedir

Windows için bir kod editörü. Açık kaynak bir editör çekirdeği üzerine kuruldu; kullanmadığım parçalar
söküldü.

Telemetriye ayar konmadı, kaynaktan kaldırıldı. Gösterilecek bir güncelleme sunucusu yok, çünkü hiç yok.
Otuz dört yerleşik eklenti gitti. Açtığında hiçbir sunucuya bağlanmıyor; yani çevrimdışıyken de
çevrimiçiyken de aynı davranıyor.

Kullanıcı klasörüne kuruluyor. Yönetici hakkı istemiyor ve mevcut editörünün ayarlarına dokunmuyor —
ikisi aynı projede yan yana çalışıyor.

### Kurulum

Kurulum dosyasını [Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest)
sayfasından indir ve çalıştır. Windows SmartScreen ilk seferde uyarır; paket henüz imzalı olmadığı için
sakıncası yoksa **Daha fazla bilgi → Yine de çalıştır** de.

```
%LOCALAPPDATA%\Programs\Talkdedsec\Talkdedsec.exe
```

Ayarların, eklentilerin ve oturum geçmişin kendi `.talkdedsec` klasöründe duruyor. Eklentiler
[Open VSX](https://open-vsx.org) üzerinden geliyor. Yalnız Marketplace'te olan birkaçı — C#, Pylance,
Remote-* ailesi — orada yayınlanmadığı için bulunmayacak.

Otomatik güncelleme yok. Yeni sürüm çıkınca indirip üzerine kuruyorsun; ayarların duruyor.

### Temalar

Beş tema geliyor. Her biri 183 renk anahtarı ve tam 16 renklik terminal paleti kapsıyor; tema
değişince paneller, git işaretleri ve terminal az önce bıraktığın temada kalmıyor.

Değiştirmek için <kbd>Ctrl</kbd>+<kbd>K</kbd> ardından <kbd>Ctrl</kbd>+<kbd>T</kbd>. Kendi temanı
üretmek için komut paletinden **Generate Color Theme From Current Settings** çalıştır ve
[tema deposuna gönder](https://github.com/talkdedseccode/talkdedsec-themes) — bir pull request yetiyor,
hesap açman gerekmiyor.

### Ajan

Ajan editörün çekirdeğinde çalışıyor. Kurulacak bir şey, geçilecek ikinci bir uygulama yok.
<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>J</kbd> ile oturum açılıyor; ajan oturumlarının kendi penceresi de var.

Kendi hesabınla bağlanıyorsun. Koltuk ücreti, token payı ve araya giren bir servis yok. Bu aynı zamanda
isteklerin kendi şartlarınla kendi sağlayıcına gittiği anlamına geliyor — senin seçtiğin bir şey, editörün
arkandan yaptığı bir şey değil.

### Nereye gidilir

| | |
|:---|:---|
| Bir şey bozuk | [Issues](https://github.com/talkdedseccode/talkdedsec-editor/issues) |
| Soru | [Discussions → Q&A](https://github.com/talkdedseccode/talkdedsec-editor/discussions/categories/q-a) |
| Yazdığın tema | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) |
| Güvenlik açığı | [Güvenlik bildirimi](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new) — herkese açık issue açma |

### Lisans

Editör kapalı kaynak ve [kullanım şartlarıyla](LICENSE) dağıtılıyor: kişisel kullanım ücretsiz, ticari
kullanım lisans anahtarı istiyor, yeniden dağıtım yok.

Açık kaynak bir editör çekirdeği üzerine kurulu. O projenin telif bildirimi ve MIT lisans metni,
pakete giren diğer her şeyle birlikte [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) içinde tam
hâliyle duruyor.

</details>
