💻 Laptop Price Prediction (Regression Project)
Teknik özelliklerine göre bir dizüstü bilgisayarın piyasa değerini tahmin etmeyi amaçlayan uçtan uca bir makine öğrenmesi projesidir.

🚀 Projenin Amacı ve Özeti
Bu çalışmada, piyasadaki laptop verileri kullanılarak fiyatı etkileyen temel bileşenler analiz edilmiş ve Gradient Boosting Regressor algoritması ile yüksek doğrulukta bir tahmin modeli geliştirilmiştir.

📊 Veri Seti ve İşleme (Preprocessing)
Ham Veri: Laptop markası, işlemci nesli, RAM, SSD/HDD ve OS bilgilerini içerir.

Outlier Temizliği: Fiyat dağılımını bozan uç değerler istatistiksel yöntemlerle ayıklanmıştır.

Logaritmik Dönüşüm: Fiyat değişkenindeki sağa çarpıklığı gidermek ve model başarısını artırmak için np.log1p uygulanmıştır.

Feature Engineering: İşlemci modelleri ve RAM tipleri hiyerarşik (Ordinal) olarak puanlanmıştır.

🛠️ Kullanılan Teknolojiler & Kütüphaneler
Python (Pandas, NumPy)

Scikit-Learn (Modelleme ve Metrikler)

Seaborn & Matplotlib (Görselleştirme)

Joblib (Modelin .pkl olarak kaydedilmesi)

📈 Sonuçlar ve Performans
Modelimiz test verisi üzerinde oldukça başarılı sonuçlar vermiştir:

R² Score: 0.87

Best Model: Gradient Boosting Regressor

Feature Importance: Tahmin yapılırken en çok İşlemci (Processor) ve SSD kapasitesinin etkili olduğu görülmüştür.

📁 Proje Yapısı
laptop_data.csv: Orijinal ham veri seti.

laptop_data_cleaned.csv: İşlenmiş ve temizlenmiş veri seti.

Laptop_Price_Prediction.ipynb: Analiz ve modelleme adımlarının bulunduğu notebook.

laptop_model.pkl: Eğitilmiş modelin kayıtlı dosyası.
