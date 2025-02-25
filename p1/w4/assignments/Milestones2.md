# Phase 1 Milestone 2

_Milestones ini dibuat guna mengevaluasi pembelajaran pada Hacktiv8 Data Science Fulltime Program khususnya pada Phase 1._

---

Untuk *Milestones 2*, student akan membuat sebuah model machine learning dengan beberapa pilihan kasus dan panduan yang harus diikuti berikut ini.

## Topik

Silakan memilih topik *Milestones 2* antara *Regression*, *Classification* atau *Clustering*. Student juga dipersilakan memilih topik mengenai *Anomaly Detection*, *Novelty Detection* hingga *Dimensionality Reduction*. Beberapa contoh kasus dari masing-masing topik adalah sebagai berikut:

- Regression: [House Pricing](), [NYC Taxi Fare Prediction](), [Wallmart Sales in Stormy Weather](), dll
- Classification: [SF Crime Classification](), [Wallmart Trip Type](), [Titanic](), dll
- Clustering: [Human Activity Recognition](), [Credit Card Clustering](), [Household Electric Consumption](), dll

## Data Sources

Student dapat memilih dataset dari salah satu repository dibawah ini. Pilihlah dataset yang paling nyaman digunakan karena tidak ada batasan untuk memilih dataset dalam mengerjakan *Milestones 2*. Konsultasikan terlebih dahulu dataset yang hendak digunakan ke buddy masing-masing student. Jika disetujui, maka silakan dikerjakan. Jika tidak disetujui, maka cari dataset yang lain dan konsultasikan lagi mengenai dataset yang baru ini.

Popular open data repositories

- [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- [Kaggle datasets](https://www.kaggle.com/datasets)
- [Amazon’s AWS datasets](https://registry.opendata.aws/)

Meta portals (they list open data repositories)

- [Data Portals](http://dataportals.org/)
- [OpenDataMonitor](https://opendatamonitor.eu/frontend/web/index.php?r=dashboard%2Findex)
- [Quandl](https://www.quandl.com/)

Other pages listing many popular open data repositories

- [Wikipedia’s list of Machine Learning datasets](https://en.wikipedia.org/wiki/List_of_datasets_for_machine-learning_research)
- [Quora.com](https://www.quora.com/Where-can-I-find-large-datasets-open-to-the-public)
- [The datasets subreddit](https://www.reddit.com/r/datasets)
- Sumber lain yang kredibel.
- **Student dilarang untuk melakukan scraping dataset** karena dikhawatirkan proses pembuatan scraper dan proses scraping akan memakan waktu. Gunakan public dataset yang tersedia diberbagai macam situs Internet.

## Assignment Instructions

*Milestones 2* dikerjakan dalam format ***notebook*** dengan ***model deployment (opsional)*** dengan beberapa *kriteria wajib* di bawah ini:

1. Machine learning framework yang digunakan adalah *Scikit-Learn*.

2. Ada penggunaan library visualisasi, seperti *matplotlib*, *seaborn*, atau yang lain.

3. Isi *notebook* harus mengikuti *outline* di bawah ini:
   1. Perkenalan
      > Bab pengenalan harus diisi dengan identitas, gambaran besar dataset yang digunakan, dan *objective* yang ingin dicapai.
   
   2. Import Libraries
      > *Cell* pertama pada *notebook* **harus berisi dan hanya berisi** semua *library* yang digunakan dalam *project*.
   
   3. Data Loading
      > Bagian ini berisi proses penyiapan data sebelum dilakukan eksplorasi data lebih lanjut. Proses Data Loading dapat berupa memberi nama baru untuk setiap kolom, mengecek ukuran dataset, dll.
   
   4. Exploratory Data Analysis (EDA)
      > Bagian ini berisi explorasi data pada dataset diatas dengan menggunakan query, grouping, visualisasi sederhana, dan lain sebagainya.
   
   5. Data Preprocessing
      > Bagian ini berisi proses penyiapan data untuk proses pelatihan model, seperti pembagian data menjadi train-dev-test, transformasi data (normalisasi, encoding, dll.), dan proses-proses lain yang dibutuhkan.   
   
   6. Model Definition
      > Bagian ini berisi cell untuk mendefinisikan model. Jelaskan alasan menggunakan suatu algoritma/model, hyperparameter yang dipakai, jenis penggunaan metrics yang dipakai, dan hal lain yang terkait dengan model.

   7. Model Training
      > Cell pada bagian ini hanya berisi code untuk melatih model dan output yang dihasilkan. Lakukan beberapa kali proses training dengan hyperparameter yang berbeda untuk melihat hasil yang didapatkan. Analisis dan narasikan hasil ini pada bagian Model Evaluation.
   
   8. Model Evaluation
      > Pada bagian ini, dilakukan evaluasi model yang harus menunjukkan bagaimana performa model berdasarkan metrics yang dipilih. Hal ini harus dibuktikan dengan visualisasi tren performa dan/atau tingkat kesalahan model. **Lakukan analisis terkait dengan hasil pada model dan tuliskan hasil analisisnya**.

   9. Model Saving
      > Dengan melihat hasil evaluasi model, pilihlah model terbaik untuk disimpan. Model terbaik ini akan digunakan kembali dalam melakukan deployment di Heroku.
   
   10. Model Inference
      > Model yang sudah dilatih akan dicoba pada data yang bukan termasuk ke dalam train-set ataupun test-set. Data ini harus dalam format yang asli, bukan data yang sudah di-scaled.
   
   11. Pengambilan Kesimpulan
       > Pada bagian terakhir ini, **harus berisi** kesimpulan yang mencerminkan hasil yang didapat dengan *objective* yang sudah ditulis di bagian pengenalan.

5. *Notebook* harus diupload dalam akun GitHub masing-masing siswa untuk selanjutnya dinilai.

6. Penilaian project dilakukan berdasarkan *notebook* dan *service/API* model yang sudah di-deploy (jika melakukan Model Deployment).

7. Presentasikan model yang telah dibuat pada P2W1D4PM.

## Assignment Submission

- Simpan assignment pada sesi ini dengan nama `h8dsft_Milestone2P1_<nama-student>.ipynb`, misal `h8dsft_Milestone2P1_raka_ardhi.ipynb`.
- Push assignment yang telah dibuat ke akun Github masing-masing.
- Jika melakukan Model Deployment ke Heroku :
  * Push juga semua file yang berkaitan dengan deployment ke repository. Akan lebih bagus jika semua file deployment berada dalam satu folder yang sama.
  * Buat sebuah file bernama `url.txt` yang berisi URL Dataset dan URL deployment.

## Assignment Objectives

*Milestones 2* ini dibuat guna mengevaluasi Pembelajaran Phase 1:

- Mampu memahami konsep supervised learning
- Mampu mempersiapkan data untuk digunakan dalam model supervised learning
- Mampu mengimplementasikan supervised learning dengan data yang diberikan
- Mampu melakukan evaluasi model
- Mampu melakukan model tuning

---

## Assignment Rubrics

### Code Review

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Feature Engineering | Mampu melakukan proses Feature Engineering sebelum melakukan proses modeling | 30 pts |
| Pipelines | Mampu membangun Pipeline | 40 pts |
| Modeling | Membuat model dengan kasus yang dipilih dengan Scikit-Learn | 40 pts |
| Model Evaluation | Mampu melakukan model evaluation dengan Scikit-Learn | 30 pts |
| Model Improvement | Mampu melakukan model improvement dengan Scikit-Learn | 40 pts |
| Model Inference | Mencoba model yang telah dibuat dengan data baru | 20 pts |
| Apakah Kode Berjalan Tanpa Ada Error? | Kode berjalan tanpa ada error. Seluruh kode berfungsi dan dibuat dengan benar. | 10 pts |

### Readability

| Criteria | Meet Expectations | Points|
| --- | --- | --- |
| Tertata Dengan Baik | Semua baris kode terdokumentasi dengan baik dengan menggunakan Markdown untuk penjelasan kode. | 10 pts |

### Analysis

| Criteria | Meet Expectations | Points|
| --- |--- |--- |
| Model Analysis | Menganalisa informasi dari model yang telah dibuat | 30 pts |
| Overall Analysis | Menarik informasi/kesimpulan dari keseluruhan kegiatan yang dilakukan | 20 pts |


### Model Deployment (Bonus Point) (Optional)

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Model Deployment | Membuat webapps terhadap project yang telah dibuat. | 30 pts |

---

```
Total Points (tanpa Deployment)  : 270
Total Points (dengan Deployment) : 300
```

---

## Score Reduction

Pengurangan poin akan diberlakukan jika Student terlambat mengumpulkan tugas yang telah diberikan. Adapun besarnya pengurangan adalah : 

| Criteria | Max Points Milesone 2 |
| --- | --- |
| Keterlambatan kurang dari 6 jam setelah deadline | 75 % dari total points |
| Keterlambatan lebih dari 6 jam setelah deadline | 0% dari total points |
