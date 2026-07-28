# Katkı Rehberi / Contributing

[English below ↓](#contributing-english)

## Önce: doğru yeri seçin

Yanlış yere açılan konu kaybolur. Aşağıdaki tablo tek kuraldır:

| Durumunuz | Gideceğiniz yer |
| --- | --- |
| Editör çöküyor, donuyor, yanlış davranıyor | [Issues → Hata bildirimi](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=hata_bildirimi.yml) |
| Şu özellik olsa iyi olur | [Issues → Özellik isteği](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=ozellik_istegi.yml) |
| Soru, "nasıl yapılır", kurulum yardımı, kullanım | [Discussions → Q&A](https://github.com/talkdedseccode/talkdedsec-editor/discussions/categories/q-a) |
| Fikir, genel sohbet, kurulumunuzu göstermek | [Discussions](https://github.com/talkdedseccode/talkdedsec-editor/discussions) |
| Tema önerisi, tema hatası, kendi temanız | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) deposu |
| Güvenlik açığı | [SECURITY.md](SECURITY.md) — herkese açık issue **açmayın** |

**Soru sormak için issue açmayın.** Issue'lar iş takibi içindir; sorular Discussions'ta hem daha hızlı
yanıt alır hem de sonradan arayan başkasının işine yarar. Soru olarak açılan issue'lar Discussions'a
taşınır.

## İyi bir hata bildirimi

Bir hata bildiriminin işe yaraması tek şeye bağlı: **biz de aynı hatayı görebiliyor muyuz?**

- Adım adım yeniden üretme yolunu yazın. "Bazen kapanıyor" ile bir şey yapamayız.
- Sürüm numarasını verin (`Yardım → Hakkında`).
- Windows sürümünü verin.
- Eklentileri kapatıp denediniz mi, yazın. Sorun sizin kurduğunuz bir eklentiden geliyorsa
  o eklentinin deposuna bildirmeniz gerekir.
- Çökme varsa günlük çıktısını ekleyin.
- Ekran görüntüsü faydalıdır ama adımların yerini tutmaz.

Yeniden üretemediğimiz ve ek bilgi gelmeyen bildirimler bir süre sonra kapatılır; yeni bilgiyle her
zaman yeniden açılabilir.

## Özellik isteği

Ne istediğinizden çok **hangi sorunu yaşadığınızı** yazın. "X düğmesi ekleyin" yerine "şunu yapmaya
çalışırken şu adımda tıkanıyorum" daha iyi sonuç verir; çözüm sizin düşündüğünüzden farklı olabilir.

Projenin duruşuna aykırı istekler reddedilir ve gerekçesi yazılır. Kabul edilmeyecek şeyler:

- Telemetri, kullanım istatistiği, "anonim" veri toplama
- Zorunlu hesap açma / oturum açma
- Arka planda kendiliğinden çalışan güncelleme servisi
- Uzaktan açılıp kapatılan deneysel özellik bayrakları

Bir istek reddedildiğinde bu "kötü fikir" demek değildir; bu ürün için uygun değil demektir.

## Pull request

Şu an bu depoda **dağıtım (Releases), belgeler ve konu takibi** yer alıyor. Buraya gönderilebilecek
PR'lar:

- Belge düzeltmeleri: README, SECURITY, CONTRIBUTING, şablonlar
- Yazım, dil ve çeviri düzeltmeleri (TR ve EN)
- Issue/PR şablonlarında iyileştirme
- Üçüncü taraf bildirimlerinde eksik veya hatalı atıf düzeltmesi

Yol:

1. Depoyu çatallayın, bir dal açın: `duzeltme/kisa-aciklama`
2. Değişikliği yapın. Küçük ve tek konulu tutun — 3 konuyu tek PR'da birleştirmeyin.
3. Commit mesajını Türkçe ve açıklayıcı yazın: `readme: ölçüm tablosuna disk boyutu eklendi`
4. PR açın, şablonu doldurun.

Büyük bir değişiklik düşünüyorsanız önce Discussions'ta veya bir issue'da konuşun. Kimsenin boşa emek
harcamasını istemiyoruz.

### Belgelerde dil kuralı

Bu depodaki belgeler **iki dillidir: Türkçe üstte, İngilizce altta.** Bir bölümü değiştiriyorsanız
diğer dildeki karşılığını da güncelleyin. Tek dilde bırakılmış değişiklikler birleştirilmez.

Rakamlara dokunmayın: README'deki ölçüm tablosundaki değerler ölçülmüş değerlerdir. Yeni bir rakam
ekliyorsanız nasıl ölçtüğünüzü PR'da yazın.

## Davranış

[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) bu depodaki her yerde geçerlidir: issue, PR, Discussions.

## Lisans

Katkınız kabul edildiğinde bu projenin MIT lisansı altında yayımlanır ([LICENSE](LICENSE)). PR açarak
bunu kabul etmiş olursunuz. Başkasına ait kod gönderiyorsanız kaynağını ve lisansını PR'da belirtin.

---

<a id="contributing-english"></a>

# Contributing (English)

## First: pick the right place

A thread opened in the wrong place gets lost. This table is the only rule:

| Your situation | Where to go |
| --- | --- |
| Editor crashes, freezes, misbehaves | [Issues → Bug report](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=hata_bildirimi.yml) |
| It would be good if it did X | [Issues → Feature request](https://github.com/talkdedseccode/talkdedsec-editor/issues/new?template=ozellik_istegi.yml) |
| Question, how-to, install help, usage | [Discussions → Q&A](https://github.com/talkdedseccode/talkdedsec-editor/discussions/categories/q-a) |
| Ideas, general chat, showing your setup | [Discussions](https://github.com/talkdedseccode/talkdedsec-editor/discussions) |
| Theme proposal, theme bug, your own theme | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) repository |
| Security vulnerability | [SECURITY.md](SECURITY.md) — do **not** open a public issue |

**Do not open an issue to ask a question.** Issues track work; questions get answered faster in
Discussions and stay useful for the next person searching. Issues that are questions get moved to
Discussions.

## A good bug report

Whether a bug report is useful comes down to one thing: **can we see the same bug?**

- Write step-by-step reproduction. "It sometimes closes" gives us nothing.
- Give the version number (`Help → About`).
- Give your Windows version.
- Say whether you tried with extensions disabled. If the problem comes from an extension you installed,
  it needs to be reported to that extension's repository.
- Attach log output if there is a crash.
- Screenshots help but do not replace the steps.

Reports we cannot reproduce and that get no further information are closed after a while; they can
always be reopened with new information.

## Feature requests

Describe **the problem you have**, not only the solution you imagined. "I get stuck at this step while
trying to do X" works better than "add an X button" — the fix may look different from what you pictured.

Requests that conflict with the project's stance are declined, with a reason. Things that will not be
accepted:

- Telemetry, usage statistics, "anonymous" data collection
- Mandatory account creation or sign-in
- A background updater service that runs on its own
- Remotely toggled experiment flags

A declined request does not mean "bad idea"; it means it is not right for this product.

## Pull requests

Right now this repository holds **distribution (Releases), documentation and issue tracking**. PRs that
belong here:

- Documentation fixes: README, SECURITY, CONTRIBUTING, templates
- Spelling, wording and translation fixes (TR and EN)
- Improvements to issue/PR templates
- Corrections to missing or incorrect third-party attribution

How:

1. Fork the repository and create a branch: `duzeltme/short-description`
2. Make the change. Keep it small and single-topic — do not bundle three subjects into one PR.
3. Write a clear commit message in Turkish: `readme: ölçüm tablosuna disk boyutu eklendi`
4. Open the PR and fill in the template.

If you are planning something large, discuss it first in Discussions or an issue. Nobody should waste
their effort.

### Language rule for documentation

Documents in this repository are **bilingual: Turkish on top, English below.** If you change a section,
update its counterpart in the other language too. Single-language changes are not merged.

Do not touch the numbers: the values in the README measurement table are measured values. If you add a
new number, explain in the PR how you measured it.

## Conduct

[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) applies everywhere in this repository: issues, PRs, Discussions.

## License

Accepted contributions are published under this project's MIT license ([LICENSE](LICENSE)). By opening a
PR you agree to this. If you submit code written by someone else, state its source and license in the PR.
