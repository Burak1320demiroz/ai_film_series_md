# Rapor değerlendirmesi, yapım rehberi v2, viral strateji ve yeni film önerisi

_Kaynak: `1.md`, satır 2939–3009. Metin değiştirilmeden aktarıldı._

> **[Derleyen notu]** Satır içindeki "datanorth", "it", "morphic", "blog" gibi kısa satırlar kopyalanan kaynak etiketleri; olduğu gibi bırakıldı.

<!-- kaynak-başlangıç -->

Raporları okudum. İki önemli düzeltmeyle başlıyorum.

Yalnızca Omni ve GPT Image. Raporlar sık sık Seedance, Veo, Kling, Midjourney, Nano Banana, ElevenLabs ve Suno öneriyor; hepsini eledim. Kurgu tarafında DaVinci Resolve ve FFmpeg gibi araçlar kalıyor, çünkü bunlar üretim modeli değil, montaj araçları. Ses ve müzik için de dışarıdan bir AI aracı yok; diyaloglar Omni'nin kendi sesiyle, kalanı kurguda.

Raporların hepsi doğru değil. Derin araştırma raporları bazen tutarsız rakamlar ya da uydurma detaylar içerir. En kritik iki iddiayı, iki modelin yeni sürümlerini kendim kontrol ettim; ikisi de doğru çıktı. Ama bazı iddialar doğrulanamadı ya da bizim deneyimimizle çelişiyor:

"Filtreye takılan üretim ücretlendiriliyor." Senin paylaştığın Omni hata ekranında tam tersi yazıyordu: "Bu üretme işlemi için sizden ödeme alınmadı."

Rakamlar ve parametreler: TikTok'ta etiketsiz AI içeriğin erişiminin %73 düştüğü, Instagram'da dakikada 694 bin Reels paylaşıldığı, Omni'de bir "motion strength" ayarı olduğu, GPT Image'e 16 referans verilebildiği ve 16:9 boyutların doğrudan desteklendiği iddiaları doğrulanmadı. Bunları test etmeden kurala çevirmiyoruz.

#### Doğrulanan iki büyük yenilik

Gemini Omni 1.1 Flash. Google, Gemini Omni 1.1 Flash'ı 27 Ağustos 2026'da genel kullanıma açtı; model sahne uzatma, ilk ve son kare arası geçiş, ucuz 360p taslaklar ve 4K'ya kadar çıktı ekliyor. Ayrıntılar bizim için çok önemli: 

datanorth

Sahne uzatma artık yalnızca son kareyi değil, önceki 10 saniyeyi bağlam olarak okuyor ve toplamda 40 saniyeye kadar uzayabiliyor. 

it

İlk ve son kare sabitlenip kamera hareketi kontrol edilebiliyor; taslaklar 720p'nin üçte biri maliyetle 360p'de üretiliyor; video klipler de karakter tutarlılığı için referans verilebiliyor.

it

Omni Flash varsayılan olarak çok planlı küçük bir anlatı kuruyor; tek kesintisiz bir plan istendiğinde prompta "single continuous shot, no scene cuts" eklenmesi gerekiyor.

morphic

Aynı görseli hem ilk hem son kare olarak vermek kesintisiz bir döngü üretiyor. 

morphic

Sahne uzatma, Google AI Plus, Pro ve Ultra abonelerine Gemini uygulamasında da açık.

blog

GPT Image 2.5. OpenAI, 8 Eylül'de GPT Image 2.5'i iki API modeliyle yayınladı: hız öncelikli Flare ve kalite ile düzenleme hassasiyeti öncelikli Sunburst. Yeni sürüm GPT Image 2'ye göre referans fotoğraflara daha sadık, tek öğe düzenlemelerinde daha hassas ve çok adımlı düzenlemelerde daha tutarlı. ChatGPT'deki görsel üretimi de bu modelle çalışıyor.

> ## Documentation Index +2

#### Yapım rehberi v2: değişen kurallar

#### Omni

Her video promptuna "Single continuous shot, no scene cuts." Bu, ilk filmde bazı kliplerde gördüğümüz istenmeyen kesmelerin muhtemel sebebi.

İlk + son kare, yüz kaymasına karşı en güçlü aracımız. İki onaylı GPT Image karesinin arasını Omni'ye doldurtursak yüz iki uçta da sabitlenir. Zor hareketler (başını çeviren biri, açılan bir kapı), geçişler ve döngüler artık bu yöntemle yapılacak. Klasik zinciri yalnızca gerektiğinde kullanacağız.

Sahne uzatma uzun planlar için. Ama yakın plan yüzlerde 20 saniyeyi geçmemeyi öneririm. Rapor kaymanın bu civarda arttığını söylüyor; ilk testlerde bunu doğrularız.

Önce 360p taslak, sonra final. Her klibi önce ucuz taslakta dene; hareket ve kompozisyon doğruysa 720p final üret.

Diyalog yine İngilizce. Raporun dudak senkronu konusunda söyledikleri bizim deneyimimizle uyumlu: güvenilir olan yalnızca İngilizce.

Video promptlarında "cinematic" kelimesini test edelim. Rapora göre bu kelime abartılı ışık huzmelerine yol açıyor. İlk filmde 5.1'de yaşadığımız sorun buydu.

Sohbetle düzenlemede 3–4 turdan sonra karakteri yeniden tarif et ya da sıfırdan üret.

#### GPT Image 2.5

Final başlangıç kareleri ve düzenlemeler Sunburst'le, taslaklar Flare'le.

Yüz referansı her zaman ilk sırada ve rolü açıkça yazılı: "image 1 is the exact facial identity". Bunu zaten yapıyorduk; artık kural.

Düzenlemede her seferinde tek değişiklik, ve onaylanan her sonuç bir sonraki düzenlemenin girdisi.

Işık kuralımızı yumuşatıyoruz. İlk filmde "no rim light, no hard shadows" diyerek fazla düz kareler ürettik. Rapor, video modelinin derinliği ışık ve gölgeden okuduğunu söylüyor. Yeni kalıp: "soft directional key light from one side, gentle shadows; no light beams, no haze".

Başlangıç karesinde hareket bulanıklığı olmasın; karakterin gideceği yönde boşluk kalsın. 3/4 açı ve profil yasağı aynen devam.

Yazılar tırnak içinde, "render exactly once" ifadesiyle ve yüksek kalitede.

#### Kurgu

Ağır çekim hissi. AI klipler hareketi yavaşlatma eğiliminde. Diyalogsuz hareket kliplerini kurguda %110–125 hızlandır; konuşmalı kliplerde yapma, ses bozulur.

Titreme. Düz yüzeylerdeki kare kare titremeyi FFmpeg'le azaltabilirsin: ffmpeg -i girdi.mp4 -vf "nlmeans=s=6:p=3:r=9" cikti.mp4

Görsel birlik. DaVinci'de bütün filme tek bir renk düzeltmesi, en sona da ortak bir film greni.

Geçişler. Işık ve flaş geçişleri (temamıza tam uyuyor), J/L kesmeler ve ses köprüleri. Morph geçişi yok; rapor da bunun filmi ucuz gösterdiğini söylüyor.

#### Filtreler

Karakterin yaşı promptun en başında, sayıyla yazılır; "young" kelimesi hiç kullanılmaz.

"Karanlık bir odada, tek başına, zor durumda biri" kombinasyonundan kaçınılır; 15.3'te bunu yaşadık.

Yeni filmde ana karakterler baştan açıkça yetişkin görünümlü tasarlanacak. Kyle'da yaşadığımız sorunların hiçbirini yeniden yaşamayalım.

#### Viral strateji: yeni filmi baştan bunun için tasarlamak

Raporun en değerli kısmı, viral olmanın kurguda değil yazım aşamasında başladığını göstermesi. Altı tasarım kararı öneriyorum:

Tek üretim, iki format. 16:9'luk bir karenin dikey (9:16) kesiti, karenin ortadaki yaklaşık üçte biri. Kuralımız şu olacak: önemli olan her şey (yüz, eylem, nesne) karenin orta üçte birinde. Böylece aynı klip hem filmde hem dikey bölümlerde kullanılır. Bu kurala uymayan birkaç geniş plan için kurguda kaydırarak kırpma yaparız.

Film, bölümlerden oluşacak. Senaryoyu baştan 60–90 saniyelik 15–20 bölüm olarak yaz. Her bölüm ilk 2 saniyede bir kancayla açılsın, bir uçurum sonuyla bitsin. Uzun versiyon bu bölümlerin birleşimi olur.

Platforma göre süre. YouTube Shorts için 20–45 saniyelik fragmanlar. TikTok'un ödül programı 60 saniyeden uzun videolar istiyor; bölümler oraya bu yüzden uygun.

Dürüst ve sade kapak. Karanlık, yüksek kontrastlı, tek odaklı. Kapakta gösterilen şey videonun ilk saniyelerinde gerçekten olmalı; aksi halde izleyici kaydırıp geçer ve algoritma videoyu gömer.

Etiket ve şeffaflık. YouTube'da gerçekçi AI içerik için "değiştirilmiş veya sentetik içerik" kutusunu işaretle, TikTok'ta AI etiketini aç ve dosyalardaki gömülü üst verileri silme. Ayrıca bir "nasıl yaptım" videosu çek: hem YouTube'un özgün olmayan içerik politikasına karşı insan emeğini gösterir, hem de en güvenilir izleyici kaynaklarından biridir.

İngilizce diyalog, Türkçe altyazı. Altyazıyı videoya göm; mobil izleyicinin çoğu sesi kapalı izliyor.

#### Lansman takvimi:

| Dönem | Ne yapılır |
|---|---|
| 1–2. hafta | Kısa merak uyandırıcı teaser'lar |
| 3. hafta | Fragman, ardından YouTube'da "İlk Gösterim" ile tam film |
| 4–8. hafta | İki günde bir dikey bölüm |
| 9. hafta | "Nasıl yaptım" videosu |

#### Yeni film önerisi

Raporlar korku türünün, öğretilebilir bir kuralın ve bulunmuş görüntü (found footage) formatının AI için en güçlü kombinasyon olduğunu söylüyor. Bulunmuş görüntü, AI'ın görsel pürüzlerini doğal hale getiriyor. Telefonla çekilmiş bir kayıt ise zaten dikey; yukarıdaki ikinci karar kendiliğinden çözülüyor.

Bu yüzden önerim, listedeki Arkana Bakma'yı bu formatla yeniden kurmak:

30'lu yaşlarında üç arkadaş, sisli bir ormandaki yürüyüşlerini telefonla kaydediyor. Peşlerindeki şey yalnızca biri dönüp arkasına baktığında bir adım yaklaşıyor. Kural, Stay in the Dark'taki gibi adım adım öğretiliyor ve her bölüm biri arkasına bakmak üzereyken bitiyor.

#### Bu format neden uygun?

Orman ve sis Omni'nin en güçlü olduğu görüntüler.

Telefon kaydı doğal olarak dikey.

"Dönüp bakma" anları ilk + son kare yöntemiyle hassasça kontrol edilebilir.

Diyaloglar İngilizce.

Şiddet yok; dehşet tamamen ima ve sesle kuruluyor.

Tek risk: el kamerası sarsıntısı yüz kaymasını artırabilir. Bunu "hafif el kamerası" tarifi ve kısa süreli yüz planlarıyla yönetiriz.

Yeni filmi bu fikirle mi kuralım, yoksa diğer fikirlerden birini bu yeni kurallarla yeniden mi şekillendirelim?

<!-- kaynak-bitiş -->
