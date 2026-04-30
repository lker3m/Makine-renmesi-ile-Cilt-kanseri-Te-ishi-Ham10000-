# Makine-renmesi-ile-Cilt-kanseri-Te-ishi-Ham10000-


🩺 Makine Öğrenmesi ile Cilt Kanseri Teşhisi (HAM10000)

👤 Öğrenci Bilgileri

Ad Soyad: Kerem Bayrak

Öğrenci Numarası: 25019909004

Üniversite: Bartın Üniversitesi

Ders: Makine Öğrenmesi

📝 Proje Açıklaması Bu proje, dermoskopik görüntüler üzerinden 7 farklı cilt lezyonu türünü sınıflandırmak amacıyla geliştirilmiştir. Proje kapsamında hem klasik makine öğrenmesi algoritmaları hem de derin öğrenme (CNN) teknikleri kullanılarak modellerin başarı oranları karşılaştırılmıştır.

📊 Veri Seti Tanıtımı Veri Seti: Skin Cancer MNIST: HAM10000

Tanıtım: Veri seti, 10.015 adet görüntü ve bunlara ait metadata (yaş, cinsiyet, lezyon bölgesi) bilgilerini içerir.

Sınıflar: akiec (Aktinik Keratoz), bcc (Bazal Hücreli Karsinom), bkl (Benign Keratoz), df (Dermatofibroma), mel (Melanom), nv (Melanositik Nevüs), vasc (Vasküler Lezyon).

🛠️ Veri Ön İşleme (Preprocessing) Eksik Veri: age sütunundaki eksik değerler veri setinin ortalaması ile doldurularak temizlenmiştir.

Görüntü Hazırlama: Tüm görseller 64x64 boyutuna getirilmiş ve piksel değerleri 0-1 arasına çekilerek normalizasyon uygulanmıştır.

Veri Bölme: Veriler %80 eğitim ve %20 test seti olarak ayrılmıştır.

🧠 Kullanılan Algoritmaların Mantığı CNN (Convolutional Neural Networks): Görüntü işleme görevlerinde en başarılı sonuçları veren bu algoritma, pikseller arasındaki karmaşık desenleri öğrenerek ana sınıflandırmayı yapmıştır.

Random Forest: Metadata üzerinden çalışan bu algoritma, çoklu karar ağaçları kullanarak klinik verilerin (yaş, cinsiyet vb.) teşhis üzerindeki etkisini ölçmüştür.

Logistic Regression: Başlangıç seviyesinde bir karşılaştırma sunmak adına basit doğrusal sınıflandırma modeli olarak kullanılmıştır.

📈 Model Performansı ve Değerlendirme Accuracy (Doğruluk): CNN modelimiz yaklaşık %70-75 doğruluk oranına ulaşmıştır.

Confusion Matrix: Modelin hata yaptığı sınıflar incelenmiş ve sonuçlar görselleştirilmiştir.

Tıbbi Risk Analizi: Tahmin sonuçları "Yüksek Riskli" (Melanom) ve "Düşük Riskli" (Nevüs vb.) olarak gruplandırılarak yorumlanmıştır.

🚀 Sonuç ve Yorumlar CNN modeli, görüntü verilerini işlemede klasik algoritmalara göre çok daha üstün performans sergilemiştir. Modelin başarısı, veri artırma (data augmentation) ve daha derin ağ yapıları ile artırılabilir. Özellikle Melanositik Nevüs (nv) sınıfının baskın olması, modelin bu sınıfa karşı daha eğilimli olmasına yol açmıştır.

💻 Kodların Çalıştırılması .ipynb dosyasını Google Colab'da açın.

Gerekli kütüphaneleri (TensorFlow, Pandas, Seaborn) kurun.

Eğitilmiş model ağırlıklarını kullanmak için cilt_kanseri_modeli.h5 dosyasını sisteme tanıtın.
