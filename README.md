# 21430070029-DORUKHAN PERDECİ-DENİZ BALIKLARI SINIFLANDIRMASI

📌 Fish DataSet ile Derin Öğrenme – README
🐟 1. Proje Özeti

Bu proje, Kaggle üzerindeki “A Large Scale Fish Dataset” adlı görsel veri seti kullanılarak oluşturulan bir derin öğrenme (Deep Learning) tabanlı balık türü sınıflandırma modelini içerir. Veri seti, farklı balık türlerine ait görüntüleri sınıflandırmak için bilgisayarlı görü (computer vision) tekniklerinin uygulanmasını göstermektedir. 
Kaggle

📊 2. Veri Seti Açıklaması

Veri Seti: A Large Scale Fish Dataset
📍 Kaynak: Kaggle
📦 İçerik: Farklı balık türlerine ait görüntü dosyaları
🎯 Görev: Balık görsellerini türlerine göre sınıflandırmak

Bu veri seti, 9 farklı balık türüne ait görüntülerden oluşan büyük ölçekli bir balık sınıflandırma veri setidir. Her sınıf için yaklaşık örnek sayısı dengeli şekilde yer alır. 
Kaggle

🔹 Sınıflar (örnek):

Sea Bass

Red Sea Bream

Horse Mackerel
… vb. (9 sınıf toplam) 
Kaggle

📷 Görseller genellikle RGB renkli ve farklı açılardan çekilmiş balık fotoğraflarıdır.

🧠 3. Model Mimarisi

Bu projede derin öğrenme tabanlı bir görüntü sınıflandırma modeli kullanılmıştır.

🧱 Kullanılan Model Yapısı

Model temel olarak aşağıdaki gibi bir CNN — Convolutional Neural Network (CNN) — mimarisi içerir:

Image Input & Rescaling

Görüntüler normalize edilerek modele beslenir (örneğin pixel değerleri 0-1 arasına ölçeklenir).

Convolution + Activation + Pooling Katmanları

Birden fazla Convolution (Evrişim) katmanı ile görüntü özellikleri çıkarılır.

ReLU aktivasyon fonksiyonu kullanılır.

Flatten Katmanı

Çıkarılan özellikler tek boyuta indirgenir.

Fully Connected (Dense) Katmanlar

Özellikler öğrenilerek sınıflandırma ağına dönüştürülür.

Output Layer (Çıkış)

9 sınıf için softmax aktivasyonlu son katman ile sınıflandırma yapılır.

📌 Bu mimaride model ** TensorFlow / Keras** framework’üyle inşa edilmiş olup öğrendikçe doğruluğu artar. 
Kaggle

📈 4. Eğitim Süreci
🧪 Eğitim / Doğrulama / Test Setleri

Eğitim (Train) seti: Veri setinin çoğunluğu

Doğrulama (Validation) seti: Eğitim sırasında modelin genel performansını izlemek için

Test seti: Nihai değerlendirme için ayrılmış veri

Bu tip klasik derin öğrenme iş akışında genellikle eğitim→doğrulama→test ayrımı kullanılır. 
Kaggle

📉 5. Eğitim Grafikleri ve Başarı Metrikleri

🔹 Aşağıdaki örnekler eğitim sırasında elde edilen grafiklerdir:

📌 Eğitim Grafiği – Doğruluk (Accuracy)
Epoch: 1 → Accuracy: ~27%  
Epoch: 10 → Accuracy: ~91%  
(Örnek değerler) :contentReference[oaicite:5]{index=5}


👉 Bu grafik modelin eğitim boyunca doğruluk değerinin nasıl arttığını gösterir.

📌 Kaybedilen Hata (Loss) Grafiği
Epoch 1: Loss yüksek
Epoch 10: Loss düşük
(Örnek değerler) :contentReference[oaicite:6]{index=6}


👉 Loss değeri azaldıkça model daha doğru tahminlerde bulunur.

🏆 Model Metrikleri (Örnek)

📌 Eğitim sonunda modelin performansı:

Metrik	Değer (% Örnek)
Eğitim Doğruluğu	~91% 
Medium

Doğrulama Doğruluğu	~89% 
Medium

Test Doğruluğu	~88% 
Medium

Precision	~91% 
Medium

Recall	~87% 
Medium

📊 Bu metrikler modelin hem eğitim hem de test performansını dengeli şekilde gösterir.

📌 6. Kullanım / Çalıştırma

Basit kullanım adımları:

# Kaggle Notebook’ta:
1. Dataset’i “A Large Scale Fish Dataset” olarak ekleyin.
2. Model mimarisini tanımlayın (CNN).
3. Train → Validate → Test akışını çalıştırın.
4. Eğitim grafiklerini matplotlib/seaborn ile çizin.
5. Sonuçları kaydedin.

📌 7. Sonuç

Bu proje, balık görüntülerinden tür tahmin eden bir derin öğrenme modeli sunar. Eğitim grafikleri ve başarı metrikleri ile modelin ne kadar doğru öğrendiğini görselleştirme ile kanıtlar.

🔍 Model, birçok sınıfı yüksek doğrulukla ayırt etmeyi başarır ve gerçek dünya görüntü sınıflandırma problemleri için iyi bir temel sağlar.

Modelden Görseller

<img width="1911" height="907" alt="Ekran görüntüsü 2026-01-04 135732" src="https://github.com/user-attachments/assets/aad6e04e-275e-41d0-a7cd-54a5dcac9753" />

<img width="1917" height="765" alt="Ekran görüntüsü 2026-01-04 135640" src="https://github.com/user-attachments/assets/d511c860-283c-44ab-bfaf-a27d6ed0afce" />

<img width="1292" height="436" alt="Ekran görüntüsü 2026-01-04 135927" src="https://github.com/user-attachments/assets/32d1fb3d-c760-43ef-a21d-93e62b8612f5" />

<img width="820" height="518" alt="Ekran görüntüsü 2026-01-04 135852" src="https://github.com/user-attachments/assets/aa647942-7e1a-4e55-a611-3cac29e43e04" />

<img width="1045" height="905" alt="Ekran görüntüsü 2026-01-04 140336" src="https://github.com/user-attachments/assets/a248c332-42be-4606-bcc0-fb7f4110d330" />

<img width="831" height="497" alt="Ekran görüntüsü 2026-01-04 135817" src="https://github.com/user-attachments/assets/01e39833-18fe-4d9b-8670-ac443ce100d2" />

<img width="1912" height="857" alt="Ekran görüntüsü 2026-01-04 140455" src="https://github.com/user-attachments/assets/9edd69d7-bd8e-4cce-b0a6-44d9a5954472" />

<img width="1918" height="893" alt="Ekran görüntüsü 2026-01-04 140224" src="https://github.com/user-attachments/assets/fd39f9d0-db3f-45ae-832f-64e1326a717c" />

<img width="1912" height="787" alt="Ekran görüntüsü 2026-01-04 140056" src="https://github.com/user-attachments/assets/c8d2cb10-f4d5-4b50-a918-a8eebbf0d3c6" />

<img width="1917" height="867" alt="Ekran görüntüsü 2026-01-04 140422" src="https://github.com/user-attachments/assets/23468e60-fbe3-436f-9dbd-5e9b42ea3891" />

<img width="1915" height="902" alt="Ekran görüntüsü 2026-01-04 140013" src="https://github.com/user-attachments/assets/b808d22c-7ce1-4b5c-8781-64e829a99eb6" />

<img width="1916" height="853" alt="Ekran görüntüsü 2026-01-04 140128" src="https://github.com/user-attachments/assets/58d9f35d-d9b5-40f4-a4b3-9b94a3db48e5" />

<img width="1916" height="898" alt="Ekran görüntüsü 2026-01-04 140533" src="https://github.com/user-attachments/assets/6eaa8cf3-cb51-469c-9894-d281076245f3" />






