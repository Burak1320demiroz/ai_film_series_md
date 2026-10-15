# SAVE THEM OR DIE (Kurtar Ya Da Öl)

AI ile üretilen, 9:16 dikey formatta Orta Çağ Sistem Fantezisi (System Fantasy / Medieval Drama). Görseller GPT Image, videolar Google Veo ve Gemini Omni 1.1 Flash, seslendirmeler ElevenLabs (Seer Morganna, Chuck Miller, Charmion, Cruella).

**Kural:** Kader Sistemi seçti: Üç kadını açık artırmadan kurtar, sadakatlerini kazan ya da kum saati bittiğinde öl.

Bu klasör, `gecmiş.md` dosyasındaki ilk sohbet dökümünün (satır 1–488) bölüm bölüm ayrılmış halidir. Kaynak metin değiştirilmedi ("bozmadan hazırla" prensibi). Promptlar kopyalanabilsin diye kod bloklarına (` ```text `) alındı, tab-ayrımlı tablolar standart markdown tablosuna dönüştürüldü. `[Derleyen notu]` ile başlayan satırlar sonradan eklenen bağlam açıklamalarıdır.

## Klasörler

| Klasör | İçerik |
|---|---|
| `00_Referanslar/` | Karakterler (Rowan, Elara, Mira, Sera, Cedric, Brandt, Tobin) ve Kostüm A/B/C referans rehberi |
| `01_Fragman_ve_Genel/` | Fragman analizi, 8 klip tablosu, ara sahneler, Veo promptları, YouTube İngilizce başlık ve yayın metni |
| `Bolum_1_Mezarcinin_Evi/` | Bölüm 1 kurgu/ritim analizi, Klip 4–9, giyinme sahneleri, müzik ve anlatıcı yerleşimi |
| `Bolum_2_Hain_Kim/` | Bölüm 2 kurgu tablosu (Hain Kim?), Klip 1–10 promptları, sadakat paneli ve yayın metni |
| `Bolum_3_Seranin_Bedeli/` | Bölüm 3 taslağı (Sera'nın Bedeli), kadınlar odaklı kanca ve ilk 4 klip hazırlığı |

## Bölüm Durumu: Kaynakta Ne Var, Ne Yok

| Bölüm | Süre / Format | Kaynakta Olan | Kaynakta Olmayan |
|---|---|---|---|
| **Fragman** | ~64–72 sn, 8–10 klip (Veo/Omni) | 8 klip tablosu, ara sahne kurguları, Veo promptları, başlık seçenekleri, etiketler | Görsel dosya ekleri (chatte metin olarak üretildi) |
| **Bölüm 1 – Mezarcının Evi** | ~80 sn, 9–10 klip | Ritim analizi, Klip 4–9 promptları, ara sahneler, müzik/anlatıcı zamanlaması, Sera ses testi | Klip 1–3 başlangıç promptları (chatte daha önceki versiyonda onaylandı) |
| **Bölüm 2 – Hain Kim?** | ~60 sn, 10 klip | 9/10 klip kurgu planı, Klip 1–10 promptları, sadakat paneli, YouTube yayın metni | Ham video render çıktıları |
| **Bölüm 3 – Sera'nın Bedeli** | 9 klip taslak | Kadınlar kancası planı, 9 klip sinopsisi, ilk 4 klip ön hazırlığı | Klip 5–9 tam promptları |

## Karakter ve Referans Haritası

| Karakter | Rol / Açıklama | Kostümler |
|---|---|---|
| **Rowan** | Beş parasız mezarcı; Kader Sistemi'nin seçtiği ev sahibi | Yıpranmış tunik / Kasaba sonrası yeni kıyafet |
| **Elara** | Düşmüş lordun kızı; zeki, gururlu | Saten gecelik & fildişi sabahlık (Kostüm C) |
| **Mira** | Elara'nın ablası; kılıç ustası, koruyucu | Kömür grisi kolsuz saten gecelik & hançer kemeri (Kostüm C) |
| **Sera** | Eski saray şarkıcısı; gizli sadakat taşıyan hain | Yırtmaçlı kırmızı saten gecelik & pelerin (Kostüm C) |
| **Cedric** | Rowan'ın çocukluk düşmanı; kibirli beyzade | Kürk pelerin, süslü kılıç |
| **Brandt** | Cedric'in muhafız komutanı | Zırhlı devriye kostümü |
| **Tobin** | Sera'nın tutsak kardeşi (yetişkin) | Zindan kıyafeti |

## Analizde Dikkat Çeken Noktalar

1. **MOD A Kanca Motoru:** Görev + sayaç → bedel → sayaç hatırlatma → ödül → büyük döküm döngüsü 64–72 saniyeye sıkıştırılmıştır.
2. **Kum Saati Kuralı:** Sistem dijital fontlarla değil, yalnızca Rowan'ın gördüğü havada asılı altın/kırmızı kum saatiyle temsil edilir. Yazılar ve paneller videoya değil montajda grafik olarak eklenir.
3. **Kadınların Temsili:** Cinselleştirilmiş esaret kalıpları (iç çamaşırı, çıplaklık) Veo ve platform filtrelerine takılmaması için asil, giyinik, zarif saten/kadife geceliklerle değiştirilmiştir.
4. **Kesme Ritmi:** Ortalama kesme süresi 3 saniyede tutulur. Uzun klipler %115–125 dijital zoom ile ikiye bölünür.
5. **Ses Ayrımı:** Rowan/Cedric/Mira/Sera replikleri Veo veya ElevenLabs ile konuşur; Seer Morganna (Sistem) yankılı VO, anlatıcı ise Chuck Miller olarak konumlandırılmıştır.

## Bölme ve Doğrulama

- Dosyalar `gecmiş.md` dosyasının 1–488 satır aralığından eksiksiz üretilmiştir.
- Hangi dosyanın hangi satırlardan geldiği `.manifest.tsv` dosyasında kayıtlıdır.
