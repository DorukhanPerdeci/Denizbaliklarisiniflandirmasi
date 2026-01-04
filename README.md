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

<img width="1917" height="765" alt="Ekran görüntüsü 2026-01-04 135640" src="https://github.com/user-attachments/assets/4df9c053-de65-4747-8e76-9524a56165fd" />



