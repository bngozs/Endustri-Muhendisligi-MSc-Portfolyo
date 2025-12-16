# Endustri-Muhendisligi-MSc-Portfolyo
Endüstri Mühendisliği Yüksek Lisans eğitimi boyunca gerçekleştirdiğim simülasyon, optimizasyon ve veri analizi projelerini içermektedir.

#### 📂 Çamaşır Makinesi Simülasyon Projesi Dosya Yapısı ve İçerik
**Kullanılan Araçlar:** Rockwell Arena Simulation 
Bu çalışma, beyaz eşya sektöründeki bir üretim hattının verimliliğini artırmak amacıyla "Ayrık Olaylı Simülasyon" tekniği ile gerçekleştirilmiş bir optimizasyon ve veri analizi projesidir.

#### Problem Tanımı
Mevcut çamaşır makinesi üretim hattında oluşan aşırı kuyruklar ve yüksek teslimat süreleri (Lead Time) nedeniyle müşteri taleplerinin karşılanmasında yaşanan aksaklıkların giderilmesi hedeflenmiştir.

#### Model Yapısı
Model, stokastik süreçlerin (rastgele varış ve işlem süreleri) analizine dayanmaktadır:
Varlıklar (Entities): Tambur ve Gövde üniteleri 
Kaynaklar (Resources): Montaj Presi, Elektrik Montaj ve Test İstasyonları 
Kısıtlar: Darboğaz oluşturan makine kapasiteleri ve vardiya düzeni 

#### Analiz Sonuçları
İyileştirme: Darboğaz istasyonlarında kapasite artırımı ve Kaizen teknikleri uygulanarak üretim miktarı %16,5 artırılmıştır.
Verimlilik: Sistemde geçen ortalama süre 1.111 dakikadan 37 dakikaya düşürülerek katma değersiz zamanlar (Non-Value Added Time) elimine edilmiştir.
Doğrulama: Sonuçların anlamlılığı %95 Güven Aralığı ile istatistiksel olarak kanıtlanmıştır.

#### 📂 Dosya İçeriği
* **`Mevcut Sistem/`**: İyileştirme öncesi durumun analiz dosyaları.
  * `Model/`: Arena (.doe) modeli.
  * `Sonuc/`: Simülasyon çıktı raporları (.out).
* **`Dengelenmis Sistem/`**: Kapasite artırımı ve Kaizen uygulanan iyileştirilmiş durum.
  * `Model/`: Optimize edilmiş Arena (.doe) modeli.
  * `Sonuc/`: İyileştirilmiş çıktı raporları.
* **`Rapor/`**: Projenin detaylı akademik raporu.

* ---

### 2. 📂 Sistem Dinamiği - iThink Projesi Dosya Yapısı ve İçerik
**Kullanılan Araçlar:** iThink / STELLA
Bu çalışma, bilişsel psikolojideki öğrenme ve unutma süreçlerini "stok ve akış" diyagramları ile modelleyen bir sistem dinamiği projesidir.

#### 🧠 Problem Tanımı
Victor isimli bir dinleyicinin, İtalyan operası aryalarını dinlerken kelimeleri hafızasına alma (öğrenme) ve zamanla unutma dinamikleri arasındaki ilişki incelenmiştir.

#### ⚙️ Model Yapısı
Model, "Birinci Dereceden Negatif Geri Besleme" (First Order Negative Feedback) yapısına sahiptir:
* **Stok:** Hafızadaki Kelime Sayısı 
* **Giriş:** Ezberleme Hızı (Şarkı Temposu) 
* **Çıkış:** Unutma Hızı (Zaman Sabiti ile ters orantılı) 

#### 📊 Analiz Sonuçları
* **Denge Durumu:** Sistem, 90 saniyelik bir zaman sabiti ile dengeye ulaşmakta ve hafızada maksimum 45 kelime tutulabilmektedir.
* **Senaryo Analizi:** Hızlı müzik senaryosunda giriş hızı arttığında, denge noktası yükselmekte ancak sistemsel davranış korunmaktadır.

#### 📂 Dosya İçeriği
* `Model/`: iThink (.itm) model dosyası.
* `Rapor/`: Detaylı proje raporu ve analizler (PDF).
* `Gorseller/`: Model diyagramı ve grafik çıktısı.
