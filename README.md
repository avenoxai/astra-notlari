# Astra Notları

GPT-6.2 Astra ve GPT-6.2 Sol testlerinin promptları ve sonuçları. Avenox kanalındaki GPT-6.2 videosu ve 17 Kasım 2026 canlı yayını için yapıldı. Hepsi Codex Desktop'ta çalıştı; promptlar Codex oturum kayıtlarından birebir alındı.

## Nasıl okunur

- `testler/`: videoda gösterilen testler. Her klasörde `README.md` (ne denendi, ayarlar, süre, sonuç), `prompt.md` (promptun kendisi ve takip mesajları) ve `sonuc/` (ekran görüntüleri, küçük çıktı dosyaları) var.
- `yayin-2026-11-17/`: canlı yayındaki testler, aynı düzende. Başında yayının kısa özeti var.
- Süreler Codex kaydındaki görev süresidir (`task_complete.duration_ms`). Saatler İstanbul saati.
- Büyük dosyalar (videolar, Blender projesi, 2 MB üstü HTML'ler) repoda yok; yerlerine ekran görüntüsü var. 2 MB altı tek dosyalık HTML demoları `sonuc/` içinde, çift tıklayıp açılabilir.
- Promptlar birebir; yalnız kişisel klasör yolları, kullanıcı adları ve kredi rakamları `[çıkarıldı]` ya da `~/` ile değiştirildi, tipografik tireler düz tireye çevrildi.

## Özet

| Test | Model | Efor | Tek prompt mu | Süre | Sonuç | Klasör |
|---|---|---|---|---|---|---|
| Satürn'ün İğnesi (Blender kısa film) | GPT-6.2 Astra | Extra High | Hayır, fikir sohbeti + 3 saatlik goal | 177,5 dk | 36 sn sesli film ve .blend proje | [testler/01](testler/01-saturnun-ignesi/) |
| Rize Çay Hattı (Three.js oyun, Higgsfield asset) | GPT-6.2 Astra | Max | Hayır, gece boyu goal | 389,4 dk | Oynanabilir sahne, 20 sn demo video | [testler/02](testler/02-rize-cay-hatti/) |
| Limon: SVG kodu ile görsel üretim | GPT-6.2 Astra | Extra High | Evet, iki ayrı sohbet | 12,4 / 15,8 dk | İki 30 sn animasyon | [testler/03](testler/03-limon-karsilastirmasi/) |
| Dünya simülasyonu | GPT-6.2 Sol, Ultra Fast | Medium | Evet | 48,0 sn | Tek HTML iklim simülasyonu | [testler/04](testler/04-sol-ultrafast/) |
| Hafıza oyunu, Computer ile | GPT-6.2 Sol, Ultra Fast | Medium | Evet | 35,4 sn (oyun 14 sn) | 8/8 çift, 13 hamle | [testler/04](testler/04-sol-ultrafast/) |
| Canlı yayın: 11 Astra testi + 1 Sol testi | GPT-6.2 Astra / Sol | Extra High | Evet | 2,8-32,0 dk | 10 hazır, 1 durduruldu | [yayin-2026-11-17](yayin-2026-11-17/) |

## Taha'nın videodaki tespitleri

Hepsi videonun dökümünden, Taha'nın kendi cümleleri.

- **Verimli ama zor model.** "Model inanılmaz verimli ama kullanması zor bir model. Yani tek prompta güzel sonuçlar alamıyorsun. Uğraşman gerekiyor." Verimlilik konusunda: "10 kat daha verimli diye 10 kat daha fazla kullanabileceğinizi düşünmeyin."
- **Tek promptta değil, uzun görevde.** "Bu model böyle tek promptta çok iyi sonuçlar alabileceğiniz model değil. Bu modelin olayı daha çok böyle uzun vadede çalıştığın, daha böyle matematik, fizik ağırlıklı işler." ve "Uzun görevleri otonom goal olarak vermekten çekinmemeniz gereken bir model."
- **Özel asset.** "Sadece kodla yaptığı işte kalite bir yere kadar olabiliyor." Rize testinde Higgsfield araçlarının kullanıldığını ayrıca belirtti.
- **Efor.** Astra için: "Medium da gayet iyidir." ve "en çok bence High'ı kullanın veya Medium'u kullanın. [...] Max'ın hiçbir anlamı yok." Sol için: "Solda mesela High, Extra High bu ikisi güzeldir."
- **Astra üstte, Sol altta.** "Astra'yı üste koyuyorsun gene altına sol agentları koyuyorsun. Gerçek işi aslında sol agentları yapıyor." ve "Astra yukarıda planı yapar, işin takibini yapar, genel resmi görür ve güzel bir vizyon koyar."
- **Paket.** "20 dolarlık paket kullanan arkadaşlar Astra'yı kullanmasın. [...] Solu kullansınlar." ve "100-200 dolarlık pakettekiler Astra ve Solu beraber kullanabilirler." Ultra Fast için: "şu an sadece 200 ve 500 dolarlık paketlerde var."

Not: Rize testi Max eforda çalıştı; efor tavsiyesi videoda bu testlerden sonra geliyor.
