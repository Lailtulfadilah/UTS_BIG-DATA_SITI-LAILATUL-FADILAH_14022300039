# UTS_BIG-DATA_SITI-LAILATUL-FADILAH_14022300039
📊 Google Play Review Scraper & Sentiment Analysis (IndoRoBERTa)

Project ini digunakan untuk:

Mengambil (scrape) ulasan aplikasi dari Google Play
Melakukan analisis sentimen menggunakan model AI IndoRoBERTa dari Hugging Face
🚀 Cara Menjalankan (Google Colab)
Buka Google Colab
Scroll ke bawah, buat notebook baru
Install library yang dibutuhkan:
pip install google-play-scraper transformers torch pandas
📥 Scraping Data Ulasan
Copy kode scraping ke Colab
Ganti ID aplikasi sesuai kebutuhan (contoh aplikasi pemerintah):
'id.go.kemensos.pelaporan'
Atur jumlah data:
count=1000  # bisa 100 - 1000
Jalankan kode untuk mengambil ulasan dan menyimpan ke CSV
🤖 Analisis Sentimen (Transformers)

Project ini menggunakan model dari Hugging Face:

IndoRoBERTa Sentiment Classifier
model="w11wo/indonesian-roberta-base-sentiment-classifier"

Model akan mengklasifikasikan ulasan menjadi:

Positive
Neutral
Negative
⚡ Tips Performa (WAJIB di Colab)

Agar proses cepat:

Aktifkan GPU:
Runtime → Change runtime type → GPU
Gunakan batch processing (lebih cepat dari satu-satu)
Batasi data saat testing:
df = df.head(200)
📁 Output

File yang dihasilkan:

ulasan_google_play.csv → hasil scraping
ulasan_dengan_sentimen.csv → hasil + label sentimen
🧠 Teknologi yang Digunakan
Python
google-play-scraper
Transformers (Hugging Face)
IndoRoBERTa
📌 Catatan
Semakin banyak data → semakin lama proses
Disarankan menggunakan GPU di Colab
Model Transformer cukup berat jika dijalankan di CPU
✨ Pengembangan Selanjutnya
Visualisasi data (pie chart / bar chart)
Wordcloud dari ulasan
Dashboard (Streamlit)
Fine-tuning model sendiri
