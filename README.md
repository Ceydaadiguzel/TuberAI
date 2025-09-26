# TuberAI: CNN ile Tüberküloz Teşhisi

## Giriş
Bu projede, [Kaggle Tuberculosis (TB) Chest X-ray Dataset](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset) veri seti kullanılmıştır. Projedeki genel amaç, tüberküloz ve normal göğüs röntgenlerini sınıflandırarak CNN ile otomatik tespit yapabilmektir. Veri seti iki sınıftan oluşmaktadır:

- **Tuberculosis:** 700 görüntü  
- **Normal:** 3500 görüntü  

Modelleme aşamasında **Convolutional Neural Network (CNN)** algoritması kullanılmıştır.  
Teknik adımlar:

1. Veri setine giriş
2. Sınıf dağılımı
3. Görsellerin teknik incelemesi (boyut, kanal, piksel istatistikleri)
4. Verilerin görselleştirilmesi  
5. Normalizasyon ve ön işleme
6. Model mimarisi
7. Accuracy & Loss grafikleri
8. Modelin performans değerlendirmesi 
9. Hyperparameter tuning ile optimizasyon

Tüm teknik anlatım ve detaylar notebook içerisinde **markdown hücreleri** ile açıklanmıştır.  

---

## Metrikler
Modelin test setindeki performansı:

- **Test Accuracy:** 94.76%  
- Confusion matrix ve classification report ile sınıf bazlı performans incelenmiştir.  

Gözlemler:

- TB sınıfı için yüksek recall elde edilmiştir, bu sağlık uygulamaları açısından kritik önemdedir.  
- Normal sınıfı için precision yüksek, yani model yanlış pozitifleri düşük tutmaktadır.  
- Model validation ve test setlerinde iyi genelleme göstermektedir.  

---

## Ekler
Projede GPU ile model eğitimi gerçekleştirilmiştir ve data augmentation sayesinde sınıf dengesizliği problemleri minimize edilmiştir.  

---

## Sonuç ve Gelecek Çalışmalar
Bu proje, göğüs röntgenlerinden TB tespitini otomatikleştirmeyi amaçlamaktadır. Sağlık alanında erken teşhis tüm insanlık için çok önemli bir husustur. Bu tür projeler, hızlı ve doğru tanı koyma konusunda sağlık sektörüne yardımcı olabilir, insan hatasını azaltabilir ve hastaların uygun tedaviye daha hızlı ulaşmasına katkı sağlar. Bu proje, bu alanda yapay zekâ ile fark yaratma motivasyonumu yansıtan bir çalışmadır.

Gelecek çalışmalar için öneriler:

- Gerçek zamanlı veri toplama ve model güncelleme  
- Daha ileri CNN mimarileri veya transfer learning kullanımı  
- Kullanıcı arayüzü ile entegre sağlık uygulaması geliştirme  

---

## Linkler
- Kaggle veri seti: [Tuberculosis Chest X-ray Dataset](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset)  
- Kaggle notebook: [TuberAI CNN ile TB Teşhisi](https://www.kaggle.com/code/ceydaadigzel/tuberai-cnn-ile-t-berk-loz-te-hisi?scriptVersionId=264216713)  
