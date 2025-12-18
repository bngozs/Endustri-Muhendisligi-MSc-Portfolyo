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

#### Problem Tanımı
Victor isimli bir dinleyicinin, İtalyan operası aryalarını dinlerken kelimeleri hafızasına alma (öğrenme) ve zamanla unutma dinamikleri arasındaki ilişki incelenmiştir.

#### Model Yapısı
Model, "Birinci Dereceden Negatif Geri Besleme" (First Order Negative Feedback) yapısına sahiptir:
* **Stok:** Hafızadaki Kelime Sayısı 
* **Giriş:** Ezberleme Hızı (Şarkı Temposu) 
* **Çıkış:** Unutma Hızı (Zaman Sabiti ile ters orantılı) 

#### Analiz Sonuçları
* **Denge Durumu:** Sistem, 90 saniyelik bir zaman sabiti ile dengeye ulaşmakta ve hafızada maksimum 45 kelime tutulabilmektedir.
* **Senaryo Analizi:** Hızlı müzik senaryosunda giriş hızı arttığında, denge noktası yükselmekte ancak sistemsel davranış korunmaktadır.

#### 📂 Dosya İçeriği
* `Model/`: iThink (.itm) model dosyası.
* `Rapor/`: Detaylı proje raporu ve analizler (PDF).
* `Gorseller/`: Model diyagramı ve grafik çıktısı.

* ---
### 2. 📂 Bireysel Kredi Satış Optimizasyonu Projesi Dosya Yapısı ve İçerik
**Kullanılan Araçlar:** Python (Pandas, Scikit-learn, Matplotlib), Jupyter Notebook, Google Colab. 
Bu çalışma, bankacılık sektöründe müşteri edinimi ve çapraz satış süreçlerini iyileştirmek amacıyla "Makine Öğrenmesi" ve "Finansal Simülasyon" teknikleri ile gerçekleştirilen bir operasyonel verimlilik projesidir.

#### Problem Tanımı
Mevcut durumda uygulanan "Soğuk Arama" (Cold Calling) stratejisi %90,4 oranında başarısızlıkla sonuçlanmakta; bu durum banka kaynaklarının (zaman, personel, bütçe) verimsiz kullanılmasına ve operasyonel maliyetlerin artmasına neden olmaktadır. Hedef, satın alma olasılığı yüksek müşterileri analitik yöntemlerle tespit etmektir.

#### Model Yapısı ve Metodoloji
Model, bankacılık verilerindeki doğrusal olmayan karmaşık ilişkilerin analizine dayanmaktadır:
Varlıklar (Veri Seti): 5.000 müşteriye ait demografik ve finansal veriler (Gelir, Eğitim, Mevduat vb.).
Algoritmalar: Random Forest ve Lojistik Regresyon modelleri karşılaştırılmış, Random Forest ile %99,1 tahmin başarısına ulaşılmıştır.
Proje Yönetimi: Süreç; Tanımlama, Planlama (CPM/PERT), Yürütme ve Kapanış evreleri ile yönetilmiştir.

#### Analiz ve İyileştirme Sonuçları
Verimlilik Artışı: Hatalı (boş) arama oranları %97 oranında azaltılarak satış ekiplerinin eforu optimize edilmiştir.
Gelir Etkisi: Model odaklı strateji ile günlük ortalama ciro potansiyeli 96.000 TL'den 329.467 TL'ye (3,5 kat) çıkarılmıştır.
Güvenilirlik: Modelin kararlılığı 5-Katlı Çapraz Doğrulama ve 0.9988 AUC skoru ile kanıtlanmıştır.

#### Maliyet ve Para Birimi Notu: 
Proje kapsamında analiz edilen tüm gelir grupları, müşteri harcamaları (CCAvg) ve simülasyon sonuçları Türk Lirası (TL) cinsinden hesaplanmış ve Türkiye ekonomik parametrelerine göre normalize edilmiştir.

#### 📂 Dosya İçeriği

* Proje-Yonetim-Dokumani/`: Proje Yönetim Dokümanı (CPM, PERT ve Çizelgeleme detayları).
* Teknik-Uygulama_Metodoloji-Raporu/`: Yazılım metodolojisi ve analiz detayları.
* Veri_Seti/`: Kaggle kaynaklı, TL bazlı normalize edilmiş müşteri verileri.
* Bireysel_Kredi_Satis_Performansinin_Optimizasyonu/`: Python (Jupyter Notebook) çalışma dosyaları.
