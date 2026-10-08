# STAY IN THE DARK (Karanlıkta Kal)

AI ile üretilen, 30 dakika hedefli zombi filmi. Video Gemini Omni ile (4, 6, 8, 10 sn'lik klipler), başlangıç kareleri ve referanslar GPT Image ile. Diyaloglar İngilizce, Türkçe altyazı.

**Kural:** Zombiler duymaz, karanlıkta görmez, ama ışığa koşar.

Bu klasör, `1.md`'deki sohbet dökümünün bölüm bölüm ayrılmış hali. Kaynak metin değiştirilmedi. Promptlar kopyalanabilsin diye kod bloklarına alındı, tablolar markdown tablosuna çevrildi. `[Derleyen notu]` ile başlayan satırlar sonradan eklenen açıklamalar.

## Klasörler

| Klasör | İçerik |
|---|---|
| `00_Referanslar/` | Karakter ve mekân referans promptları (#1–#9) ve geçersiz ilk sürüm |
| `00_Genel/` | Sahne 13'ten sonraki "nerede duruyoruz" ara planı |
| `Bolum_1_Soguk_Acilis/` | Sahne 1–5 (Marco'nun ölümü) |
| `Bolum_2_Kurulum/` | Sahne 6–11 (Ellie, Kyle, Frank) |
| `Bolum_3_Ilk_Temas/` | Sahne 12–15 (koridor, merdiven, bodrum) |
| `Bolum_4_Mahsur/` | Sahne 16–21 (lobi, 1A, kalem feneri) |
| `Bolum_5_Doruk/` | Sahne 22–24 (jeneratör, Frank'in fedakârlığı, tırmanış) |
| `Bolum_6_Final/` | Sahne 25–29 ve kapanış (çatı, helikopter, şafak) |
| `Fragman_ve_Kapak/` | Fragman, teaser, dikey kesim, T1–T22 promptları, film adı, 3 kapak |
| `Arastirma/` | 4 derin araştırma promptu, gelen raporlar, yapım rehberi v2, yeni film önerisi |

## Bölüm durumu: kaynakta ne var, ne yok

| Bölüm | Süre (sohbetteki son hali) | Kaynakta olan | Kaynakta olmayan |
|---|---|---|---|
| 1 – Soğuk açılış | 0:00–2:14, 23 klip | Sahne 3, 4 (tablolar yok). Sahne 1 ve klip tabloları yalnızca eski sürümde | Sahne 2 ve 5 promptları (5.4 anons, 5.5 başlık kartı dahil) |
| 2 – Kurulum | kırpmalardan sonra ~3:20 | Sahne 6, 7, 11, test sonrası düzeltmeler | Sahne 8, 9, 10; test sonuçları |
| 3 – İlk Temas | ~6:40 → ~12 dk | Sahne 12, 13, 14; Sahne 15 düzeltmeleri | Sahne 15 tablosu, 15.1–15.2, 15'in ilk sürümü |
| 4 – Mahsur | ~6:30, film 18. dakikaya varıyor | Sahne 20, 21 | Sahne 16, 17, 18, 19 |
| 5 – Doruk | ~4 dk, film 22. dakikaya varıyor | Sahne 22, 23, 24 | yok |
| 6 – Final | ~22:10 → ~30:00 | Plan, referans #31–#35, Sahne 25, 26, 27 | Sahne 28, 29, kapanış promptları |

Promptu olan klipler: 175 (Bölüm 1–6), eski sürümdeki Sahne 1 ile 178. Fragman: 22 klip.

Bu boşlukların sebebi büyük ihtimalle paylaşım sayfasından kopyalama. Sohbetin tamamı `1.md`'ye gelmemiş. Eksik sahneler için sohbeti claude.ai'da açıp o mesajları ayrıca kopyalaman gerekiyor.

> **[Derleyen notu]** `1.md`'nin ilk, 81 satırlık halinde soğuk açılışın tam klip tablosu ve Sahne 1 promptları vardı; yeni `1.md`'de bunlar yok. O metin `Bolum_1_Soguk_Acilis/eski_surum_ilk_1md/` klasöründe korunuyor.

## Referanslar

Üretim promptu kaynakta olanlar: #1–#9 (`00_Referanslar/02_...`) ve #31–#35 (`Bolum_6_Final/00_...`). #10–#30'un promptları kaynakta yok; sadece adları geçiyor.

| No | Ad | No | Ad |
|---|---|---|---|
| #1 | Ellie | #19 | Hollis |
| #2 | Kyle | #20 | Merdiven sahanlığı |
| #3 | Frank | #21 | Lobi |
| #4 | Marco | #22 | Bodrum |
| #5 | Eşofmanlı zombi | #23 | Kırmızı halka |
| #6 | Mrs. Doyle | #24 | Zombi Marco |
| #7 | Göz parlaması | #25–#28 | Adı hiç geçmiyor (muhtemelen Bölüm 4'teki yeni zombi tasarımları) |
| #8 | Sokak | #29 | Fotoğraf |
| #9 | Rosewood girişi | #30 | Dolu lobi |
| #10 | Salon | #31 | Çatı |
| #11 | Mutfak köşesi | #32 | Çatı kapısı (dış taraf) |
| #12 | Kyle'ın odası | #33 | Helikopter |
| #13 | Daire kapısı | #34 | Şafak |
| #14 | Koridor ve merdiven | #35 | Işığa yürüyenler |
| #15 | Pencereden sokak ve karşı bina | | |
| #16 | Telefon | | |
| #17 | Kalem feneri | | |
| #18 | Radyo | | |

## Analizde dikkat çeken noktalar

1. **Plan sohbet içinde değişti.** `00_Genel/`'deki ara planda Sahne 21 "Kuşatma", Bölüm 6 ise Sahne 25–26 idi. Son halinde Sahne 21 Bölüm 4'ün finali ("Başka bir yol"), Bölüm 5 Sahne 22–24, Bölüm 6 Sahne 25–29 ve kapanış. Geçerli olan son hali.
2. **Sahne 19 yeniden yazılmış.** Ara planda Kyle bodrumda tek başına; Sahne 21'deki not ise 19.4'te Frank'in "If this place has a heart, it's down here" repliğinden söz ediyor. Sahne 19'un yeni hali kaynakta yok.
3. **Soğuk açılış büyüdü.** Eski sürümde 21 klip ve ~2:00, durum tablosunda 23 klip ve 2:14. Fragmandaki "5.5 başlık kartı" ve düzeltmelerdeki "5.4 anons" bu eklemeler.
4. **Kurallar zamanla eklendi.** Hangi sahneden itibaren geçerli olduklarına dikkat et:
   - Sahne 6'dan itibaren: her video promptunda ses bölümü, konuşan karakterin ses tarifi.
   - Sahne 11'den itibaren: replik ilk saniyede, bakış yönü yazılı, çok kısık ışık, yakın plan diyalogda en fazla 2 halkalı zincir, tam profil yok, kalabalık sadece koşar (`Bolum_2_Kurulum/Sahne_07-10_...`).
   - Sahne 21'den itibaren: genç görünen karakter ağzına bir şey götürüp çekmez (inhaler dahil).
   - Sahne 22'den itibaren (kullanıcının isteği): sahneler arası zincir ve önceki sahnelerin karelerini yeniden kullanma yok.
5. **Sahne 15'te iki düzeltme turu var.** Geçerli olan sondaki "Güncellenmiş plan". 15.7 orada 4 sn değil 6 sn.
6. **Yapım rehberi v2 yeni film için.** Işık kuralını yumuşatıyor ("no rim light, no hard shadows" kalkıyor) ve "young" kelimesini yasaklıyor. Bu filmin mevcut promptları eski kurallarla yazıldı; ikisini karıştırma.
7. **Film adı.** "STAY IN THE DARK" önerildi ve başlık kartında zaten kullanılıyor. Kullanıcının onayı kaynakta görünmüyor.
8. **Sohbet yeni bir filmle bitiyor.** Son mesaj found-footage tarzı "Arkana Bakma" fikrini öneriyor ve "listedeki" diyerek bir fikir listesine atıf yapıyor. O liste kaynakta yok.

## Bölme ve doğrulama

- Dosyalar bir script ile satır aralıklarından üretildi. Hangi dosyanın hangi satırlardan geldiği `.manifest.tsv`'de ve her dosyanın başında yazıyor.
- Atlanan satırlar: sohbet arayüzünün "düşünüyor" özetleri (satır 2, 52, 53, 1395, 1547, 1708, 2274, 2315) ve sayfa altlığı "Update Shared Chat" (satır 3013).
- Doğrulama: bütün dosyalar geri çevrilip `1.md` ile satır satır karşılaştırıldı. Sonuç 0 fark; yukarıdakiler dışında dışarıda kalan satır yok.
- `Arastirma/02_Arastirma_Raporlari_KULLANICI.txt` kullanıcının yapıştırdığı 4 raporun ham hali; tabloları bozuk olduğu için hiç dokunulmadı.
