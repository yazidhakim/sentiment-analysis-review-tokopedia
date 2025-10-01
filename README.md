# sentiment-analysis-review-tokopedia

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan produk di Tokopedia menggunakan teknik **Natural Language Processing (NLP)** dan model **Machine Learning**. Sentimen dalam ulasan akan diklasifikasikan ke dalam kategori **positif**, **negatif**, atau **netral**.

🎯 **Tujuan**  
Membangun model klasifikasi untuk memprediksi sentimen pada ulasan produk di Tokopedia.  
Membantu bisnis dalam memahami feedback pelanggan dan meningkatkan produk.

📁 **Dataset Overview**  
Jumlah data: 10.000+ ulasan, 5 fitur utama  
Beberapa fitur penting:
- **Content**: Teks ulasan dari pelanggan
- **Score**: Rating yang diberikan pelanggan (1-5)
- **Label**: Sentimen pelanggan yang dihasilkan oleh model (Positif/Negatif/Netral)
- **Date**: Tanggal ulasan diterima

Label target: **Sentiment** (positif, negatif, netral) yang digunakan untuk membangun model klasifikasi.

🧠 **Skema Model**  
### **Skema 1: SVM + TF-IDF**
- **TF-IDF (Term Frequency-Inverse Document Frequency)** digunakan untuk transformasi teks menjadi vektor fitur.
- **SVM (Support Vector Machine)** digunakan sebagai model klasifikasi untuk memprediksi sentimen berdasarkan vektor fitur yang dihasilkan oleh TF-IDF.
- **Metode**:  
  - Preprocessing data: Tokenisasi, stopword removal, dan normalisasi.
  - Fitur: TF-IDF untuk representasi teks.
  - Model: SVM untuk klasifikasi.
  
### **Skema 2: Logistic Regression + BoW**
- **BoW (Bag of Words)** digunakan untuk mengubah teks menjadi representasi vektor berdasarkan frekuensi kata.
- **Logistic Regression** digunakan sebagai model klasifikasi untuk memprediksi sentimen berdasarkan vektor fitur yang dihasilkan oleh BoW.
- **Metode**:  
  - Preprocessing data: Tokenisasi, stopword removal, dan normalisasi.
  - Fitur: BoW untuk representasi teks.
  - Model: Logistic Regression untuk klasifikasi.

Evaluasi model yang digunakan:
- **Akurasi**
- **Presisi**
- **Recall**
- **F1-Score**
- **Confusion Matrix**
