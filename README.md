# Obesity-Classification-and-PCA

🧠 Obesity Prediction with Machine Learning
Bu proje, bireylerin fiziksel özellikleri ve yaşam tarzı alışkanlıklarına göre obezite seviyelerini tahmin etmeyi amaçlayan bir makine öğrenimi çalışmasıdır. Proje, Kaggle'dan alınan veri seti ile gerçekleştirilmiştir.

📂 Kullanılan Veri Seti
Obesity prediction.csv dosyası Kaggle’dan alınmıştır ve aşağıdaki türden özellikler içerir:

Yaş, boy, kilo gibi fiziksel ölçümler

Kalori alımı, fiziksel aktivite düzeyi gibi yaşam tarzı bilgileri

Hedef: Obezite kategorileri (örneğin: Normal Weight, Obesity Type II, Overweight Level I ...)

🛠️ Kullanılan Kütüphaneler
pandas, numpy

matplotlib

scikit-learn: modelleme, ön işleme ve metrikler

PCA: boyut indirgeme

LogisticRegression, RandomForestClassifier, SVC

🔍 Modelleme Süreci
Veri Yükleme & İnceleme

Label Encoding ile kategorik verilerin sayısallaştırılması

Veri Standartlaştırma (StandardScaler)

Model Eğitimi

Lojistik Regresyon

Rastgele Orman (Random Forest)

Destek Vektör Makineleri (SVM)

Model Performans Analizi
Her model için classification_report ile doğruluk, hassasiyet, f1-score gibi ölçütler raporlandı.

PCA (Principal Component Analysis)
Verinin boyutu 2’ye indirgenerek tekrar Logistic Regression ile sınıflandırma yapıldı (görselleştirme/dim reduce denemesi amacıyla).

📊 Sonuçlar (Karşılaştırmalı)
Model	Accuracy (Test Set)
Logistic Regression	~87%
Random Forest	~96%
SVM	~96%
PCA + Logistic	~30%

📌 Not: PCA ile boyut indirgeme sonrası performans ciddi oranda düştü. Bu da veri setinde yüksek boyutlu değişkenlerin önemli bilgiler içerdiğini gösteriyor.
