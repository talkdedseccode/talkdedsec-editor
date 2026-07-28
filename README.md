# Talkdedsec Editor

Windows için masaüstü kod editörü. Telemetri yok, hesap yok, arka planda çalışan servis yok.
Kurulum dosyası [Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest) üzerinden dağıtılır.

**[Site](https://code.talkdedsec.com)** · **[İndir](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest)** · **[Forum](https://github.com/talkdedseccode/talkdedsec-editor/discussions)** · **[Temalar](https://github.com/talkdedseccode/talkdedsec-themes)**

[English below ↓](#talkdedsec-editor-english)

---

## Nedir

Açık kaynak bir editör çekirdeğinin çatallanmasıdır. Değişen şey davranıştır: veri toplayan uç noktalar
kaldırıldı, ihtiyaç duyulmayan yerleşik eklentiler çıkarıldı, dağıtımdan source map'ler atıldı.
Editörün kendisi tanıdık kalır — aynı kısayollar, aynı eklenti biçimi, aynı ayar dosyası.

Üst projeye atıf ve lisans bilgisi için [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) dosyasına bakın.

## Ölçülen değerler

Sürüm 1.130.0, Windows x64. Rakamlar soğuk profille (eklenti yüklü değil, ayar geçmişi yok) ölçüldü.

| Ölçüm | Değer |
| --- | --- |
| Açılıştan kullanılabilir pencereye | 0,41 sn |
| Süreç sayısı | 9 |
| Boşta bellek kullanımı | 1,40 GB |
| Diskte kurulu boyut | 1,12 GB |
| Kurulum dosyası | 253 MB |
| Yerleşik eklenti | 64 (üst projede 98) |
| Telemetri uç noktası | 0 |
| Dağıtımdaki source map | 0 |
| Yerleşik tema | 5 |

Kendi makinenizde farklı sonuç alabilirsiniz; açılış süresi diske, boştaki bellek ise açık klasöre
ve yüklü eklentilere göre değişir.

## Kurulum

1. [Releases sayfasından](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest) `.exe` kurulum dosyasını indirin.
2. Çalıştırın. Kurulum **kullanıcı düzeyindedir** — yönetici hakkı istemez, `Program Files` altına yazmaz,
   sisteme servis veya sürücü kurmaz.
3. Kaldırmak için Windows "Uygulamalar ve özellikler" listesinden kaldırın.

Kurulum dosyası bu depodaki Releases dışında hiçbir yerde dağıtılmaz. Başka bir kaynaktan indirdiğiniz
dosya bizim yayınımız değildir.

## Gizlilik duruşu

| Konu | Durum |
| --- | --- |
| Kullanım/çökme telemetrisi | Gönderilmez — uç nokta bulunmaz |
| Hesap açma, oturum açma | Gerekmez |
| Arka plan güncelleme servisi | Kurulmaz |
| Deneysel özellik / uzaktan bayrak çekme | Yok |
| Eklenti mağazası | Open VSX |
| Gömülü ajan (Claude) | Yalnızca siz başlattığınızda, **kendi aboneliğinizle** çalışır |

Gömülü ajanı kullandığınızda istekler doğrudan sizin sağlayıcı hesabınız üzerinden gider; araya biz
girmeyiz, bir sunucumuzdan geçmez. Ajanı hiç kullanmazsanız editör tamamen çevrimdışı çalışır.

Güncellemeleri kendiniz alırsınız: yeni sürüm çıktığında Releases'te yayımlanır, editör kendi kendine
indirmeye çalışmaz. Sürüm bildirimi için depoyu **Watch → Releases only** ile izleyebilirsiniz.

## Temalar

5 tema yerleşik gelir. Her tema 183 renk anahtarı ve 16 renkli terminal paleti tanımlar — yani arayüzün
tamamı ve terminal, yarım kalmış bir tema gibi karışık görünmez.

Tema dosyaları standart biçimdedir:

```jsonc
{
  "name": "tema-adi",
  "type": "dark",
  "colors": {
    "editor.background": "#0b0d10",
    "editor.foreground": "#d7dae0",
    "terminal.ansiRed": "#e06c75"
  },
  "tokenColors": [
    { "scope": "comment", "settings": { "foreground": "#5c6370" } }
  ]
}
```

Kendi temanızı paylaşmak, mevcut bir temada renk düzeltmek veya yeni tema önermek için
**[talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes)** deposunu kullanın.
Tema ile ilgili issue'lar bu depoda değil, orada açılır.

## Forum ve destek

Sitedeki forum bu deponun **[Discussions](https://github.com/talkdedseccode/talkdedsec-editor/discussions)**
bölümünü okur. Yani buraya yazdığınız gönderi sitede de görünür.

| Ne | Nereye |
| --- | --- |
| Çöküyor, hatalı davranıyor | [Issues → Hata bildirimi](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=hata_bildirimi.yml) |
| Şu özellik olsun | [Issues → Özellik isteği](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=ozellik_istegi.yml) |
| Soru, kullanım, "nasıl yapılır" | [Discussions → Q&A](https://github.com/talkdedseccode/talkdedsec-editor/discussions/categories/q-a) |
| Güvenlik açığı | [SECURITY.md](SECURITY.md) — herkese açık issue açmayın |
| Tema | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) |

Katkı kuralları: [CONTRIBUTING.md](CONTRIBUTING.md) · Davranış kuralları: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## Lisans

MIT — [LICENSE](LICENSE). Üst projenin ve birlikte dağıtılan bileşenlerin lisansları
[THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) dosyasındadır.

---

<a id="talkdedsec-editor-english"></a>

# Talkdedsec Editor (English)

A desktop code editor for Windows. No telemetry, no account, no background service.
The installer is distributed through [Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest).

**[Website](https://code.talkdedsec.com)** · **[Download](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest)** · **[Forum](https://github.com/talkdedseccode/talkdedsec-editor/discussions)** · **[Themes](https://github.com/talkdedseccode/talkdedsec-themes)**

## What it is

A fork of an open-source editor core. What changed is behaviour: data-collecting endpoints were removed,
built-in extensions that were not needed were dropped, and source maps were excluded from the build.
The editor itself stays familiar — same shortcuts, same extension format, same settings file.

Upstream attribution and licensing: see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

## Measured numbers

Version 1.130.0, Windows x64. Measured on a cold profile (no extensions installed, no settings history).

| Measurement | Value |
| --- | --- |
| Launch to usable window | 0.41 s |
| Process count | 9 |
| Idle memory usage | 1.40 GB |
| Installed size on disk | 1.12 GB |
| Installer size | 253 MB |
| Built-in extensions | 64 (98 upstream) |
| Telemetry endpoints | 0 |
| Source maps shipped | 0 |
| Built-in themes | 5 |

Your machine may report different figures; launch time depends on the disk, and idle memory depends on
the folder you open and the extensions you install.

## Install

1. Download the `.exe` installer from [Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest).
2. Run it. The install is **user-level** — no administrator rights, nothing written to `Program Files`,
   no service or driver installed.
3. To remove it, uninstall from Windows "Apps & features".

The installer is not distributed anywhere except the Releases page of this repository. A file obtained
from any other source is not our build.

## Privacy stance

| Topic | Status |
| --- | --- |
| Usage / crash telemetry | Not sent — no endpoint present |
| Sign-up, sign-in | Not required |
| Background updater service | Not installed |
| Experiments / remote feature flags | None |
| Extension marketplace | Open VSX |
| Embedded agent (Claude) | Runs only when you start it, on **your own subscription** |

When you use the embedded agent, requests go through your own provider account; we are not in the middle
and nothing passes through a server of ours. If you never use the agent, the editor runs fully offline.

Updates are pull-only: new versions are published to Releases, and the editor does not fetch them on its
own. Use **Watch → Releases only** on this repository to get notified.

## Themes

Five themes ship built in. Each defines 183 colour keys plus a 16-colour terminal palette, so the whole
UI and the terminal are covered rather than half-themed.

Theme files use the standard format:

```jsonc
{
  "name": "theme-name",
  "type": "dark",
  "colors": {
    "editor.background": "#0b0d10",
    "editor.foreground": "#d7dae0",
    "terminal.ansiRed": "#e06c75"
  },
  "tokenColors": [
    { "scope": "comment", "settings": { "foreground": "#5c6370" } }
  ]
}
```

To share a theme, fix colours in an existing one, or propose a new theme, use the
**[talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes)** repository.
Theme issues belong there, not here.

## Forum and support

The forum on the website reads this repository's
**[Discussions](https://github.com/talkdedseccode/talkdedsec-editor/discussions)**. A post you write here
also appears on the site.

| What | Where |
| --- | --- |
| Crash or wrong behaviour | [Issues → Bug report](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=hata_bildirimi.yml) |
| Feature request | [Issues → Feature request](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=ozellik_istegi.yml) |
| Question, usage, how-to | [Discussions → Q&A](https://github.com/talkdedseccode/talkdedsec-editor/discussions/categories/q-a) |
| Security vulnerability | [SECURITY.md](SECURITY.md) — do not open a public issue |
| Themes | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) |

Contribution rules: [CONTRIBUTING.md](CONTRIBUTING.md) · Code of conduct: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## License

MIT — [LICENSE](LICENSE). Licenses of the upstream project and bundled components are in
[THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
