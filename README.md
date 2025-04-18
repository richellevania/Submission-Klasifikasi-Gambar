# 🏞️ Proyek Klasifikasi Gambar: Intel Image Classification

Selamat datang di proyek klasifikasi gambar! Proyek ini bertujuan membangun model deep learning untuk mengklasifikasikan gambar alam ke dalam beberapa kategori menggunakan TensorFlow dan Keras. Dataset diambil dari Kaggle (*Intel Image Classification Dataset*), dan proyek mencakup tahap preprocessing, augmentasi data, pelatihan model CNN, serta evaluasi hasil. 🚀

---

## 📑 Daftar Isi

- [📘 Ikhtisar Proyek](#📘-ikhtisar-proyek)
- [🗂️ Dataset](#🗂️-dataset)
- [📦 Persyaratan](#📦-persyaratan)
- [⚙️ Cara Menjalankan](#⚙️-cara-menjalankan)
- [▶️ Penggunaan](#▶️-penggunaan)
- [🏗️ Arsitektur Model](#🏗️-arsitektur-model)
- [🏋️ Pelatihan dan Evaluasi](#🏋️-pelatihan-dan-evaluasi)
- [📊 Hasil](#📊-hasil)
- [🤝 Kontribusi](#🤝-kontribusi)

---

## 📘 Ikhtisar Proyek

Proyek ini mengembangkan model CNN (Convolutional Neural Network) untuk klasifikasi gambar pemandangan seperti laut, pegunungan, hutan, dan kota. Model dilatih menggunakan kombinasi data augmentasi dan teknik pelatihan standar pada **Google Colab dengan GPU T4** untuk hasil optimal. ⚡

---

## 🗂️ Dataset

Dataset berasal dari Kaggle: [Intel Image Classification Dataset](https://www.kaggle.com/puneet6060/intel-image-classification).  
Dataset terdiri dari **6 kelas gambar**:
- Buildings 🏢
- Forest 🌲
- Glacier 🧊
- Mountain ⛰️
- Sea 🌊
- Street 🛣️

---

## 📦 Persyaratan

Proyek ini menggunakan library berikut:
```bash
tensorflow
tensorflowjs
numpy
pandas
matplotlib
seaborn
scikit-learn
```

---

## ⚙️ Cara Menjalankan

Untuk menjalankan proyek ini secara lokal atau di Colab:
```
1. Unduh dan tempatkan file `kaggle.json` di direktori `/content/`.
2. Jalankan semua sel dalam notebook Colab (GPU direkomendasikan untuk performa terbaik).
```

---

## ▶️ Penggunaan

1. Unduh dataset dari Kaggle.
2. Jalankan notebook: `Notebook_Submission_Klasifikasi_Gambar.ipynb`
3. Ikuti alur mulai dari:
   - Preprocessing dan augmentasi data
   - Pembuatan dan pelatihan model
   - Evaluasi performa model

---

## 🏗️ Arsitektur Model

Model CNN dibangun menggunakan Keras Sequential API dengan komponen:
- Beberapa blok `Conv2D + MaxPooling2D`
- `Dropout` untuk regularisasi
- `Flatten` layer
- Dense layer dengan aktivasi `relu`
- Output layer: `Dense(6, activation='softmax')`

Loss: `categorical_crossentropy`  
Optimizer: `Adam`  
Metrik: `accuracy`

---

## 🏋️ Pelatihan dan Evaluasi

Model dilatih selama **20 epoch**.  
📈 **Hasil utama:**
- Akurasi Training: 98.78%
- Akurasi Validasi: 85.58%
- Akurasi Testing: 85.09%

📉 **Overfitting ringan** terdeteksi, tapi performa validasi tetap stabil.

---

## 📊 Hasil

📋 **Classification Report (Test set):**
- Accuracy: 85.09%
- Macro Avg F1-score: 0.8515
- Precision tertinggi: *Forest*, *Sea*
- Precision terendah: *Buildings*

---

## 🤝 Kontribusi

Proyek ini merupakan bagian dari submission Dicoding:

- **Nama:** Richelle Vania Thionanda  
- **Email:** mc172d5x1392@student.devacademy.id  
- **ID Dicoding:** MC172D5X1392  

---
