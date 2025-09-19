# Akbank-Derin-Ogrenme-Projesi

# Akbank Derin Öğrenme Bootcamp: Yeni Nesil Proje Kampı

Bu proje, Akbank Derin Öğrenme Bootcamp kapsamında, Convolutional Neural Network (CNN) mimarisi kullanarak çok sınıflı bir görüntü sınıflandırma problemi çözmek için geliştirilmiştir. Proje, Intel Image Classification veri setini kullanarak farklı coğrafi ve mimari yapıları sınıflandırmayı amaçlamaktadır.

## Projenin Amacı

Projenin temel amacı, derin öğrenme tekniklerini kullanarak farklı doğa ve yapay ortam kategorilerine ait görüntüleri (binalar, orman, buzul, dağ, deniz, sokak) doğru bir şekilde sınıflandıran bir model geliştirmektir.

## Veri Seti Hakkında Bilgi

* **Veri Seti:** Intel Image Classification
* **Türü:** Multiclass Image Classification
* **Sınıflar:** Buildings, Forest, Glacier, Mountain, Sea, Street (6 sınıf)
* **Boyut:** Toplam ~25.000 eğitim görüntüsü, 14.000 test görüntüsü
* **Veri Seti Linki:** [https://www.kaggle.com/datasets/puneet6060/intel-image-classification](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)

## Kullanılan Yöntemler

* **Veri Ön İşleme:** Görüntülerin yeniden boyutlandırılması, etiketlenmesi ve normalizasyonu işlemleri yapılmıştır.
* **Veri Çoğaltma (Data Augmentation):** Modelin genelleme yeteneğini artırmak amacıyla, ImageDataGenerator kullanılarak görüntü rotasyonu, çevirme (flip), yakınlaştırma (zoom) ve parlaklık ayarları gibi dönüşümler uygulanmıştır.
* **Model Mimarisi:** Temel CNN katmanları (Convolutional, Pooling, Dropout, Dense) içeren bir model oluşturulmuştur.
* **Hiperparametre Optimizasyonu:** Model performansını artırmak için çeşitli hiperparametreler (katman sayısı, filtre boyutu, öğrenme oranı, vb.) üzerinde denemeler yapılmıştır.
* **Model Değerlendirmesi:** Modelin performansı, doğruluk (accuracy) ve kayıp (loss) grafikleri, karmaşıklık matrisi (confusion matrix) ve sınıflandırma raporu (classification report) ile değerlendirilmiştir.
* **Model Yorumlama:** Grad-CAM yöntemi kullanılarak modelin karar verirken görüntülerin hangi bölgelerine odaklandığı görselleştirilmiştir.

## Elde Edilen Sonuçlar

(Bu bölümü projenin sonunda, modelin eğitimini tamamladığımızda elde ettiğimiz sonuçlara göre dolduracağız.)

## Kaggle Notebook

Projenin tüm detaylı kodlarına ve açıklamalarına aşağıdaki Kaggle Notebook linkinden ulaşabilirsiniz:

[Kaggle Notebook Linki Buraya Gelecek]
