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
Pengumpulan link berita secara manual
→ Link_Scraping_Danantara.csv

Scraping konten berita menggunakan newspaper3k
→ Notebook: Scrap_Danantara_TERBARU.ipynb
→ Output: Scraping_Danantara.csv

Preprocessing teks berita
→ Notebook: PREPROCESSING_DANANTARA.ipynb
→ Output: Danantara_Preprocessed.csv

Augmentasi data
→ Notebook: augmentasi part2.ipynb
→ Output: Danantara_Augmented_Preprocessed.csv

Eksplorasi Teks dan Analisis Linguistik

TF-IDF Analysis → TFIDF_Analysis_Danantara.ipynb

POS Tagging & Named Entity Recognition → POS_dan_NER.ipynb

Analisis Sentimen dan Perbandingan Model
→ Notebook: Perbandingan_Analisis_Sentimen_pada_Pemberitaan_Danantara_Menggunakan_Model_Logistic_Regression_dengan_Feature_Engineering_TF_IDF_dan_BERT.ipynb
