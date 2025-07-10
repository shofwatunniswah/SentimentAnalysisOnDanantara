🧠 Analisis Sentimen terhadap Pemberitaan Danantara Menggunakan NLP
Penelitian ini bertujuan untuk menganalisis sentimen masyarakat terhadap Danantara melalui pendekatan Natural Language Processing (NLP) pada artikel-artikel berita.

Beberapa metode yang digunakan dalam penelitian ini meliputi:

Analisis Sentimen

TF-IDF

POS Tagging

Named Entity Recognition (NER)

Metode-metode tersebut digunakan untuk mengeksplorasi konten berita, mengidentifikasi kata kunci yang dominan, serta memahami tren sentimen dari waktu ke waktu.
Penelitian ini juga membandingkan performa dua model klasifikasi sentimen, yaitu Logistic Regression dengan fitur TF-IDF dan model berbasis BERT.

🔁 Alur Pengerjaan

1. Pengumpulan link berita secara manual
→ Link_Scraping_Danantara.csv

2. Scraping konten berita menggunakan newspaper3k
→ Notebook: Scrap_Danantara_TERBARU.ipynb
→ Output: Scraping_Danantara.csv

3. Preprocessing teks berita
→ Notebook: PREPROCESSING_DANANTARA.ipynb
→ Output: Danantara_Preprocessed.csv

4. Augmentasi data
→ Notebook: augmentasi part2.ipynb
→ Output: Danantara_Augmented_Preprocessed.csv

5. Eksplorasi Teks dan Analisis Linguistik

TF-IDF Analysis → TFIDF_Analysis_Danantara.ipynb

POS Tagging & Named Entity Recognition → POS_dan_NER.ipynb

6. Analisis Sentimen dan Perbandingan Model
→ Notebook: Perbandingan_Analisis_Sentimen_pada_Pemberitaan_Danantara_Menggunakan_Model_Logistic_Regression_dengan_Feature_Engineering_TF_IDF_dan_BERT.ipynb
