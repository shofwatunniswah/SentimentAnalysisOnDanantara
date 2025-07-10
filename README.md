# Analisis Sentimen pada Pemberitaan Danantara Menggunakan NLP

Penelitian ini berfokus pada analisis sentimen masyarakat terhadap "Danantara" melalui pendekatan Natural Language Processing (NLP) pada artikel-artikel berita. Tujuannya adalah untuk mengeksplorasi konten berita, mengidentifikasi kata kunci dominan, serta memahami tren sentimen seiring waktu. Proyek ini juga membandingkan performa model klasifikasi sentimen, yaitu Logistic Regression dengan fitur TF-IDF dan model berbasis BERT.

| **Judul** | **Penulis** | **Tanggal** | **Output** |
| :------------------------------------------------------------------------------------------------------------ | :---------- | :------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Analisis Sentimen pada Pemberitaan Danantara Menggunakan Natural Language Processing (NLP) | Diva Ardelia Alyadrus (5026221029), Shof Watun Niswah 	(5026221043), Muhammad Daffa Alvinoer Rahman 	(5026221180) | 06/05/2025 | `Link_Scraping_Danantara.csv`, `Scraping_Danantara.csv`, `Danantara_Preprocessed.csv`, `Danantara_Augmented_Preprocessed.csv` |

## Struktur Repositori
```
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

```
---

## Daftar Isi

- [Ikhtisar Proyek](#ikhtisar-proyek)
- [Tujuan](#tujuan)
- [Metode yang Digunakan](#metode-yang-digunakan)
- [Alur Pengerjaan](#alur-pengerjaan)
- [Notebooks](#notebooks)
- [Dataset](#dataset)

## Ikhtisar Proyek

Proyek ini berfokus pada pemahaman opini publik terhadap Danantara melalui analisis sentimen dari artikel-artikel berita daring. Teknik NLP diterapkan untuk proses pembersihan, ekstraksi fitur, dan klasifikasi sentimen, serta membandingkan dua model klasifikasi utama.

## Tujuan

- Menganalisis sentimen publik terhadap Danantara.
- Mengidentifikasi kata kunci dominan dalam pemberitaan.
- Mempelajari tren sentimen dari waktu ke waktu.
- Membandingkan performa model Logistic Regression dengan TF-IDF dan model BERT.

## Metode yang Digunakan

- **Analisis Sentimen**: Mengelompokkan teks menjadi sentimen positif, negatif, atau netral.
- **TF-IDF** (*Term Frequency–Inverse Document Frequency*): Ekstraksi fitur dari teks berdasarkan frekuensi kata.
- **POS Tagging** (*Part-of-Speech Tagging*): Klasifikasi kata berdasarkan kategori gramatikal.
- **Named Entity Recognition (NER)**: Deteksi entitas penting seperti nama orang, organisasi, atau lokasi.

## Alur Pengerjaan

1. **Pengumpulan Link Berita**  
   Link dikumpulkan secara manual dan disimpan dalam `Link_Scraping_Danantara.csv`.

2. **Scraping Konten Berita**  
   Konten dari link yang terkumpul diambil menggunakan `newspaper3k` dan disimpan dalam `Scraping_Danantara.csv`. Proses ini dilakukan di notebook `Scrap_Danantara_TERBARU.ipynb`.

3. **Preprocessing Teks**  
   Dilakukan pembersihan teks (case folding, stopwords removal, dll.) menggunakan notebook `PREPROCESSING_DANANTARA.ipynb`, menghasilkan `Danantara_Preprocessed.csv`.

4. **Augmentasi Data**  
   Variasi data ditambahkan untuk memperkaya representasi menggunakan notebook `augmentasi_part2.ipynb`, hasilnya disimpan di `Danantara_Augmented_Preprocessed.csv`.

5. **Analisis Linguistik dan Ekstraksi Fitur**  
   - Analisis kata penting dilakukan dengan TF-IDF pada `TFIDF_Analysis_Danantara.ipynb`.
   - POS Tagging dan Named Entity Recognition dilakukan pada `POS_dan_NER.ipynb`.

6. **Analisis Sentimen dan Evaluasi Model**  
   Evaluasi dua model klasifikasi sentimen dilakukan melalui:
   - `PERBANDINGAN_LOGREG_TFIDF_VS_BERT.ipynb`
   - `Perbandingan_LogReg_vs_BERT_Final.ipynb` (ringkasan lengkap)

## Notebooks

| Notebook | Deskripsi |
|----------|-----------|
| `Scrap_Danantara_TERBARU.ipynb` | Scraping berita dari link yang tersedia |
| `PREPROCESSING_DANANTARA.ipynb` | Preprocessing teks berita |
| `augmentasi_part2.ipynb` | Augmentasi data untuk memperkaya dataset |
| `TFIDF_Analysis_Danantara.ipynb` | Analisis fitur kata menggunakan TF-IDF |
| `POS_dan_NER.ipynb` | Analisis linguistik dengan POS Tagging dan NER |
| `PERBANDINGAN_LOGREG_TFIDF_VS_BERT.ipynb` | Evaluasi dua model klasifikasi |
| `Perbandingan_LogReg_vs_BERT_Final.ipynb` | Notebook utama perbandingan model |

## Dataset

- `Link_Scraping_Danantara.csv`  
  Daftar URL berita yang dikumpulkan secara manual.

- `Scraping_Danantara.csv`  
  Konten mentah dari artikel berita hasil scraping.

- `Danantara_Preprocessed.csv`  
  Teks hasil preprocessing untuk keperluan analisis.

- `Danantara_Augmented_Preprocessed.csv`  
  Dataset hasil augmentasi untuk meningkatkan keragaman data.

