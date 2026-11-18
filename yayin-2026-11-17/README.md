# Canlı yayın, 17 Kasım 2026: GPT-6.2 Astra testleri

Yayın sırasında Taha tek bir ana Codex sohbetini (GPT-6.2 Astra, Extra High) "patron" olarak kullandı. Ana sohbet, Taha'nın ya da sohbetteki izleyicilerin kısa isteklerini bir prompta çevirip her test için ayrı bir Codex sohbeti açtı. Bütün alt sohbetler GPT-6.2 Astra, Extra High; Taha'nın istediği gibi Fast hızında (kayıtta `priority`).

Taha'nın ana sohbete verdiği kural (birebir, kısaltılmış): "GPT Astra 6.2 modeline her biri ekstra high'da çalışsın. [...] Hep aynı modda çalışsın ki bir standart oluşsun. [...] Bir Astra modeli genel olarak yaratıcılığını görmek istediğimiz model. O yüzden verdiğim promptların çok detaylı olmaması lazım. Genel yaratıcılığına bırakmamız lazım, tamam mı? [...] Fast modunda yolla, hızlı çalışsın."

Ayrıca yayın sırasında ayrı bir sohbette GPT-6.2 Sol ile bir test yapıldı (12).

| # | Test | Model · efor | Süre | Sonuç | Repoda çalışan dosya |
|---|---|---|---|---|---|
| 01 | [Tek HTML FPS](01-fps/) | Astra · Extra High | 19,8 dk | Yayını yavaşlattığı için durduruldu, son test yarıda | Yok (4,5 MB) |
| 02 | [Parfüm simülasyonu](02-parfum/) | Astra · Extra High | 14,5 dk | Hazır: "Sillage" | [HTML](02-parfum/sonuc/sillage.html) |
| 03 | [2D robot savaşı](03-robot-savasi/) | Astra · Extra High | 15,0 dk | Hazır: "Çelik Raunt" | Yok (2,9 MB) |
| 04 | [Half-Life 3 fan bölümü](04-half-life-3/) | Astra · Extra High | 16,8 dk | Hazır: "Ters Gelgit" | Yok (3,1 MB) |
| 05 | [Kuantum parçacık hızlandırıcısı](05-parcacik-hizlandirici/) | Astra · Extra High | 13,5 dk | Hazır: "Fazlab" | [HTML](05-parcacik-hizlandirici/sonuc/fazlab.html) |
| 06 | [Dünya atmosferi](06-atmosfer/) | Astra · Extra High | 12,8 dk | Hazır: "Stratos" | Yok (2,5 MB) |
| 07 | [Evrenin dışı (SVG)](07-evrenin-disi-svg/) | Astra · Extra High | 5,7 dk | Hazır: "Gece Dokuması" | Yok (2,9 MB) |
| 08 | [Beyblade arenası](08-beyblade/) | Astra · Extra High | 14,4 dk | Hazır: "Ripcore" | Yok (çok dosyalı) |
| 09 | [Limon, SVG kodu](09-limon-svg-kod/) | Astra · Extra High | 12,4 dk | Hazır: "Otoportre", 30 sn | [SVG](09-limon-svg-kod/sonuc/limon.svg) |
| 10 | [Limon, görsel üretim](10-limon-gorsel/) | Astra · Extra High | 15,8 dk | Hazır: "Ayın Çalışanı", 30 sn | Yok (görseller büyük) |
| 11 | [Traffic Rider tarzı motosiklet](11-trafik-motosiklet/) | Astra · Extra High | 32,0 dk | Hazır: "Sunset Shift" | [HTML](11-trafik-motosiklet/sonuc/sunset-shift.html) |
| 12 | [Sol: voxel Limon sunumu](12-sol-voxel-limon/) | Sol · Extra High · Ultra Fast | 2,8 dk | Hazır | [HTML](12-sol-voxel-limon/sonuc/limon-voxel-sunumu.html) |

Süreler, her alt sohbetin kayıttaki ilk görev süresi (takip mesajlarının kısa turları hariç).

## Yayın sırasında bütün alt sohbetlere giden ortak mesajlar

Taha'nın "bu arada testlerini sessiz modda yapsınlar yayında gürültü oluyor ve benim bilgisayarımda çamasınlar headless açsınlar" isteği üzerine 22:21'de çalışan bütün sohbetlere şu mesaj gitti (birebir):

> Yayındaki operatörden test koşulu: Tüm doğrulamaları tamamen sessiz ve headless çalıştır. Görünür tarayıcı veya uygulama açma, kendi test penceren / ses oynatıcın açıksa kapat; yayıncının pencerelerine ve ses ayarına dokunma. Chromium/Playwright için headless:true ve --mute-audio kullan; ses testi gerekiyorsa çevrimdışı ses bağlamı veya ölçüm kullan, hoparlöre çalma. Oyunun kendi normal ses özelliklerini koru. İşin bittiyse yeniden kapsamlı test başlatma.

Sonra Taha "bu arada 2 taneyi durdur yayını kastırıyor" dedi; 01-fps'e "DUR" mesajı gitti (bkz. [01](01-fps/prompt.md)).

## Olmayanlar

- **Bulut denemesi:** Taha alt sohbetleri Codex Cloud'da açmak istedi. İki smoke testi gönderildi. Yayın klasöründeki notta: "Bulut erişim denemesinde araç Astra 6.2 + Extra High eşleşmesini doğrulayamadı. Yalnızca model adıyla yapılan denemede 15 dakikadan uzun bekleme sonunda oturum kimliği veya komut çıktısı alınamadı." Testler yerelde sürdü.
- **Hollow Knight:** Taha "hollow knight yaptırır mısın bu burada kalsın" dedi; başlatılmadı.
