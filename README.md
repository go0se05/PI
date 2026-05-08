# Analisis Sentimen Fenomena #KABURAJADULU Menggunakan Random Forest

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-orange.svg)](https://scikit-learn.org/)
[![NLP](https://img.shields.io/badge/NLP-Sastrawi-green.svg)](https://github.com/sastrawi/sastrawi)

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk melakukan analisis sentimen terhadap fenomena **#KABURAJADULU** yang viral di media sosial X (sebelumnya Twitter). Fenomena ini berkaitan dengan diskursus kewarganegaraan dan keresahan sosial di Indonesia. Dengan menggunakan algoritma **Random Forest**, penelitian ini mengklasifikasikan opini masyarakat ke dalam kategori sentimen tertentu untuk memahami persepsi publik secara otomatis.

## 📊 Hasil Karya
- **Dataset:** Mengolah lebih dari 15.000 data tweet mentah (setelah pembersihan menjadi ~8.700 data unik).
- **Akurasi Model:** Menggunakan algoritma klasifikasi Random Forest dengan optimasi parameter.
- **Visualisasi:** Menyajikan distribusi sentimen melalui grafik dan kata-kata kunci yang paling sering muncul menggunakan *WordCloud*.

## 📂 Isi Repositori & Alur Kerja
File utama dalam proyek ini adalah `pi_kad_nofen.ipynb` yang mencakup tahapan-tahapan berikut:

1.  **Loading Dataset:** Mengambil data dari file CSV yang bersumber dari hasil *crawling* media sosial X.
2.  **Data Cleaning:** * Penanganan nilai kosong (*missing values*).
    * Penghapusan data duplikat untuk menjaga kualitas data.
3.  **Preprocessing (NLP):**
    * **Case Folding:** Menyeragamkan huruf menjadi kecil.
    * **Filtering & Labelling:** Membersihkan teks dari simbol, URL, dan memberikan label sentimen.
    * **Tokenizing:** Memecah kalimat menjadi kata-kata.
    * **Stemming:** Mengubah kata ke bentuk dasar menggunakan library *Sastrawi*.
4.  **Feature Extraction:** Menggunakan *TF-IDF Vectorizer* atau *Count Vectorizer* untuk mengubah teks menjadi bentuk numerik yang dapat dipahami mesin.
5.  **Modeling:** Pelatihan model klasifikasi menggunakan **Random Forest Classifier**.
6.  **Evaluation:** Pengujian model menggunakan *Confusion Matrix* dan *Classification Report* (Precision, Recall, F1-Score).

## 🛠️ Teknologi yang Digunakan
- **Bahasa Pemrograman:** Python
- **Library Utama:**
    - `Pandas` & `NumPy` (Manipulasi Data)
    - `Scikit-Learn` (Machine Learning)
    - `NLTK` & `Sastrawi` (Natural Language Processing)
    - `Matplotlib` & `Seaborn` (Visualisasi Data)
    - `WordCloud` (Analisis Kata Kunci)
