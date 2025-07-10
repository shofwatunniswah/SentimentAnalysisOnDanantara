# Analisis Sentimen pada Pemberitaan Danantara Menggunakan NLP

Penelitian ini berfokus pada analisis sentimen masyarakat terhadap "Danantara" melalui pendekatan Natural Language Processing (NLP) pada artikel-artikel berita. Tujuannya adalah untuk mengeksplorasi konten berita, mengidentifikasi kata kunci dominan, serta memahami tren sentimen seiring waktu. Proyek ini juga membandingkan performa model klasifikasi sentimen, yaitu Logistic Regression dengan fitur TF-IDF dan model berbasis BERT.

| **Judul** | **Penulis** | **Tanggal** | **Output** |
| :------------------------------------------------------------------------------------------------------------ | :---------- | :------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Analisis Sentimen pada Pemberitaan Danantara Menggunakan Natural Language Processing (NLP) | Diva Ardelia Alyadrus (5026221029), Shof Watun Niswah 	(5026221043), Muhammad Daffa Alvinoer Rahman 	(5026221180) | 06/05/2025 | `Link_Scraping_Danantara.csv`, `Scraping_Danantara.csv`, `Danantara_Preprocessed.csv`, `Danantara_Augmented_Preprocessed.csv` |

## Struktur Repositori
📂 SentimentAnalysisOnDanantara
├── Data/                   # Direktori untuk dataset mentah dan yang telah diproses
│   ├── Danantara_Augmented_Preprocessed (1).csv  # Dataset yang telah di-augmentasi dan di-preproses
│   ├── Danantara_Preprocessed.csv                # Dataset yang telah di-preproses
│   ├── Link_Scraping_Danantara (1).csv           # Link berita yang dikumpulkan
│   ├── Scraping_Danantara.csv                    # Konten berita hasil scraping
│
├── Notebooks/              # Jupyter Notebooks untuk analisis
│   ├── PERBANDINGAN_ANALISIS_SENTIMEN_MENGGUNAKAN_LOGISTIC_REGRESSION_+_TF_IDF_DAN_BERT.ipynb  # Perbandingan model sentimen
│   ├── POS_dan_NER.ipynb                                                                       # Analisis POS Tagging dan NER
│   ├── PREPROCESSING_DANANTARA.ipynb                                                           # Notebook untuk preprocessing teks
│   ├── Scrap_Danantara_TERBARU.ipynb                                                           # Notebook untuk scraping konten berita
│   ├── TFIDF_Analysis_Danantara.ipynb                                                          # Analisis TF-IDF
│   ├── augmentasi part2.ipynb                                                                  # Notebook untuk augmentasi data
│
├── Perbandingan_Analisis_Sentimen_pada_Pemberitaan_Danantara_Menggunakan_Model_Logistic_Regression_dengan_Feature_Engineering_TF_IDF_dan_BERT.ipynb  # Notebook utama perbandingan model
├── README.md               # Pengantar proyek (file ini)

## Daftar Isi

- [Ikhtisar Proyek](#ikhtisar-proyek)
- [Metode yang Digunakan](#metode-yang-digunakan)
- [Alur Pengerjaan](#alur-pengerjaan)
- [Notebooks](#notebooks)
- [Data](#data)

---

## Ikhtisar Proyek

Proyek ini melakukan analisis sentimen terhadap pemberitaan tentang "Danantara" dengan memanfaatkan teknik Natural Language Processing (NLP). Tujuan utamanya adalah untuk mendapatkan pemahaman mendalam mengenai opini dan pandangan yang terekspresikan dalam artikel berita.

### Tujuan

- Menganalisis sentimen publik terhadap Danantara.
- Mengidentifikasi kata kunci dominan dalam pemberitaan.
- Memahami tren sentimen dari waktu ke waktu.
- Membandingkan performa model klasifikasi sentimen Logistic Regression dengan fitur TF-IDF dan model berbasis BERT.

## Metode yang Digunakan

Beberapa metode NLP yang diterapkan dalam penelitian ini meliputi:

-   **Analisis Sentimen**: Untuk mengklasifikasikan teks berita ke dalam kategori sentimen (positif, negatif, netral).
-   **TF-IDF (Term Frequency-Inverse Document Frequency)**: Digunakan untuk ekstraksi fitur teks dan identifikasi kata kunci penting.
-   **POS Tagging (Part-of-Speech Tagging)**: Untuk mengidentifikasi kategori gramatikal kata.
-   **Named Entity Recognition (NER)**: Untuk mengidentifikasi dan mengklasifikasikan entitas bernama dalam teks.

---

## Alur Pengerjaan

Penelitian ini mengikuti alur pengerjaan berikut:

1.  **Pengumpulan Link Berita Secara Manual**: Link berita dikumpulkan secara manual dan disimpan dalam `Link_Scraping_Danantara.csv`.
2.  **Scraping Konten Berita**: Konten berita di-scrape menggunakan `newspaper3k` melalui notebook `Scrap_Danantara_TERBARU.ipynb`, dengan output `Scraping_Danantara.csv`.
3.  **Preprocessing Teks Berita**: Teks berita di-preproses menggunakan notebook `PREPROCESSING_DANANTARA.ipynb`, menghasilkan `Danantara_Preprocessed.csv`.
4.  **Augmentasi Data**: Data di-augmentasi menggunakan notebook `augmentasi part2.ipynb`, dengan output `Danantara_Augmented_Preprocessed.csv`.
5.  **Eksplorasi Teks dan Analisis Linguistik**:
    * Analisis TF-IDF dilakukan dalam `TFIDF_Analysis_Danantara.ipynb`.
    * POS Tagging dan Named Entity Recognition dilakukan dalam `POS_dan_NER.ipynb`.
6.  **Analisis Sentimen dan Perbandingan Model**: Analisis sentimen dan perbandingan model dilakukan dalam notebook `Perbandingan_Analisis_Sentimen_pada_Pemberitaan_Danantara_Menggunakan_Model_Logistic_Regression_dengan_Feature_Engineering_TF_IDF_dan_BERT.ipynb`.

---

## Notebooks

Proyek ini dibagi menjadi beberapa Jupyter Notebooks yang mencakup berbagai tahapan analisis:

1.  **Scrap_Danantara_TERBARU.ipynb**: Mengumpulkan konten berita Danantara dari link yang telah dikumpulkan.
2.  **PREPROCESSING_DANANTARA.ipynb**: Melakukan tahapan pembersihan dan normalisasi teks berita.
3.  **augmentasi part2.ipynb**: Melakukan augmentasi data untuk memperkaya dataset.
4.  **TFIDF_Analysis_Danantara.ipynb**: Menerapkan TF-IDF untuk analisis fitur teks dan identifikasi kata kunci.
5.  **POS_dan_NER.ipynb**: Menganalisis Part-of-Speech (POS) Tagging dan Named Entity Recognition (NER) pada teks.
6.  **PERBANDINGAN_ANALISIS_SENTIMEN_MENGGUNAKAN_LOGISTIC_REGRESSION_+_TF_IDF_DAN_BERT.ipynb**: Membandingkan performa model Logistic Regression dengan TF-IDF dan BERT untuk klasifikasi sentimen.
7.  **Perbandingan_Analisis_Sentimen_pada_Pemberitaan_Danantara_Menggunakan_Model_Logistic_Regression_dengan_Feature_Engineering_TF_IDF_dan_BERT.ipynb**: Notebook utama yang merangkum perbandingan model sentimen.

---

## Data

Proyek ini menggunakan dataset berikut:

1.  **Link_Scraping_Danantara (1).csv**: Berisi daftar link berita yang menjadi sumber data.
2.  **Scraping_Danantara.csv**: Mengandung konten berita mentah yang di-scrape dari link.
3.  **Danantara_Preprocessed.csv**: Versi data yang telah dibersihkan dan di-preproses.
4.  **Danantara_Augmented_Preprocessed (1).csv**: Data yang telah di-augmentasi dan siap untuk analisis lebih lanjut.
