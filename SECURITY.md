# Güvenlik Politikası / Security Policy

[English below ↓](#security-policy-english)

## Açık bildirimi

**Güvenlik açığı için herkese açık issue veya Discussions gönderisi açmayın.** Bildirimi özel kanaldan
yapın:

**→ [Güvenlik danışmanlığı aç (GitHub Security Advisories)](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new)**

Bu form yalnızca depo yöneticilerine görünür. Konuşma, düzeltme yayımlanana kadar özel kalır.

GitHub hesabınız yoksa veya form size kapalıysa, **hiçbir teknik ayrıntı yazmadan**
`Güvenlik: özel kanal talebi` başlıklı bir issue açın; size özel bir iletişim yolu veririz. Açığın
kendisini o issue'da anlatmayın.

## Bildirimde yer alması gerekenler

- Etkilenen sürüm (editörde `Yardım → Hakkında` ekranındaki sürüm numarası)
- Windows sürümü ve mimarisi
- Sorunun ne olduğu ve saldırganın ne kazandığı
- Adım adım yeniden üretme yolu — mümkünse en küçük örnek dosya/proje
- Varsa günlük çıktısı, çökme kaydı, ekran görüntüsü

Yeniden üretilebilir bir adım listesi, en iyi yazılmış açıklamadan daha değerlidir.

## Süreç

1. Bildiriminizi alır ve doğrulamaya çalışırız.
2. Doğrulanırsa düzeltmeyi hazırlar, yeni bir sürüm yayımlarız.
3. Sürümle birlikte bir güvenlik danışmanlığı (advisory) yayımlanır; aksini istemezseniz bulan kişi
   olarak adınız/kullanıcı adınız anılır.

Bu proje tek kişi tarafından yürütülüyor. **Yanıt süresi taahhüdü vermiyoruz** — gerçek olmayan bir
süre yazmaktansa bunu açıkça söylemeyi tercih ediyoruz. Bildiriminiz sırayla okunur ve yanıtlanır.

Ödül programımız yok, para ödülü veremiyoruz.

## Kapsam

| Kapsam içinde | Kapsam dışında |
| --- | --- |
| Editörün kendisi (bu depodan yayımlanan yapı) | Open VSX'ten kurduğunuz üçüncü taraf eklentiler |
| Releases'teki kurulum dosyası, kurulum davranışı | Üst projede bulunan ve henüz üst projede düzeltilmemiş açıklar |
| `code.talkdedsec.com` sitesi | Gömülü ajanın bağlandığı sağlayıcı servisi (ilgili sağlayıcıya bildirin) |
| Bu depodaki yapılandırma ve iş akışı dosyaları | Sosyal mühendislik, fiziksel erişim, DoS senaryoları |

Üst projeden devralınan bir açık bulursanız yine de bize haber verin; hem yapımızı etkileyip
etkilemediğine bakarız hem de sizi doğru yere yönlendirebiliriz.

## Desteklenen sürümler

Yalnızca **Releases'teki en son sürüm** güvenlik düzeltmesi alır. Eski sürümlere geriye dönük yama
yayımlanmaz — güncel sürüme geçin.

## Kurulum dosyasının doğruluğu

Kurulum dosyası yalnızca bu deponun [Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases)
sayfasından dağıtılır. Başka bir siteden, aynalardan veya paylaşım bağlantılarından indirdiğiniz dosya
bizim yayınımız değildir; böyle bir dağıtım görürseniz bildirin.

Paket henüz kod imzalı değildir. Çalıştırmadan önce SHA-256 özetini README'deki değer ve
[`checksums/`](checksums/) altındaki sürüme özel dosyayla doğrulayın. Özet eşleşmiyorsa dosyayı
çalıştırmayın ve özel güvenlik bildirimi açın.

---

<a id="security-policy-english"></a>

# Security Policy (English)

## Reporting a vulnerability

**Do not open a public issue or Discussions post for a security vulnerability.** Report it privately:

**→ [Open a security advisory (GitHub Security Advisories)](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new)**

That form is visible only to repository maintainers. The thread stays private until a fix is published.

If you do not have a GitHub account or the form is unavailable to you, open an issue titled
`Security: private channel request` with **no technical details at all**, and we will give you a private
contact route. Do not describe the vulnerability in that issue.

## What to include

- Affected version (the version number shown under `Help → About` in the editor)
- Windows version and architecture
- What the issue is and what an attacker gains
- Step-by-step reproduction — the smallest sample file/project you can manage
- Logs, crash records or screenshots if you have them

A reproducible list of steps is worth more than the best-written description.

## Process

1. We receive your report and try to reproduce it.
2. If confirmed, we prepare a fix and publish a new release.
3. A security advisory is published alongside that release; unless you prefer otherwise, you are
   credited by name or handle.

This project is run by one person. **We do not promise a response time** — we would rather say so plainly
than publish a number that is not real. Reports are read and answered in order.

There is no bug bounty; we cannot offer monetary rewards.

## Scope

| In scope | Out of scope |
| --- | --- |
| The editor itself (builds published from this repository) | Third-party extensions you install from Open VSX |
| The installer on Releases and its install behaviour | Upstream vulnerabilities not yet fixed upstream |
| The `code.talkdedsec.com` website | The provider service the embedded agent connects to (report it to the relevant provider) |
| Configuration and workflow files in this repository | Social engineering, physical access, DoS scenarios |

If you find a vulnerability inherited from upstream, tell us anyway; we will check whether our build is
affected and point you to the right place.

## Supported versions

Only the **latest release on Releases** receives security fixes. Older versions are not back-patched —
please update.

## Installer authenticity

The installer is distributed only from this repository's
[Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases) page. A file downloaded from
another site, a mirror or a shared link is not our build; if you see such a distribution, report it.

The package is not code-signed yet. Before running it, verify its SHA-256 digest against the value in
the README and the version-specific file under [`checksums/`](checksums/). If the digest does not
match, do not execute the file and open a private security report.
