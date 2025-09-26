# Göz Hastalıkları Sınıflandırması CNN Projesi

## 📄 Proje Amacı
Bu proje, fundus görüntülerinden göz hastalıklarının otomatik tespiti için Convolutional Neural Network (CNN) kullanarak bir derin öğrenme modeli geliştirmeyi amaçlamaktadır.

## 📊 Veri Seti Hakkında
- **Kaynak:** Kaggle - Eye Diseases Classification Dataset
- **Görüntü Sayısı:** 4217
- **Sınıf Sayısı:** 4
- **Görüntü Boyutu:** Çeşitli boyutlar (224x224'e yeniden boyutlandırıldı)
- **Sınıflar:** glaucoma, normal, diabetic_retinopathy, cataract

## 🛠️ Kullanılan Yöntemler
- **Framework:** TensorFlow/Keras
- **Model Mimarisi:** Özel CNN + Transfer Learning
- **Data Augmentation:** Rotation, Flip, Zoom, Color Jitter
- **Regularization:** Dropout, Batch Normalization
- **Optimizasyon:** Adam Optimizer + Learning Rate Scheduling
- **Görselleştirme:** Accuracy, Confusion Matrix, Classification Report

### Model Performansı
Aşağıdaki tablo, modelin dört sınıftaki sınıflandırma performansını göstermektedir:

| Hastalık / Sınıf       | Precision | Recall | F1-Score | Support |
|-------------------------|-----------|--------|----------|---------|
| Glaucoma                | 0.90      | 0.65   | 0.75     | 151     |
| Normal                  | 0.76      | 0.96   | 0.85     | 161     |
| Diabetic Retinopathy    | 0.99      | 0.99   | 0.99     | 165     |
| Cataract                | 0.90      | 0.89   | 0.89     | 156     |
| **Accuracy**            |           |        | **0.88** | **633** |
| **Macro Avg.**          | 0.89      | 0.87   | 0.87     | 633     |
| **Weighted Avg.**       | 0.89      | 0.88   | 0.87     | 633     |

🔎 **Notlar:**
- Modelin genel doğruluk (accuracy) değeri **%88**’dir.  
- En yüksek başarı **Diabetic Retinopathy** sınıfında gözlemlenmiştir (F1-Score: **0.99**).  
- **Glaucoma** sınıfında recall değerinin düşük olması, bazı vakaların yanlış sınıflandırıldığını göstermektedir.  

## 🔗 Kaggle Notebook Linki
[Projenin Kaggle Notebook'u](https://www.kaggle.com/code/remdilatkse/eye-diseases-classification2)
