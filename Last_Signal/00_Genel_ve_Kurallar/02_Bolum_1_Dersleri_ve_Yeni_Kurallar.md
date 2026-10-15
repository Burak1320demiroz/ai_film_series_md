# Genel – Bölüm 1'den Çıkan Dersler ve Yapım Kuralları

_Kaynak: `gecmiş.md`, satır 684–736. Metin değiştirilmeden aktarıldı._

> **[Derleyen notu]** Senaryo, görüntü/tutarlılık, kurgu, Omni 1.1 kuralları, 60 saniyelik yeni bölüm şablonu ve kontrol listesi.

<!-- kaynak-başlangıç -->

Bölüm 1'den çıkan dersler
Senaryo
Seçim ve bedel asla kesilmez. Her bölümün olmazsa olmaz iki satırı var: kararın kendisi ve neye mal olduğu. Kurgu sırasında süreyi kısaltmak gerekiyorsa başka yerden kes.
Ödemesi olan hazırlık da kesilmez. Sinyal kaydı gitti ama “Signal corrupted” kaldı; ödeme havada kaldı. Bir satırı keserken ona bağlı satırı da kontrol et.
Görüntü ve tutarlılık
Ayırt edici detaylar tek tek yazılmalı. Omuzdaki turuncu yama sol koldan sağa geçti. Her promptta “orange patch on her LEFT shoulder” diye açıkça yaz. Kemer ve askı gibi ayrıntıları kostümden çıkar; geometrisi bozuluyor.
Amber halka da kesin tarifle sabitlenmeli. Halka fazladan iç içe halkalar kazandı. Her promptta “a single thin amber ring” yaz.
Eller hologramlardan uzak dursun. El hologram ışınlarına karıştı. Ada’nın elleri ya iki yanında ya kadraj dışında olsun; hologramlara bakarak tepki versin.
Mekanik hareketler kısa kalsın. Kapaklar kapanırken lastik gibi esnedi. Bu tür hareketleri 4 saniyelik kliplere koy ve sert bir metal sesiyle maskele.
Kapanış kartı sade olsun. Kapaktaki eldeki başparmak bozulmuştu. Bölüm sonuna siyah zemin üstüne yalnızca başlık koy.
Kurgu
Geri sayım görsel katmanı zorunlu. 60 saniyelik acil durumun omurgası o; yoksa gerilim de yok. Kırmızıdan maviye ışık değişimi de kurguda düştüyse efektle ekle.
Altyazılar ekranın %65–70 yüksekliğinde olsun. Bu ikinci kez çıktı. CapCut’ta bir altyazı şablonu kaydet ve her bölümde onu kullan.
Plan uzunluğu kontrolü. Ortalama plan 6 saniye. 3 saniyeden uzun, yeni bilgi vermeyen hiçbir an kalmasın; tek istisna bilinçli olarak işaretlenmiş sessizlik.
Kanca ilk karede olsun. Açılış yavaş bir kamera hareketiyle başlamış. İlk kare hareketin ortasından başlasın: kıvılcım, alarm, Ada’nın yüzü çoktan tepkide.
Ses ve çeviri
VESPER’i işlemden geçir. Ada ile VESPER aynı akustikte duyuldu. Ada artık Omni’den doğal oda sesiyle geleceği için VESPER’e “istasyon hoparlörü” efekti ver: alçak frekansları kes, hafif yankı ekle.
Terim sözlüğü kullan. “Dizi” kelimesi TV dizisi gibi okundu. Sabit karşılıklar:
array → anten · Section C → C bölümü · escape pod → kaçış kapsülü · override → manuel kontrol · hull → gövde · signal → sinyal
Omni 1.1 Flash için yeni kurallar
Ada artık kamerada konuşuyor:
Repliği kısa tut. Her klipte tek replik, en fazla 8 kelime. Promptta tam zamanlamasıyla yaz: “At 3 seconds she says: ...”.
Sesini her promptta aynı tarifle sabitle. Her üretimde ses değişebilir; bunu önlemek için her promptta aynı satırı kullan: Ada's voice: low, steady, slightly husky, British accent, early thirties.
Kaymaya karşı yedek plan: Klipler arasında ses yine de kayarsa, Ada’nın repliklerini ElevenLabs’in Voice Changer’ından sabit bir sese çevir. Zamanlama ve dudak hareketi korunur, ses tek tipe iner.
VESPER için boşluk bırak. VESPER’in konuşacağı anları Omni promptunda açıkça “Ada listens silently” olarak yaz. Promptun sonuna her zaman şunu ekle: No other voices, no narration, no music. Böylece VESPER’i ve müziği temiz bir zemine eklersin.
Süreleri sahneye göre seç:
4 sn: alarm, dış çekim, tepki, kısa ekleme
6 sn: tek replik ve ardından tepki
8 sn: VESPER’in konuşması ve Ada’nın cevabı
10 sn: yalnızca bölümün doruk anı; bölüm başına en fazla bir kez
Yeni bölüm şablonu (60 sn, 11 klip):
1. Kanca — 4 sn: alarm, Ada zaten tepkide (VESPER: acil durum + süre)
2. Tehlike — 4 sn: dış çekim
3. VESPER'in çözümü ve bedeli — 6 sn: Ada dinliyor, tepki veriyor
4. İtiraz — 6 sn: Ada'nın repliği
5. Baskı — 4 sn: göz veya hologram yakın planı (VESPER: geri sayım)
6. Riskli yol — 6 sn: Ada'nın repliği
7. Uyarı — 4 sn: Ada'nın tepkisi (VESPER: olasılık)
8. KARAR — 6 sn: Ada'nın komutu + ışık değişimi
9. Sonuç — 6 sn: dış çekim
10. Hazırlık/ödeme — 8 sn: sinyal, kayıt ya da ipucu
11. Ürpertici son — 6 sn: VESPER'in son satırı, halka nabzı
+ 2 sn siyah zemin üstünde başlık kartı
Yüklemeden önce kontrol listesi:
□ Seçim satırı ve bedel satırı var
□ Her ödemenin hazırlığı duruyor
□ Geri sayım 0:02'den çözüme kadar ekranda
□ Altyazı %65–70 yükseklikte, terimler sözlüğe uygun
□ VESPER'e hoparlör efekti verildi
□ 3 saniyeden uzun ölü an yok (bilinçli sessizlik hariç)
□ Ada'nın sesi tüm kliplerde aynı
□ Bitiş: siyah zemin, başlık, 2 sn
Bölüm 1'deki düzeltmelerin çoğu (eksik sesler, geri sayım, altyazı yeri, terim, kırpmalar) yalnızca kurgu işi. İstersen düzeltip yeniden yükleyebilirsin; tek yeniden üretilmesi gereken, Ada’nın ağzının oynadığı klip.

<!-- kaynak-bitiş -->
