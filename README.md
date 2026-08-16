Müşteri Ayrılma Tahmini

Bu proje, Türkiye Yapay Zeka Akademisi Makine Öğrenmesi Ara Ödevi kapsamında hazırlanmıştır.

Projede müşterilerin bazı temel özellikleri kullanılarak müşterinin hizmetten ayrılıp ayrılmayacağını tahmin eden basit bir makine öğrenmesi uygulaması geliştirilmiştir.

Kullanılan Veri

Çalışmada Python ile 200 satırlık örnek bir müşteri veri seti oluşturulmuştur.

Veri setinde kullanılan bazı değişkenler:

• Yaş
• Gelir
• Abonelik süresi
• Destek talebi sayısı
• Şehir
• Üyelik tipi
• Churn

churn hedef değişkenidir.

• 0: Müşteri kalıyor
• 1: Müşteri ayrılıyor

Yapılan İşlemler

Çalışma kapsamında:

• Veri seti oluşturuldu ve incelendi.
• Eksik değer kontrolü yapıldı.
• Yeni bir öznitelik oluşturuldu.
• Kategorik değişkenlere One-Hot Encoding uygulandı.
• Sayısal değişkenler StandardScaler ile ölçeklendi.
• Veri train, validation ve test kümelerine ayrıldı.
• Logistic Regression modeli eğitildi.
• KNN modeli eğitildi.
• Modeller validation sonuçlarına göre karşılaştırıldı.
• Daha başarılı olan model test verisi üzerinde değerlendirildi.

Değerlendirme Metrikleri

Seçilen model aşağıdaki metriklerle değerlendirilmiştir:

• Accuracy
• Precision
• Recall
• F1-score
• Confusion Matrix

Kurulum

Gerekli kütüphaneleri yüklemek için:

```bash
pip install -r requirements.txt
```

Programı çalıştırmak için:

```bash
python churn_prediction.py
```

Sonuç

Logistic Regression ve KNN modellerinin validation performansları karşılaştırılmış ve daha başarılı olan model test verisi üzerinde değerlendirilmiştir.

Bu çalışma sayesinde veri ön işleme, öznitelik oluşturma, veri bölme, model eğitimi ve sınıflandırma metriklerinin kullanımı temel bir müşteri ayrılma problemi üzerinde uygulanmıştır.
