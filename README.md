# Kalp Hastalığı Riski Tahmini – Makine Öğrenmesi Projesi
## 👩‍🎓 KızKarDes: Afetten Etkilenmiş Kadınlar için Kariyer Destek Programı
### Yapay Zeka Akademisi – Bitirme Projesi

<br>

📌 Proje Hakkında 

Bu proje, Yapay Zeka Akademisi Final Projesi kapsamında gerçekleştirilmiştir. Projede, Heart Disease UCI veri seti kullanılarak bir sınıflandırma modeli oluşturulmuş ve bireylerin kalp hastalığı riski taşıyıp taşımadığı tahmin edilmeye çalışılmıştır.

Seçilen Problem Türü: Sınıflandırma

Kullanılan Veri Seti: Heart Disease UCI (https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data/data)

Hedef Değişken: target (1 = kalp hastalığı var, 0 = yok)

<br>

🎯 Problem Tanımı

Bu projede amaç, bireylerin tıbbi verileri üzerinden kalp hastalığı taşıyıp taşımadıklarını tahmin eden bir makine öğrenmesi modeli geliştirmektir.

🔍 Tahminin Pratik Önemi

- Erken teşhis ile yaşam kalitesinin artırılması

- Sağlık sistemlerinde önleyici müdahaleler için karar destek sistemleri oluşturulması

<br>

📊 Veri Analizi (EDA)

Veri seti incelenerek aşağıdaki adımlar uygulanmıştır:

- Veri yapısı ve istatistiksel özetler: df.info(), df.describe()

<img width="517" height="431" alt="info" src="https://github.com/user-attachments/assets/171c8cf4-b075-4f64-87f8-de408e176a52" />


- Eksik değer kontrolü ve uygun şekilde doldurma / çıkarma, aykırı değer analizi

<img width="953" height="563" alt="eksik" src="https://github.com/user-attachments/assets/bdf65175-fe1b-4bcd-8cdc-7839a0bf9695" />

<img width="875" height="340" alt="aykırı" src="https://github.com/user-attachments/assets/9ef2fea5-6862-4b4e-b51e-98d951caeea3" />


- Hedef değişkenin dağılım analizi (target)

<img width="915" height="418" alt="hedef" src="https://github.com/user-attachments/assets/40cdb1e2-cc6d-4c43-ae2f-4e678e511329" />


- Görselleştirmeler:

  - Korelasyon matrisi (heatmap)

<img width="764" height="637" alt="korelasyon" src="https://github.com/user-attachments/assets/222a1b44-fa32-46e0-80f9-889163ba9b91" />


  - Yaş dağılımı ve kalp hastalığı ilişkisi (histogram/barplot)

<img width="733" height="439" alt="age" src="https://github.com/user-attachments/assets/dc01f4c3-2d6c-43d0-a1b3-8c77ec0f544d" />


- Cinsiyet, egzersizle gelen anjina, göğüs ağrısı tipi gibi kategorik değişkenlerin etkisi

<br>

🔧 Veri Ön İşleme

- Kategorik değişkenler LabelEncoder veya OneHotEncoder ile kodlandı.

<img width="972" height="415" alt="label" src="https://github.com/user-attachments/assets/475f80b2-2850-4b2c-9004-ac7fea55da19" />


- Sayısal veriler için StandardScaler uygulandı.

- Veri %80 eğitim, %20 test olarak train_test_split() ile ayrıldı.

<img width="804" height="391" alt="ayırma" src="https://github.com/user-attachments/assets/54a65075-c83e-49ba-9b53-66b350fd2e73" />


<br>

🤖 Uygulanan Modeller

Farklı sınıflandırma algoritmaları kullanılarak modeller oluşturuldu:

- Logistic Regression

- Random Forest Classifier 

- KNN (K-Nearest Neighbors)

<img width="967" height="525" alt="model" src="https://github.com/user-attachments/assets/fa88501f-7256-4ce9-ba38-2d1ea13e028c" />



🧪 Kullanılan Başarı Metriklerine göre değerlendirme:

- Accuracy, Precision, Recall, F1-Score, Confusion Matrix, ROC-AUC eğrisi
<img width="1015" height="623" alt="sonuc" src="https://github.com/user-attachments/assets/8c146efb-3041-4266-9f64-bf60f7c28a36" />



<br>

🔍 Model Karşılaştırması

En iyi performans gösteren model:

- Random Forest modeli, özellikle Recall, F1-score ve AUC metriklerinde öne çıkmıştır.

- Logistic Regression modeli daha basit ve yorumlanabilir olsa da, Random Forest daha yüksek doğruluk sunmuştur.

- Overfitting kontrolü için eğitim/test başarıları karşılaştırılmıştır.

<img width="495" height="123" alt="m_sonuc" src="https://github.com/user-attachments/assets/3bd3d94e-9f0d-433c-a125-9d8b3fb8fa05" />


<br>

📌 Sonuç ve Yorumlar

- Model, kalp hastalığı riskinin tahmini için güçlü bir karar destek sistemi potansiyeli taşımaktadır.

- Özellikle cp, thalach, oldpeak, ca gibi değişkenlerin önemli etkileri olduğu gözlemlenmiştir.

- Daha büyük ve dengeli veri setleri, hiperparametre ayarlamaları ile doğruluk artırılabilir.

- Model, sağlık kuruluşları için ön tarama süreçlerinde kullanılabilir.

<br>

🌟 Ekstra Adımlar

- GridSearchCV ile Random Forest hiperparametre optimizasyonu gerçekleştirildi.

- Özellik önemleri (Feature Importance) grafiği ile modelin hangi değişkenlere dayandığı analiz edildi.

<img width="903" height="480" alt="feature" src="https://github.com/user-attachments/assets/24a7e6b3-7fca-4d70-a40d-aac01056bff8" />


Proje detaylarını incelemekten ve geri bildirim vermekten lütfen çekinmeyin :) Değerli yorumlarınız için çok teşekkürler.
