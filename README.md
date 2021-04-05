# Facelift Yarışması
Fatih YAVUZ & Ahmet Yakup ÇETİNKAYA

### Proje Amacı
3 farklı araca ait görüntülerle aracın eski kasa mı yeni kasa mı olduğu tespit edilecektir.

### Araç Markaları 
- Hyundai_I20_Hatchback_2018 
- Nissan_Qashqai_SUV_2017 
- Volkswagen_Passat_Sedan_2014

### Kullanılan Teknolojiler

- Python
- Keras
- Tensorflow
- Scikitlearn
- Numpy

### Veriseti Linki
https://drive.google.com/file/d/1xlgr13cp3H64Byb7WNwjpJvH-OA11ccr/view?usp=sharing

### Validation Score

%84

### Kodlama Süreci
- Veriler eleme yapıldıktan sonra 64x64 boyutlarında kullanılmaya başlandı. Bunun nedeni yetersiz ram'dir. Daha yüksek ram'li teknolojiler ile skor değeri artırılabilir.
- Veriler her aracın eski yeni modeli olarak 6 ayrı şekilde etiketlenmiştir.
- Her seferinde boyutlandırma yapmamak için .npz formatında kaydedilmiştir.
- Test edilen model mimarileri  
    - EfficientNet B0-B7 arası
    - ResNet50
    - DenseNet169
    - DenseNet201
- En iyi skor DenseNet201 de alındığından o kullanılmıştır.    

### Karşılaşılan Sorunlar
- Resim sayısı fazla olduğundan bilgisayar ram'leri yetersiz gelmektedir.
- Araçlardaki resim sayılarının birbirlerine göre tutarsız olması.