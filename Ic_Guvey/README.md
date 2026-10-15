# İÇ GÜVEY

AI ile üretilen, 9:16 dikey formatta 1 dakikalık intikam, aldatılma ve fiziksel/sosyal dönüşüm drama dizisi (Revenge & Transformation Drama Series). Görseller GPT Image (dikey 9:16 ve 3:2 referans sayfaları), videolar Gemini Omni 1.1 Flash (4, 6, 8, 10 sn'lik klipler), sesler Omni video modelinde doğal İngilizce (veya Türkçe dublaj/altyazı seçeneği).

**Konu:** Zengin bir aileye iç güvey giren, 145 kilo ve hor görülen Kerem'in uğradığı aşağılanmalar (aile yemeğinde tokat, boşanma protokolü, kapı dışarı ediliş, lüks restoranda kafasının pastaya basılması), eski boks şampiyonu Cemal Usta'nın köhne salonuna sığınması, yoğun bir antrenmanla dönüşmesi ve intikam için geri dönüşü.

Bu klasör, `gecmişs2.md` dosyasındaki sohbet dökümünün (satır 1–1.498) bölüm bölüm ayrılmış halidir. Kaynak metin değiştirilmeden korunmuştur ("bozmadan hazırla"). Promptlar kopyalanabilsin diye kod bloklarına (` ```text `) alınmış, ham tablolar standart markdown tablolarına dönüştürülmüştür.

## Klasörler

| Klasör | İçerik |
|---|---|
| `00_Genel_ve_Referanslar/` | Dizi format kuralları, 10 bölümlük akış, Kerem (Faz 1, 2, 3), Rüya, Handan Hanım, Cemal Usta ve mekân kartları |
| `Bolum_1_Kapi_Disari/` | Bölüm 1: Kapı Dışarı (Klip 0–9 promptları: Akraba yemeği, tokat kancası, kovulma, Cemal Usta ve kapak) |
| `Bolum_2_Yil_Donumu/` | Bölüm 2: Yıl Dönümü (Klip 0–10 promptları: Lüks restoran, KAAN girişi, pastaya basma ve cliffhanger) |
| `Raporlar_ve_Dersler/` | YouTube Studio performans analizi, metrikler, Bölüm 1 Fix List ve AI yapım kuralları |

## Bölüm Durumu: Kaynakta Ne Var, Ne Yok

| Bölüm | Süre / Format | Kaynakta Olan | Kaynakta Olmayan |
|---|---|---|---|
| **Bölüm 1 – Kapı Dışarı** | ~66 sn, 10 klip (0–9) | Klip 0–9 tam promptları, başlangıç kareleri, montaj sıralaması, 9:16 kapak promptu, YouTube yayın paketi | Yok (tam takım mevcut) |
| **Bölüm 2 – Yıl Dönümü** | ~60 sn, 11 klip (0–10) | Klip 0–10 tam promptları, KAAN ve Restoran referans kartları, YouTube yayın metni, etiketler | Yok (tam takım mevcut) |
| **Bölüm 3–10 (Gelecek Planı)** | 1 dk dikey format | 10 bölümlük kanca cümleleri, ekran metinleri ve genel hikâye akışı | Klip promptları (henüz yazılmadı) |

## Karakter ve Mekân Referans Listesi

| Karakter / Mekân | Rol / Tanım | Özellikler / Referans Notu |
|---|---|---|
| **KEREM (1. Faz)** | Başrol (Aşağılanan damat) | 30 yaşında, 145 kg, aşırı kilolu, terleyen yuvarlak yüz, ucuz mavi kareli gömlek, ucuz dijital saat |
| **KEREM (2. Faz)** | Dönüşüm süreci | 105 kg, yağ kaybetmiş, geniş omuzlu, kaslı, spor kıyafetli boksör |
| **KEREM (3. Faz)** | Zafer ve İntikam | 88 kg, kusursuz kesimli İtalyan takım elbise, lüks saat, karizmatik iş insanı |
| **RÜYA** | Kibirli Eş | 28 yaşında, soğuk, lüks zümrüt yeşili saten elbiseler, pırlanta takılar |
| **HANDAN HANIM (NEVIN)** | Otoriter Kayınvalide | 52 yaşında, sivri dilli, siyah gece elbisesi, gösterişli elmas kolye, uzun kırmızı tırnaklar |
| **CEMAL USTA** | Antrenör / Akıl Hocası | 58 yaşında, eski boks şampiyonu, kır saçlı, kırışık ama sert yüz, gri kapüşonlu |
| **KAAN** | Zengin Rakip (Rüya'nın sevgilisi) | 32 yaşında, atletik, bronz tenli, lüks lacivert blazer ceket, altın Rolex saat |
| **Mekân 1: Yalı Salonu** | Boğaz Manzaralı Villa | Beyaz mermer masa, zümrüt yeşili kadife sandalyeler, kristal avize, Boğaz pencereleri |
| **Mekân 2: Boks Salonu** | Köhne Boks Salonu | Paslı demirler, yıpranmış deri kum torbaları, floresan ışıklar, terli beton zemin |
| **Mekân 3: Fransız Restoranı** | Lüks Restoran | Koyu mermer paneller, beyaz örtülü masalar, kristal kadehler, piyano köşesi |

## Analizde Dikkat Çeken Noktalar

1. **Flash-Forward Açılış Kancası (Klip 0):** Her bölüm ilk 4–6 saniyede gelecekteki büyük intikam veya skandal anını gösterir; ardından "6 MONTHS EARLIER" yazısıyla geriye döner. Bu teknik izleme terkini (swipe-away) minimuma indirir.
2. **Eller Kuralı:** Yapay zekânın elleri deforme etmesini engellemek için her görsel promptuna `Hands: anatomically correct human hands with exactly five fingers each, natural grip` kuralı eklenmiştir.
3. **Omni Kelime Sınırı:** Dudak senkronunun bozulmaması için 4 saniyede en fazla 8 kelime, 6 saniyede en fazla 12 kelime kuralı uygulanmıştır.
4. **Kesme Ritmi:** Ortalama klip süresi 6 saniyedir; aksiyon anlarında 2 saniyelik insert planlar (yüzük kutusu vb.) kullanılır.
5. **Ses Tutarlılığı:** Her karakterin ses profili (Nevin: soğuk elit ton; Kerem: çekingen derin ton; Kaan: kibirli tok ton) tüm kliplerde kelimesi kelimesine kilitlenmiştir.

## Bölme ve Doğrulama

- Dosyalar `gecmişs2.md` dosyasının 1–1.498 satır aralığından eksiksiz üretilmiştir.
- Hangi dosyanın hangi satırlardan geldiği `.manifest.tsv` dosyasında kayıtlıdır.
