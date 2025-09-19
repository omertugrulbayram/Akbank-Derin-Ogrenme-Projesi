Akbank Derin Öğrenme Bootcamp: Yeni Nesil Proje Kampı
Bu proje, Akbank Derin Öğrenme Bootcamp kapsamında, CNN (Convolutional Neural Network) mimarisi kullanarak çok sınıflı bir görüntü sınıflandırma problemi çözmek için geliştirilmiştir. Projenin temel amacı, farklı coğrafi ve mimari yapıları doğru bir şekilde sınıflandıran bir model oluşturmaktır.

Projenin Amacı
Projenin temel amacı, derin öğrenme tekniklerini kullanarak Intel Image Classification veri setindeki doğa ve yapay ortamlara ait görüntüleri (binalar, orman, buzul, dağ, deniz, sokak) yüksek doğrulukla sınıflandıran bir model geliştirmektir.

Veri Seti Hakkında Bilgi
Veri Seti: Intel Image Classification

Türü: Çok Sınıflı Görüntü Sınıflandırması (Multiclass Image Classification)

Sınıflar: Buildings, Forest, Glacier, Mountain, Sea, Street (6 sınıf)

Boyut: Yaklaşık 25.000 eğitim görüntüsü, 3.000 test görüntüsü

Veri Seti Linki: https://www.kaggle.com/datasets/puneet6060/intel-image-classification

Kullanılan Yöntemler
Veri Ön İşleme: Görüntülerin yeniden boyutlandırılması (150x150 piksel) ve piksellerin 0-1 aralığına normalize edilmesi işlemleri yapılmıştır.

Veri Çoğaltma (Data Augmentation): Modelin genelleme yeteneğini artırmak ve aşırı uydurma (overfitting) sorununu engellemek amacıyla, ImageDataGenerator kullanılarak görüntü rotasyonu, yatay çevirme ve yakınlaştırma gibi dönüşümler uygulanmıştır.

Model Mimarisi: Temel CNN katmanları (Convolutional, Pooling, Dropout, Dense) içeren ardışık bir model (Sequential) oluşturulmuştur. Model, ReLU aktivasyon fonksiyonu ve Softmax çıkış katmanını kullanmaktadır.

Hiperparametre Optimizasyonu: Modelin performansı, katman sayısı, filtre boyutları, Dropout oranı ve öğrenme oranı gibi parametreler üzerinde yapılan denemelerle optimize edilmiştir.

Model Değerlendirmesi: Modelin performansı, doğruluk ve kayıp grafikleri, karmaşıklık matrisi (confusion matrix) ve sınıflandırma raporu (classification report) ile kapsamlı bir şekilde değerlendirilmiştir.

Elde Edilen Sonuçlar
Eğitimden sonra, modelin test verileri üzerindeki performansı oldukça başarılı bulunmuştur.

Genel Doğruluk Skoru: %84

Eğitim Grafikleri: Doğruluk ve Kayıp grafikleri, modelin eğitim ve doğrulama setleri üzerinde aşırı uydurma yapmadığını göstermiştir.

Sınıflandırma Raporu: Her sınıf için elde edilen detaylı metrikler aşağıdadır:

<img width="544" height="352" alt="image" src="https://github.com/user-attachments/assets/42065e98-fd83-43d9-9e70-7ad82f88e616" />


Elde edilen sonuçlar, modelin özellikle Forest (orman) sınıfında %96'lık F1-skoru ile mükemmel bir performans sergilediğini göstermektedir. Diğer tüm sınıflarda da güvenilir tahminler yapılmıştır.

Proje Linki
Projenin tüm kodlarına, detaylı anlatımlarına ve canlı demosuna aşağıdaki Kaggle Notebook linkinden ulaşabilirsiniz:

[https://www.kaggle.com/code/merturulbayram/notebookcdd3c38460]
