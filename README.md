# bitirmeprojesi
# 📁 Dosya Erişim Loglarından Anomali Tespiti

Bu proje, Windows sistemlerdeki kullanıcı dosya erişim loglarını analiz ederek, olağandışı erişimleri derin öğrenme modelleriyle tespit etmeyi amaçlamaktadır.

---

## 🔍 Proje Amacı

Kurum içi güvenlik tehditlerini, kullanıcıların günlük erişim alışkanlıklarındaki anomalileri tespit ederek belirlemek.
- Etiketli veri olmadan çalışan gözetimsiz modeller
- Zaman serisi analizi yapan yapılar
- Dosya yolu semantiğine dayalı anlamlı analiz

---

## 🧠 Kullanılan Modeller

### 1. **LSTM Autoencoder**
- Gözetimsiz öğrenme
- Yeniden üretim hatası üzerinden karar
- Yalnızca normal verilerle eğitilir
- Doğruluk oranı: %85–90

### 2. **CNN-LSTM**
- CNN ile örüntü çıkarımı
- LSTM ile zaman bağımlılığı
- Ağırlıklı loss fonksiyonu ile eğitim
- Doğruluk oranı: %92–94

### 3. **SemantikLSTM**
- Dosya yolu tokenize edilerek işlenir
- Embedding + LSTM ile semantik analiz
- Doğruluk oranı: %70–75

---

## 🧪 Veri Seti

Projede iki farklı veri kümesi kullanılmıştır:
- `balanced_logs_dense.csv`: Normal ve anormal etiketli log verisi
- `realistic_anomaly_dataset.csv`: Gerçekçi semantik dosya yolları içeren veri seti

Veriler, kullanıcı_id, işlem, zaman, dosya_yolu gibi alanlardan oluşur.

---

## 🛠️ Kullanılan Teknolojiler

- Python 3.10
- TensorFlow / Keras
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn

---

## 📊 Performans Metrikleri

- Accuracy
- Precision / Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

---

## 🚀 Nasıl Çalıştırılır?



# Jupyter veya Colab üzerinden çalıştır

