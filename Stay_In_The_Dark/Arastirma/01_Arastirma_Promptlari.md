# Derin araştırma promptları (4 adet)

_Kaynak: `1.md`, satır 2585–2684. Metin değiştirilmeden aktarıldı._

> **[Derleyen notu]** Bu promptları isteyen kullanıcı mesajı kaynakta yok.

<!-- kaynak-başlangıç -->

Dört promptu birbirini tamamlayacak şekilde ayırdım; her biri farklı bir alanı kazıyor:

Gemini Omni: Video modelinin bütün yetenekleri, sınırları ve filtreleri.

GPT Image: Referans ve başlangıç karesi üretiminde en iyi yöntemler.

AI film zanaatı: Senaryo, sahne kurgusu, geçişler, ses ve kurgu.

Viral AI videolar: Neyin neden yayıldığı ve dağıtım stratejisi.

Her promptun içine bizim projede yaşadığımız sorunları da yazdım (yüz kayması, filtre engelleri, ölü zaman, dudak senkronu). Böylece araştırma genel bilgiyle yetinmeyip doğrudan bizim derdimize çözüm arayacak.

Promptları Türkçe yazdım, ama araştırmanın ağırlıklı olarak İngilizce kaynaklarda yapılmasını istedim; bu alandaki kaynakların çoğu İngilizce. Raporlar Türkçe gelecek. Her birini ayrı bir derin araştırma oturumunda çalıştır.

### 1. Gemini Omni

```text
Bugünün tarihi Ekim 2026. Bağımsız bir içerik üreticisiyim. Google'ın Gemini Omni video modeliyle (image-to-video, 4/6/8/10 saniyelik klipler) ve GPT Image ile üretilen başlangıç kareleriyle 30 dakikalık bir AI korku filmi tamamladım. Şimdi yeni bir film yapacağım ve Gemini Omni'yi derinlemesine anlamak istiyorum.

Araştırmayı ağırlıklı olarak İngilizce kaynaklarda yap: Google'ın resmi dokümanları ve blog yazıları, Gemini API / AI Studio / Vertex AI dokümantasyonu, geliştirici forumları, Reddit ve Discord toplulukları, deneyimli üreticilerin YouTube eğitimleri ve karşılaştırma testleri. Mayıs 2026'daki lansmandan sonraki bilgilere öncelik ver ve her bilginin tarihini belirt. Resmi bilgiyi, topluluk deneyimini ve söylentiyi birbirinden ayır.

Cevaplamanı istediğim sorular:
1. Sürümler ve erişim: Hangi Omni sürümleri var (Flash, Pro vb.)? Gemini uygulaması, API, Vertex AI, YouTube Create ve üçüncü taraf platformlar arasında özellik, kalite, fiyat ve kullanım limiti farkları neler?
2. Teknik özellikler: Desteklenen süreler, çözünürlükler (720p / 1080p / 4K iddiaları), en-boy oranları, kare hızı. Referans görsel sayısı ve ağırlığı. Başlangıç karesinin yanında bitiş karesi (first + last frame) verilebiliyor mu? Video uzatma, sohbetle düzenleme, karakter ve ses profili kimlikleri nasıl çalışıyor?
3. Ses: Diyalog, ses efekti ve ortam sesi üretimi ne kadar iyi? Aynı karakterin sesi klipler arasında nasıl tutarlı tutulur? Ses referansı verilebiliyor mu? Dudak senkronunun güçlü ve zayıf yanları neler?
4. Prompt yazımı: Resmi prompt rehberi ne öneriyor? Kamera dili, zamanlama ifadeleri ("0–2s") ve ses tarifleri nasıl yazılmalı? Negatif ifadeler işe yarıyor mu? Çalıştığı kanıtlanmış örnek promptlar topla.
5. Tutarlılık: Yüz, kıyafet ve nesne tutarlılığı için en iyi yöntemler. Son kareden devam eden zincirlerde yüz kayması neden oluyor ve nasıl azaltılır?
6. Bilinen hatalar ve çözümleri: Klip başında ve sonunda replik öncesi bekleme (ölü zaman), uç yüz ifadelerinde deformasyon, kalabalıkların yapay hareketi (tırmanma, üst üste binme), ışığın abartılı huzmelere dönüşmesi, nesnelerin şekil değiştirmesi, yazı bozulması.
7. Güvenlik filtreleri: Hangi içerikler engelleniyor (genç görünen karakterler, şiddet, gerçek kişiler, telif)? Yetişkin bir karakter yanlışlıkla reşit olmayan biri sanıldığında üreticiler bunu meşru yollarla nasıl çözüyor? SynthID ve içerik politikası ne diyor?
8. Karşılaştırma: Omni; Veo, Kling, Seedance, Runway ve diğer güncel modellere göre hangi işlerde daha iyi, hangilerinde daha zayıf? Hangi sahne türü için hangi model?

Çıktı formatı (Türkçe, teknik terimlerin İngilizcesi parantez içinde):
- Kısa yönetici özeti
- Teknik özellikler ve limitler tablosu
- "Omni için prompt şablonu": görsel, kamera, hareket, ses ve diyalog bölümleriyle
- Bilinen hatalar ve çözümleri tablosu (hata | sebep | çözüm | kaynak)
- Filtrelerle ilgili pratik kontrol listesi
- Model karşılaştırma tablosu
- Bütün iddialar için tarihli kaynak bağlantıları; emin olunamayan bilgiler açıkça işaretlenmiş
```

### 2. GPT Image

```text
Bugünün tarihi Ekim 2026. AI film yapıyorum: karakter, mekân ve nesne referanslarını ve her klibin başlangıç karesini OpenAI'nin GPT Image modeliyle üretip Gemini Omni'ye image-to-video olarak veriyorum. Yeni filmimden önce GPT Image'i bu iş akışı için en verimli şekilde kullanmayı öğrenmek istiyorum.

Araştırmayı ağırlıklı olarak İngilizce kaynaklarda yap: OpenAI'nin resmi dokümanları, API referansı ve kullanım politikaları, OpenAI Cookbook, geliştirici forumları, Reddit toplulukları ve deneyimli AI film üreticilerinin eğitimleri. 2025–2026 bilgilerine öncelik ver ve tarihlerini belirt.

Cevaplamanı istediğim sorular:
1. Güncel sürümler ve erişim: Hangi GPT Image sürümleri var? ChatGPT ile API arasındaki farklar, desteklenen boyutlar ve en-boy oranları (16:9 doğrudan destekleniyor mu?), kalite ayarları, bir istekte kaç referans görsel verilebildiği.
2. Düzenleme: Maskeli ve maskesiz düzenleme (inpainting), çok adımlı düzenlemelerde yüzün ve kompozisyonun korunması. Onaylanmış bir karede yalnızca bir şeyi (bir nesne, bakış yönü, eldeki bir eşya) değiştirmenin en güvenilir yolu.
3. Karakter tutarlılığı: Karakter sayfası (character sheet / turnaround) için en iyi düzen. Aynı yüzü onlarca farklı sahnede korumanın yöntemleri. Referans görsellerin sırası ve sayısı sonucu nasıl etkiliyor?
4. Video modelleri için başlangıç karesi: Bir image-to-video modeline verilecek karede nelere dikkat edilmeli (hareket için boş alan, kenarlardan uzak öğeler, ışık ipuçları, tam profilden kaçınma)? Başlangıç karesindeki seçimler videonun kalitesini nasıl etkiliyor?
5. Yazı üretimi: Poster, başlık kartı ve ekran yazıları ne kadar güvenilir? Harf hatalarını düzeltmenin yolları.
6. Güvenlik filtreleri: Hangi durumlar reddediliyor? "Other" gibi belirsiz kategorilerle gelen retlerin bilinen sebepleri neler (karakterin yaşının belirsiz görünmesi, sıkıntı içindeki biri, şiddet, gerçek kişiler, telif)? Meşru içerik yanlışlıkla engellendiğinde, bağlamı ve yetişkinliği netleştirmek gibi politikaya uygun hangi yöntemler kullanılıyor?
7. Alternatifler: Gemini'nin görsel modeli (Nano Banana), Midjourney, Flux Kontext, Ideogram, Seedream gibi modellerle karşılaştırma. Referans üretimi, düzenleme ve yazı için hangisi ne zaman daha iyi?

Çıktı formatı (Türkçe, teknik terimlerin İngilizcesi parantez içinde):
- Kısa yönetici özeti
- Özellikler ve limitler tablosu
- Hazır prompt şablonları: karakter sayfası, mekân referansı, nesne referansı, başlangıç karesi, düzenleme isteği, poster ve küçük resim (thumbnail)
- "Başlangıç karesi kontrol listesi"
- Filtre retleri ve meşru çözümler tablosu
- Model karşılaştırma tablosu
- Tarihli kaynak bağlantıları; emin olunamayan bilgiler açıkça işaretlenmiş
```

### 3. AI film zanaatı

```text
Bugünün tarihi Ekim 2026. 4–10 saniyelik AI video klipleriyle 30 dakikalık kısa filmler yapıyorum. İlk filmimde öğrendiğim temel ilkeler: az karakter ve az mekân, seyirciye adım adım öğretilen net bir kural, tutarsızlıkları gizleyen bir atmosfer (karanlık, sis), son kareden devam eden klip zincirleri ve sesle anlatılan şiddet. Şimdi bu zanaatı profesyonel seviyeye taşımak istiyorum.

Araştırmayı ağırlıklı olarak İngilizce kaynaklarda yap: AI film festivalleri ve kazanan filmler (örneğin Runway'in AI Film Festival'i ve benzerleri), tanınmış AI film yapımcılarının yapım günlükleri ve röportajları, sinema dergileri, kurgu ve ses tasarımı eğitimleri, topluluk forumları. 2025–2026'ya öncelik ver.

Cevaplamanı istediğim sorular:
1. Hikâye ve senaryo: Başarılı AI kısa filmleri hikâyelerini teknolojinin sınırlarına göre nasıl kuruyor? Hangi türler ve yapılar AI'ya en uygun? Örnek filmler ve neden çalıştıkları.
2. Senaryodan çekim listesine: 4–10 saniyelik klipler için senaryo ve çekim listesi (shot list) formatları. Sahne başına klip sayısı, ortalama plan süresi ve tempo.
3. Geçişler: Eşleşme kesmesi (match cut), son kare / ilk kare zincirleme, J ve L kesmeleri, ses köprüleri, ışık ve flaş geçişleri, morph geçişleri. Hangi geçişler AI hatalarını gizler, hangileri açığa çıkarır? Modellerin ilk kare + son kare özelliklerinin geçişlerde kullanımı.
4. Tutarlılık iş akışları: Karakter ve nesne takibi, "yapım kutsal kitabı" (production bible) düzeni, renk düzeltme ve LUT ile görsel birlik, büyütme (upscaling), kare ara değerleme, kumlanma (grain) ve gürültü azaltma araçları.
5. Diyalog: Modelin kendi ürettiği ses ile sonradan seslendirme ve dublaj karşılaştırması, dudak senkronu araçları, çok dilli versiyonlar.
6. Ses tasarımı ve müzik: Sessizliğin ve ses katmanlarının kullanımı. AI müzik araçlarının lisans ve telif durumu, güvenli ses kütüphaneleri.
7. Kurgu: AI kliplerle çalışırken DaVinci Resolve, Premiere ve CapCut iş akışları; kırpma ve tempo kuralları.
8. "AI işi" görünümü: Bir filmi ucuz AI içeriği gibi gösteren en yaygın hatalar ve profesyonellerin bunları nasıl önlediği.

Çıktı formatı (Türkçe, teknik terimlerin İngilizcesi parantez içinde):
- Kısa yönetici özeti
- Örnek filmler tablosu (film | yapımcı | süre | araçlar | neden başarılı | bağlantı)
- Adım adım bir AI kısa film iş akışı (fikirden dışa aktarıma)
- Geçiş türleri tablosu (geçiş | ne zaman kullanılır | AI hatalarını gizler mi | nasıl yapılır)
- "AI işi görünmeme" kontrol listesi
- Önerilen araçlar listesi (fiyat ve lisans notlarıyla)
- Tarihli kaynak bağlantıları
```

### 4. Viral AI videolar ve dağıtım

```text
Bugünün tarihi Ekim 2026. Türkiye'de yaşayan bağımsız bir AI film üreticisiyim. 30 dakikalık bir AI korku filmini tamamladım; filmin diyalogları İngilizce, Türkçe altyazılı. Bir sonraki filmimi baştan viral olacak şekilde tasarlamak ve dağıtmak istiyorum.

Araştırmayı İngilizce ve Türkçe kaynaklarda yap: platformların resmi yaratıcı rehberleri ve politika sayfaları, sosyal medya analiz raporları, teknoloji ve medya haberleri, viral olmuş içerik üreticilerinin röportajları ve vaka analizleri. 2024–2026 dönemine odaklan ve her rakamın kaynağını ve tarihini belirt.

Cevaplamanı istediğim sorular:
1. Vaka analizleri: 2024–2026 arasında viral olmuş AI filmleri, kısa filmler, sahte fragmanlar, diziler ve kısa formatlı AI videolar. Her biri için platform, izlenme, süre, kullanılan araçlar ve neden yayıldığı.
2. Platformlar: YouTube (uzun video ve Shorts), TikTok, Instagram Reels ve X'te algoritmanın neyi ödüllendirdiği (izlenme süresi, ilk 2–3 saniyedeki kanca, tekrar izleme, döngü). İdeal süreler ve paylaşım sıklığı.
3. Türler ve formatlar: AI içerikte en iyi performans gösteren türler ve kancalar (korku, bilim kurgu, "ya şöyle olsaydı" senaryoları, bölümlük dikey mikro diziler). Uzun bir filmin kısa bölümlere ve dikey kesitlere dönüştürülmesi.
4. Kapak ve başlık: Küçük resim ve başlık için kanıtlanmış en iyi uygulamalar.
5. İzleyici tepkisi: İzleyicilerin AI içeriğe yaklaşımı, tepki ve eleştiri örnekleri, "AI çöpü" algısından kaçınmanın yolları.
6. Kurallar: YouTube, TikTok ve Meta'nın AI içerik etiketleme zorunlulukları; YouTube'un "özgün olmayan ve seri üretilmiş içerik" politikası ve para kazanma kuralları; AB Yapay Zekâ Yasası'nın şeffaflık hükümleri; AI içerikte telif riskleri.
7. Gelir modelleri: Reklam geliri, marka iş birlikleri, festivaller, Patreon ve benzeri platformlar, yayın platformlarına lisanslama.
8. Türkiye pazarı: Türk AI içerik üreticileri, Türkçe AI filmler ve diziler, yerel trendler. Türk izleyici için altyazı mı dublaj mı, İngilizce içerik mi Türkçe içerik mi?

Çıktı formatı (Türkçe):
- Kısa yönetici özeti
- Vaka analizleri tablosu (başlık | üretici | platform | izlenme | süre | araçlar | neden viral oldu | bağlantı)
- Platform bazlı strateji rehberi
- "Viral AI filmi" tasarım kontrol listesi: fikir, kanca, format, süre, kapak
- 30 dakikalık bir film için örnek bir lansman planı (fragman, teaser, dikey kesitler, bölümlere ayırma, takvim)
- Kurallar ve riskler tablosu
- Tarihli kaynak bağlantıları; doğrulanamayan rakamlar açıkça işaretlenmiş
```

#### Sonrası

Dört rapor geldiğinde bunları tek bir "yapım rehberi"nde birleştiririm. İçinde yeni modelleri ve kuralları içeren güncel prompt şablonları ile viral olma ihtimali en yüksek film fikri ve formatı olur. Hangi filmi yapacağımıza da o zaman, verilere dayanarak karar veririz.

<!-- kaynak-bitiş -->
