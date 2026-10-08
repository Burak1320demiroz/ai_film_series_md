# Genel kurallar (eski sürüm)

> **[Derleyen notu]** Bu dosya `1.md`'nin ilk, 81 satırlık halinden alındı. O metin yeni `1.md`'de yok; bu klasör elde kalan tek kopyası. Kurallar sonraki sahnelerde geliştirildi; güncel kurallar için `Bolum_2_Kurulum/Sahne_07-10_Duzeltmeler_ve_Yeni_Kurallar.md` ve `Arastirma/03_...` dosyalarına bak.

- **Video:** Gemini Omni. Klipler 4, 6, 8 ya da 10 saniye.
- **Görsel (başlangıç kareleri):** GPT Image.

## Temel mantık

Sahne hikâyedeki bir bölüm, klip ise tek bir AI üretimi (en fazla 10 sn). Her klibin başlangıç karesi için iki tür işaret kullanılıyor:

- **YENİ:** Başlangıç karesini GPT Image'de, referanslarını vererek sıfırdan üretiyorsun. Yeni bir kamera açısı ya da yeni bir yer demek.
- **ZİNCİR ← X:** Başlangıç karesi, X klibinin son karesi. Aynı hareket kesintisiz devam ediyor.

Zincirlerin hepsini peş peşe dizmedim. Araya başka açılar girip sonra zincire geri dönebiliyoruz, filmlerde kesme zaten böyle çalışır. Örneğin 2.2'den sonra 2.3'te sokağın öbür ucuna kesiyoruz, 2.4 ise 2.2'nin son karesinden devam ediyor.

## Üretim akışı

Her klip için önce GPT Image'e başlangıç karesini ürettireceksin, sonra o kareyi Omni'ye verip videoyu üreteceksin.

**16:9 kırpma:** GPT Image yatay görselleri genelde 3:2 oranında üretiyor, film ise 16:9. Görseli Omni'ye vermeden önce 16:9'a kırpman gerekebilir. Promptlara önemli öğeleri kadrajın üst ve alt kenarından uzak tutma talimatını bu yüzden ekledim, kırpınca bir şey kaybolmasın.

Her klip için 2–3 deneme üretip en iyisini seç.

## Zincirleme için kurallar

1. **Zincir 3 klibi geçmesin.** Her üretimde yüz ve detaylar biraz kayıyor, kayma da birikiyor. Plandaki en uzun zincir bu yüzden 3 klip (2.1 → 2.2 → 2.4, 2.3 → 4.1 → 4.3, 3.1 → 3.2 → 3.5). 4.4'ü de bilerek YENİ yaptım, yoksa Marco'nun zinciri 5 klibe çıkıyordu.
2. **Zincirli kliplerde de karakter referansını ver.** Son kareyi başlangıç karesi yap, karakter sayfasını da referans slotuna koy. Böylece yüz kayması büyük ölçüde azalır.
3. **Zincire devredecek klibi sakin bir anda bitir.** Video promptuna "klip, Marco motorun üstünde hareketsiz otururken biter" gibi bir cümle ekle. Hareket bulanıklığı olan bir son kare, devam klibini de bozar.
4. **Son kareyi temiz al.** Kurgu programından dışa aktarabilirsin ya da şu komutu kullanabilirsin:

   ```bash
   ffmpeg -sseof -0.5 -i klip_2-1.mp4 -update 1 -q:v 1 klip_2-1_son.png
   ```

   Son kare bulanıksa birkaç kare öncesindeki net bir kareyi al ve kurguda klibi o noktadan kes.
5. **Ortam sesini tek parça döşe.** Omni her klibe kendi ortam sesini üretir ve zincir noktalarında ses "zıplar". Rüzgârı, uzak sirenleri ve şehir uğultusunu kurguda kesintisiz tek bir katman olarak koy, Omni'nin ortam sesini kıs. Efektleri ve çığlıkları klipten alırsın.
