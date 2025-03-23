# Tokopedia Sentiment Analysis

Ini merupakan project dari submission pertama pada **Belajar Pengembangan Machine Learning** di Dicoding. Pada project ini, saya melakukan **sentimen analisis** pada aplikasi Tokopedia dengan menggunakan data ulasan (*reviews*) dari aplikasi yang ada di **Google Play Store**.

## 📌 Objectives
Analisis ini bertujuan untuk:
- Mengidentifikasi pola sentimen pengguna terhadap aplikasi Tokopedia.
- Membantu pihak Tokopedia memahami kepuasan pelanggan melalui analisis ulasan.
- Mengembangkan model Machine Learning untuk mengklasifikasikan sentimen ulasan secara otomatis.


## 📑 Methodology

### 1️⃣ Scraping Data
- Melakukan scraping data secara mandiri yang bersumber dari **Google Play Store**.
- Mengambil **30.000 total ulasan** yang merepresentasikan opini pengguna.
- Menggunakan library `google-play-scraper` untuk mengambil ulasan.

### 2️⃣ Text Preprocessing
- Membersihkan teks dengan menghapus angka, tanda baca, dan karakter khusus.
- Mengubah teks menjadi huruf kecil dan menghapus *stopwords*.
- Melakukan *tokenization* (memecah teks menjadi kata-kata individu), *stemming* (mengubah kata ke bentuk dasar agar lebih seragam), dan mengubah kata tidak baku (slang) ke bentuk standar untuk normalisasi teks.

### 3️⃣ Sentiment Categorization
- Menggunakan metode **Lexicon-Based Analysis** untuk mengkategorikan sentimen ulasan.
- Menggunakan kamus kata positif dan negatif untuk menentukan polaritas ulasan.

### 4️⃣ Exploratory Data (EDA)
- Melihat distribusi jumlah ulasan berdasarkan sentimen.
- Analisis kata-kata yang paling sering muncul dalam ulasan.

### 5️⃣ Feature Extraction
- Menggunakan teknik **tokenisasi dan padding** untuk mengubah teks menjadi representasi numerik.
- Memanfaatkan `Tokenizer` dari Keras untuk memproses teks ulasan.

### 6️⃣ Model Training
Membangun model deep learning untuk klasifikasi sentimen:
- **LSTM (Long Short-Term Memory)** → Model utama yang digunakan karena kemampuannya dalam menangani data sequential.
- **GRU (Gated Recurrent Unit)** → Alternatif model yang lebih ringan dibandingkan LSTM.
- **RNN (Recurrent Neural Network)** → Model dasar sebagai perbandingan.

### 7️⃣ Model Evaluation
- Menggunakan **akurasi, precision, recall, dan F1-score** untuk mengukur performa model.
- Membandingkan hasil antar model untuk memilih yang terbaik.


## 📊 Submission Review

![Submission Score]([https://github.com/user-attachments/assets/4e13c229-3d5e-4880-bd73-a15ce7c789a3])

## 📌 Conclusion
Pada project ini, saya melakukan **analisis sentimen** dengan pendekatan **lexicon-based** dan **deep learning**. Tiga model deep learning dikomparasi untuk melihat performa masing-masing model. Model ini nantinya dapat digunakan untuk menganalisis sentimen ulasan baru secara otomatis, yang dapat membantu dalam memahami kepuasan pengguna dan meningkatkan kualitas layanan aplikasi mereka.



**Author:** Mellisa  
**Date:** 09-11-2024  
**Tools:** Python, TensorFlow, Keras, Google Play Scraper, Pandas, NLTK
