# PBA: Sentiment Analysis M-Paspor 🛂
Tugas 1-A: Pemrosesan Bahasa Alami (NLP)

## Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis sentimen pengguna aplikasi **M-Paspor** di Google Play Store. Fokus utama tahap ini adalah *Data Acquisition* dan *Preprocessing* hingga tahap **Tokenisasi**.

## Prosedur Preprocessing
1. **Scrapping**: Mengambil data menggunakan `google-play-scraper`.
2. **Cleaning**: Menghapus simbol, angka, dan URL.
3. **Normalisasi**: Mengubah kata tidak baku menggunakan *Colloquial Indonesian Lexicon*.
4. **Stemming**: Mencari kata dasar menggunakan library `Sastrawi`.
5. **Tokenisasi**: Memecah kalimat menjadi token kata tunggal.

## Sumber Referensi (Reviewer Insights)
- Kamus Alay: nasalsabila/kamus-alay
- Lexicon: fajri91/InSet
- Stopwords: louisowen6/NLP_bahasa_resources

