# trex Cloud Deneme Programı – Öneri Dokümanı

## Amaç  
trex Cloud Deneme Programı, potansiyel müşterilerin herhangi bir yatırım yapmadan önce trex’in bulut tabanlı üretim veri toplama çözümünü sahalarında deneyimlemelerini sağlar.  
Bu program, donanım veya abonelik satın almadan önce müşterinin gerçek zamanlı veri toplama, hızlı kurulum ve OEE analizi deneyimini yaşamasına olanak tanır.

Not: trex Cloud markası, teknik olarak **NightWatch (veri toplama)** ve **EasyThings (bulut platformu)** altyapısı üzerine inşa edilmiş bir **rebranding çalışmasıdır**.  
Bu nedenle program, mevcut teknolojilerimizin yeni bir müşteri deneyimi ve satış modeliyle sunulmasını hedefler.

---

## Programın Temel Fikri  
trex Cloud Deneme Programı, 3 makineye kadar olan sahalarda kısa sürede veri toplamayı ve bu verileri bulutta görselleştirerek yatırım öncesi değer ispatı sunmayı amaçlar.  
Program sonunda müşteri, kendi makinelerinden gelen canlı verilerle sistemin sağladığı verimlilik ve görünürlük avantajlarını ölçümleyebilir.

**Ana hedef:** “Kurulumdan 1 saat sonra kendi makineni bulutta gör.”

---

## Katılım Koşulları  
- En fazla **3 makine/ekipman** dahil edilebilir.  
- Deneme yapılacak makineler trex Cloud’un desteklediği protokoller (OPC UA, Modbus, Fanuc, Nukon vb.) ile uyumlu olmalıdır.  
- Katılımcı firmada:  
  - Bir **Champion (teknik sorumlu)**  
  - Bir **Sponsor (yönetim/karar verici)** belirlenmelidir.  
- Deneme süresi ve kapsamı net tanımlanır (örneğin **30 gün**).  
- Deneme senaryosu başlangıçta **MES kapsamındaki OEE (Overall Equipment Effectiveness)** takibiyle sınırlıdır.  

---

## Program Akışı  
1. **Başvuru:**  
   Müşteri web sitesindeki formu doldurur ve başvuru trex ekibine iletilir.  
2. **Uyumluluk kontrolü:**  
   trex ekibi makine ve protokol uygunluğunu kontrol eder.  
3. **Deneme hesabı:**  
   Müşteri için trex Cloud (EasyThings) üzerinde özel bir tenant oluşturulur.  
4. **Veri toplama kurulumu:**  
   trex ekibi uzaktan erişimle müşterinin PC’sine **NightWatch veri toplama servislerini** kurar.  
5. **Görselleştirme:**  
   Kurulumdan sonra müşteri **web** veya **mobil uygulamadan** makine durumu, sayaç ve OEE metriklerini izlemeye başlar.  
6. **Süre:**  
   Ortalama kurulum süresi **yaklaşık 1 saattir.**  
7. **Opsiyonel donanım:**  
   - Eski nesil makineler için **trex IoT Box + Box PC** sağlanabilir.  
   - Sahada Andon ihtiyacı varsa **standart dashboard’lar** devreye alınabilir.  

---

## Deneme Sonrası Çıktılar  
Deneme sonunda müşteriye rapor veya kısa video anlatım ile aşağıdaki temel metrikler sunulur:  
- **Utilization (Makine Kullanım Oranı)**  
- **OEE (Overall Equipment Effectiveness)**  
- **Good Parts (Sağlam Ürün Sayısı)**  

Bu metrikler üzerinden müşteriyle birlikte iyileştirme fırsatları değerlendirilir.

---

## Bu Program Neden Önemli?  
- **Satın alma öncesi bariyeri kaldırır:** Müşteri, hiçbir yatırım yapmadan trex Cloud deneyimini yaşar.  
- **Gerçek saha geri bildirimi sağlar:** Kurulum, bağlantı ve performans adımları gerçek koşullarda test edilir.  
- **Rebranding doğrulaması:** trex Cloud markası, NightWatch + EasyThings altyapısının “plug & insight” yaklaşımıyla pazarda konumlanmasını test eder.  
- **Referans yaratır:** Başarılı denemeler, pazaryeri satışına geçişte ilk müşteri başarı hikâyeleri olarak kullanılabilir.  
- **Satış sonrası dönüşümleri hızlandırır:** Deneme → abonelik veya trex Cloud Box satışına yönlendirme kolaylaşır.

---

## Deneme Programı İçin Gereken İlave Çalışmalar

### 1. Web Sitesi ve Başvuru Süreci
- **trexcloud.com.tr** veya **cloud.trex.com.tr** altında özel bir tanıtım sayfası hazırlanmalı.  
- Sayfa içeriği:  
  - Program tanıtımı  
  - Katılım koşulları  
  - Görseller ve kısa açıklama videosu  
  - **Başvuru formu** (firma bilgileri, makine sayısı, iletişim kişisi vb.)  
- Başvuru sonrası otomatik e-posta bilgilendirmesi yapılmalı.

### 2. Operasyonel Yönergelerin Hazırlanması
- Operasyon ekipleri için adım adım dokümantasyon oluşturulmalı:  
  - **Deneme hesabı oluşturma ve tenant tanımlama**  
  - **Konfigürasyon hazırlama** (EasyThings/NightWatch servisleri)  
  - **Uzaktan erişim prosedürü** (VPN, AnyDesk, TeamViewer)  
  - **Veri toplama servislerinin kurulumu ve test adımları**  

### 3. Dashboard (Andon) Geliştirmeleri
- Deneme müşterilerinin ortak kullanabileceği **3 temel dashboard** geliştirilip standardize edilmeli:  
  1. **Makine Durumları (Çalışıyor/Duruyor/Arıza)**  
  2. **OEE Takip Ekranı**  
  3. **Üretim Sayacı & Fire Durumu**  
- Bu dashboard’lar mevcut EasyThings altyapısında kısmen mevcut; sadeleştirilerek herkes için erişilebilir hale getirilmeli.

---

## Sorumluluk Paylaşımı (Ekip Bazında)

| Ekip | Sorumluluk |
|------|-------------|
| **Yazılım Geliştirme** | Dashboard’ların tamamlanması, bulut hesap akışı, otomatik konfigürasyon sürecinin iyileştirilmesi |
| **Proje Ekibi** | Deneme müşterisi seçimi, saha iletişimi, kurulum takibi, sonuç raporlaması |
| **Elektronik Ekibi** | IoT Box + Box PC hazırlığı, bağlantı şeması ve donanım desteği |
| **Operasyon Ekibi** | Hesap oluşturma, uzaktan kurulum, servislerin devreye alınması |
| **CEO / Yönetim** | Programın duyurusu, satış sonrası modelin (abonelik/box satışı) onayı, fiyatlandırma stratejisi |

---

## Önerilen Yol Haritası

| Aşama | Süre | Açıklama |
|--------|------|----------|
| İçerik ve program yapısının onayı | 1 hafta | Tüm ekiplerle gözden geçirme |
| Web sayfası + başvuru formunun yayına alınması | 2 hafta | trexcloud.com.tr veya cloud.trex.com.tr altında |
| Operasyon yönergeleri ve dashboard geliştirmesi | 3 hafta | Paralel yürütülebilir |
| İlk pilot denemelerin başlatılması | 4. hafta | 2–3 pilot müşteri seçimi |
| Sonuç değerlendirmesi ve optimize edilmiş versiyon | 6. hafta | Pilot sonuçlarının analizi |

---

## Sonuç  
Bu program, trex Cloud markasının **NightWatch + EasyThings** altyapısı üzerinde gerçek saha doğrulamasını sağlayacak, aynı zamanda **pazaryeri satış öncesi düşük riskli bir müşteri kazanım modeli** olacaktır.  
Program, teknik olgunluk, kullanıcı deneyimi ve müşteri dönüşüm oranlarını ölçerek gelecekteki satış stratejisine sağlam bir temel oluşturur.
