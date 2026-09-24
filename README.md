## Hi there 👋
### ✈️ Havacılık MRO Sektörü İçin Tamir Edilebilir Yedek Parça Envanter Karar Destek Sistemi
*Kurumsal gizlilik prensipleri gereği operasyonel veri setleri ve kaynak kodlar gizli tutulmaktadır.*

#### 📌 Problem Tanımı & Mevcut Durum
* **Operasyonel Riskler:** Faal stok eksikliği ve tamirden dönüş gecikmelerinin uçak bakım sürelerinde aksamalara ve hat duruşlarına yol açması.
* **Maliyet Baskısı:** Faal stok yetersizliğinden kaynaklanan yüksek maliyetli acil parça alımları ve gayri faal stok birikimi nedeniyle oluşan atıl sermaye yükü.
* **Mevcut Planlama Kısıtları:** İç ve dış tamir döngülerinin bütünleşik bir sistem yerine büyük ölçüde uzman tecrübesine dayalı yönetilmesi.

---

#### ⚙️ Sistem Mimarisi & Metot
* **Ayrıştırılmış Tamir Döngüleri:**
  * **İç Tamir (Şirket İçi Atölyeler):** Talep, iç tamir ve tedarik süreleri analiz edilerek kurgulanan *Aylık Envanter Modeli*, *İş Emri Oluşturma* ve *Atölye/Kapasite Atama Modelleri*.
  * **Dış Tamir (Yurt Dışı Atölyeler):** Uzun tedarik ve lojistik süreleri dikkate alınarak geliştirilen çift eşikli stok kontrol politikaları (`rrQQ / (r, Q)` algoritmaları).
* **Teknik Altyapı:**
  * **Arka Uç (Python):** Güvenlik stoğu hesaplamaları, yeniden sipariş seviyeleri ve çok parametreli optimizasyon motoru.
  * **Ön Yüz & Karar Destek Arayüzü:** Planlamacıların atölye kapasitelerini, sipariş tetikleyicilerini ve acil alım risklerini simüle edip senaryo analizleri yapabileceği interaktif web paneli.

---

#### 🎯 Kazanımlar
* Parça arızaları, satın alma ve tamir süreçleri arasındaki bağıntıyı dinamik olarak modelleme,
* Acil tedarik maliyetlerini ve hareketsiz stok birikimini en aza indirme,
* Hedeflenen uçak servis seviyesini minimum toplam envanter maliyetiyle güvenceye alma.
