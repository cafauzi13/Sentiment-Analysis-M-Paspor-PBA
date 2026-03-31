# PBA: Sentiment Analysis M-Paspor 🛂
**Tugas Mata Kuliah Pemrosesan Bahasa Alami (NLP)**

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis sentimen pengguna aplikasi **M-Paspor** di Google Play Store dengan menarik lebih dari **20.000 ulasan**. Analisis ini mencakup alur lengkap NLP mulai dari pembersihan data hingga ekstraksi fitur numerik untuk persiapan pemodelan Machine Learning.

---

## 📂 Struktur Repositori
| Folder | Deskripsi Materi | Progres Utama |
| :--- | :--- | :--- |
| `Week 1/` | **Basics & Tokenization** | Setup NLTK & latihan tokenisasi sampel ulasan. |
| `Week 2/` | **Preprocessing & Scraping** | Scraping 20k ulasan & Stemming Sastrawi (Data 1A). |
| `Week 3/` | **EDA, BoW & Regex** | Analisis frekuensi kata dan pola ulasan spesifik. |
| `Week 4/` | **Feature Extraction** | Implementasi TF-IDF Vectorizer & Cosine Distance. |

---

## 🛠️ NLP Pipeline & Prosedur
Proses pengolahan data dilakukan melalui tahapan berikut:

1.  **Scraping**: Mengambil ulasan (ID & EN) menggunakan `google-play-scraper`.
2.  **Cleaning**: Menghapus simbol, angka, dan URL menggunakan **Regex**.
3.  **Normalisasi**: Mengubah kata "alay" menggunakan *Colloquial Indonesian Lexicon*.
4.  **Stemming**: Mengubah kata berimbuhan menjadi kata dasar dengan `Sastrawi`.
5.  **Tokenisasi**: Memecah kalimat menjadi unit kata tunggal (`tokens`).
6.  **Bag of Words (BoW)**: Menghitung frekuensi kemunculan kata dalam korpus.
7.  **TF-IDF**: Memberikan bobot pada kata berdasarkan tingkat kepentingan dan keunikannya.

---

## 🔍 Analisis Sentimen & Referensi
Kami menggunakan metode **Lexicon-Based** untuk pelabelan awal sebelum masuk ke tahap pelatihan model:

* **Sentiment Scoring**: Menggunakan **InSet Lexicon** (Fajri dkk.) untuk menentukan bobot positif/negatif ulasan.
* **Kamus Alay**: [nasalsabila/kamus-alay](https://github.com/nasalsabila/kamus-alay).
* **Stopwords**: Gabungan sumber dari [louisowen6](https://github.com/louisowen6/NLP_bahasa_resources).

---

## 🚀 Cara Menjalankan
1. Clone repositori ini.
2. Pastikan file dataset `.csv` berada dalam folder yang sama dengan Notebook.
3. Jalankan `.ipynb` pada setiap folder secara berurutan (Week 1 -> Week 4).

---

