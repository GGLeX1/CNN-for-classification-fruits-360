# CNN-for-classification-fruits-360

data fruits 360 (https://www.kaggle.com/datasets/moltean/fruits/data)

Proyek ini menggunakan **Convolutional Neural Network (CNN)** untuk mengklasifikasikan gambar buah menjadi beberapa kelas.  

---

## 🚀 Cara Menjalankan di Colab

1. Upload dataset kamu ke Google Drive atau Colab.
2. Jalankan notebook `Submission_CNN.ipynb`.
3. Model akan otomatis dilatih dan disimpan ke tiga format:
   - TensorFlow SavedModel
   - TensorFlow.js
   - TensorFlow Lite

---

## 🧠 Arsitektur Model CNN

```text
Conv2D (32 filters, 3x3, ReLU)
MaxPooling2D (2x2)
Conv2D (64 filters, 3x3, ReLU)
MaxPooling2D (2x2)
Conv2D (128 filters, 3x3, ReLU)
MaxPooling2D (2x2)
Flatten
Dense (128, ReLU)
Dropout (0.5)
Dense (num_classes, Softmax)
```

---

## 📊 Evaluasi

| Dataset    |   Akurasi  |  Loss  |
|------------|------------|--------|
| Training   |   0.9805   | 0.0571 |
| Validation |   0.9994   | 0.0018 |
| Test       |   0.9993   | 0.0017 |

*(Gantilah angka sesuai hasil evaluasi kamu)*

---

## 🧾 Informasi Tambahan

- Dataset: Folder gambar buah (train, val, test)
- Framework: TensorFlow 2.19.0
- Notebook: `Submission_CNN.ipynb`
- Platform: Google Colab

---

## 🪪 Lisensi

Proyek ini dibuat untuk keperluan pembelajaran dan pengembangan model CNN.  
Silakan gunakan, modifikasi, dan kembangkan sesuai kebutuhan.
