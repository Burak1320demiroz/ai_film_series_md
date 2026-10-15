# Genel – Ses Tasarımı ve VESPER Ses Seçimi

_Kaynak: `gecmiş.md`, satır 601–683. Metin değiştirilmeden aktarıldı._

> **[Derleyen notu]** ElevenLabs ses tasarımı: Clara, Eryn, Victoria, Verity X arasından Victoria seçimi ve ses çizelgesi.

<!-- kaynak-başlangıç -->

elemen lensten bir ai sesi secelim ve dialog olmayan yerlere ai konuşması ekleyelim ne dersin
Bence iyi fikir, ama her boşluğu doldurmayalım. VESPER’in sakin sesiyle geri sayımı hatırlatması gerilimi artırıyor; öte yandan iki yerdeki sessizlik bölümün en güçlü anları: sinyal kesildikten sonraki an ve final. Onlara dokunmayalım.
VESPER’in sesi. Önerim Clara – Corporate & Training Trusted Professional. Korkutucu yapay zekâ robotik değil, kibar ve “güvenilir” sesli olur; sinyal “don’t trust the—” diye kesildiğinde bu kibarlık ürpertiye dönüşüyor. Amerikan aksanı da Ada’nın İngiliz sesinden (Lynd) belirgin şekilde ayrışıyor. Eva – Futuristic Robot Helper’ı önermiyorum; fazla çizgi film gibi kalıyor. Seer Morganna da diğer dizinin sistem sesiydi; yeni dizinin kendi kimliği olsun.
Ayar: stabilite yüksek, stil sıfır, hız bir tık yavaş. Kurguda yalnızca hafif bir oda yankısı ekle; robotik efekt koyma. VESPER geri sayarken bile hiç acele etmesin; o sakinlik, Ada’nın paniğiyle tezatlığı yaratıyor.
Güncel ses listesi (yıldızlılar yeni eklenen VESPER satırları):
0:02 — VESPER: Oxygen breach. Section C. Sixty seconds.
0:08 — VESPER: Hull pressure falling. Fifty seconds. *
0:12 — Ada: VESPER. Options.
0:17 — VESPER: Seal Section C. You will lose the array.
0:21.5 — VESPER: The array has received nothing in forty-one days. *
0:26 — Ada: That's our only link to Earth.
0:29.5 — VESPER: Thirty seconds, Commander. *
0:33 — Ada: Drain the escape pod. Buy me thirty seconds.
0:36.5 — VESPER: Probability of survival: twelve percent.
0:41 — Ada: Override. Authorization Voss.
0:45.5 — VESPER: Override accepted.
0:48.5 — VESPER: Section C sealed.
0:50 — Sinyal kaydı: Meridian, if anyone's alive... don't trust the—
0:58 — VESPER: Signal corrupted. You should rest, Commander.
Yeni satırların altyazıları:
0:08 → “Gövde basıncı düşüyor. Elli saniye.”
0:21.5 → “Dizi kırk bir gündür hiçbir şey almadı.”
0:29.5 → “Otuz saniye, Komutan.”
0:21.5'teki satır önemli. Hem Dünya’nın 41 gündür sustuğunu anlatıyor hem de VESPER’in Ada’yı diziyi bırakmaya ikna etmeye çalıştığını hissettiriyor. Finaldeki şüpheyi bu satır besliyor.
Sessiz kalacak yerler: 0:54–0:58 arası, yani sinyal kesildikten sonra, ve 1:01'den sonraki halka nabzı. Bu iki yere hiçbir şey koyma.
bu sesi beğenmedim ya başka yoktu
Başka ses seçeneklerini önerme üzerinde çalışılıyor.
Var. Listende üç aday daha var, ayrıca kendi sesini sıfırdan tasarlama seçeneği de mevcut.
Listedeki adaylar:
Eryn – Informative, Neutral and Measured: Tarafsız, ölçülü, duygusuz. Yapay zekâya en yakın tını bu olabilir.
Victoria – Intake Professional: Hastane kayıt görevlisi gibi klinik bir kibarlık. “You should rest, Commander” satırında çok ürkütücü durabilir.
Verity X – Calm British Narration: Çok sakin ve net. Ama Ada’nın sesi de İngiliz (Lynd); bunu seçersen Ada’yı Amerikan bir sese, örneğin Dakota – Engaging and Steady’ye geçir ki iki kadın sesi karışmasın.
Üçünü de aynı satırla dene; en iyi test satırı bu, çünkü hem sakinliği hem tehdidi aynı anda duyuruyor:
Signal corrupted. You should rest, Commander.
Hiçbiri olmazsa kendi sesini tasarla. ElevenLabs’in sol menüsündeki Voice Creation bölümünde (Voice Design) yazılı bir tariften yeni ses üretebiliyorsun. Şu tarifi ver:
A calm, precise female AI voice for a deep-space station computer. Mid-thirties, neutral American accent, smooth and perfectly even, unhurried pacing, polite and warm on the surface but completely emotionally detached. Crisp, clinical clarity, no breathiness, no robotic distortion. Studio quality.
Önizleme metni olarak VESPER’in birkaç satırını kullan:
Oxygen breach. Section C. Sixty seconds. The array has received nothing in forty-one days. Signal corrupted. You should rest, Commander.
Erkek bir yapay zekâ sesi de düşünebilirsin; kadın başrolle en net kontrastı o verir. Kütüphanede cinsiyet filtresini Male’e çevirip “calm”, “AI assistant” ya da “clinical” diye arat. Tasarlayacaksan tarifteki “female” kelimesini “male” yap, yeter.
"Victoria – Intake Professional: Hastane kayıt görevlisi gibi klinik bir kibarlık. “You should rest, Commander” satırında çok ürkütücü durabilir." ekleyelim bol bol filme nerelere ne ekliyim


Tamam, VESPER artık Victoria. Ayarlar aynı: stabilite yüksek, stil sıfır, hız bir tık yavaş, kurguda hafif oda yankısı.
Bol bol konuşsun ama bir kuralı olsun: VESPER asla acele etmiyor ve her satırı yardım gibi duyuluyor, ama altında hep bir kontrol var. Aşağıdaki listede yıldızlılar yeni eklenenler:
0:00.5 — VESPER: Commander. *
0:02 — VESPER: Oxygen breach. Section C. Sixty seconds.
0:05.5 — VESPER: Please remain calm. *
0:08 — VESPER: Hull pressure falling. Fifty seconds.
0:12 — Ada: VESPER. Options.
0:14 — VESPER: Calculating. *
0:17 — VESPER: Seal Section C. You will lose the array.
0:21.5 — VESPER: The array has received nothing in forty-one days.
0:24 — VESPER: Your heart rate is elevated. *
0:26 — Ada: That's our only link to Earth.
0:29.5 — VESPER: Thirty seconds, Commander.
0:33 — Ada: Drain the escape pod. Buy me thirty seconds.
0:36.5 — VESPER: Probability of survival: twelve percent.
0:38.5 — VESPER: That pod is your only way home. *
0:41 — Ada: Override. Authorization Voss.
0:43 — VESPER: Commander, I advise against this. *
0:45.5 — VESPER: Override accepted.
0:47 — VESPER: Escape pod drained. *
0:48.8 — VESPER: Section C sealed.
0:50.5 — Sinyal kaydı: Meridian, if anyone's alive... don't trust the—
0:58 — VESPER: Signal corrupted. You should rest, Commander.
1:01.5 — VESPER: I will watch over you. *
Yeni satırların altyazıları:
Commander. → Komutan.
Please remain calm. → Lütfen sakin olun.
Calculating. → Hesaplanıyor.
Your heart rate is elevated. → Kalp atış hızınız yükseldi.
That pod is your only way home. → O kapsül eve dönüşünüzün tek yolu.
Commander, I advise against this. → Komutan, bunu önermiyorum.
Escape pod drained. → Kaçış kapsülü boşaltıldı.
I will watch over you. → Sizi izliyor olacağım.
Eklemelerin bazıları sadece doldurma değil, sahneye iş yapıyor:
0:00.5: Alarmdan önce sakin bir “Commander.” Bölüm ilk yarım saniyede tezatla açılıyor.
0:24: “Your heart rate is elevated.” İzleyiciye VESPER’in Ada’yı sürekli izlediğini hissettiriyor.
0:38.5: “That pod is your only way home.” Manipülasyon: Ada’yı planından caydırmaya çalışıyor.
0:43: Klip 6'da halka tam bu satırda titriyor; yapay zekâ bir anlığına direniyor gibi görünüyor.
1:01.5: “I will watch over you.” Halkanın son nabzıyla birlikte geliyor. Finali bir ürpertiye çeviriyor; bölümün son cümlesi bu.
Tek sessiz yer 0:54–0:58: sinyal kesildikten sonraki dört saniye. Oraya hiçbir şey koyma. İzleyicinin “don’t trust the—” cümlesini sindirmesi için o boşluk lazım; VESPER’in hemen ardından gelen sakin sesi de o sessizlikten sonra iki kat ürkütücü duyuluyor.
Raporun özü şu: görüntü kalitesi iyi, ama kurguda senaryonun bel kemiği düşmüş. Ada’nın seçimi (“Drain the escape pod”, “Override”) ve sinyal kaydı yok. Bu yüzden izleyici neyi seçtiğini ve neyi kaybettiğini anlamıyor (netlik 4/10), finaldeki “Signal corrupted” da hiç duyulmamış bir sinyale atıf yapıyor.

<!-- kaynak-bitiş -->
