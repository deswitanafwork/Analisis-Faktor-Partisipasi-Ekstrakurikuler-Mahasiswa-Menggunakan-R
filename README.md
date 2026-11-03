# Analisis-Faktor-Partisipasi-Ekstrakurikuler-Mahasiswa-Menggunakan-R
End-to-end data analysis Analisis Faktor Partisipasi Ekstrakurikuler Mahasiswa Menggunakan R

Tingkat partisipasi mahasiswa dalam kegiatan ekstrakurikuler seringkali bervariasi dan dipengaruhi oleh ragam faktor demografis serta akademis. Untuk mengoptimalkan program kemahasiswaan, institusi pendidikan membutuhkan pemahaman berbasis data mengenai karakteristik mahasiswa yang aktif berpartisipasi. Oleh karena itu, diperlukan analisis statistik mendalam guna mengukur pengaruh variabel seperti usia, gender, jurusan, dan status pekerjaan paruh waktu terhadap keputusan mahasiswa.

Sebagai Data Analyst, saya melakukan pengolahan data eksploratif, uji hipotesis, dan pemodelan regresi logistik terhadap 500 baris data observasi mahasiswa. Proses ini bertujuan untuk memberikan wawasan berbasis data (*data-driven insight*) mengenai peluang dan risiko partisipasi mahasiswa, sehingga pihak universitas atau manajemen akademik dapat merancang strategi peningkatan keterlibatan mahasiswa secara lebih terarah, inklusif, dan objektif.

# **Import Library & Tech Stack**
Ekstraksi, pemrosesan, dan pemodelan pada projek ini dibangun di atas lingkungan bahasa pemrograman R menggunakan *Tech Stack* analitik berikut:

* **R (dplyr, readr):** Digunakan untuk ekstraksi data dari format CSV, manipulasi *dataframe* secara efisien, pembuatan variabel biner, serta agregasi proporsi data.


* **Base R (Stats):** Dimanfaatkan secara intensif untuk pengujian hipotesis (Z-Test), perhitungan *Confidence Interval* (CI) 95%, komputasi *Relative Risk* (RR) dan *Odds Ratio* (OR), serta pembangunan algoritma Regresi Logistik (GLM).



# **Pengumpulan Data**
Dataset yang dianalisis mencakup 500 data observasi dengan 9 metrik atau variabel utama. Variabel yang dieksplorasi meliputi ID Siswa, Gender, Usia, Jam Belajar per Minggu, Tingkat Kehadiran, IPK, Jurusan (*Arts, Business, Education, Science, Engineering*), Status Pekerjaan Paruh Waktu, serta Status Partisipasi Ekstrakurikuler sebagai variabel target.

**Preprocessing & Feature Engineering**
Pendekatan *preprocessing* dilakukan agar data siap dievaluasi menggunakan metode statistik lanjutan:

* **Data Transformation:** Mengonversi variabel kategorikal ("Yes"/"No" pada Partisipasi Ekstrakurikuler dan Pekerjaan Paruh Waktu) menjadi representasi biner numerik (1 dan 0) agar dapat diproses oleh model algoritma regresi.


* **Proportion Grouping:** Melakukan segmentasi agregat berdasarkan variabel prediktor (Gender, Jurusan, dan Pekerjaan Paruh Waktu) untuk menemukan rata-rata rasio keberhasilan partisipasi pada masing-masing kelompok demografi.



# **Pengujian Statistik & Pemodelan Prediktif**
Tahap ini memuat analisis inferensial untuk menemukan korelasi dan probabilitas antar variabel:

* **Hypothesis Testing & Confidence Intervals (CI):** Melakukan evaluasi proporsi sampel menggunakan nilai Z (*Z-value* 1.96) dan menghitung rentang *Confidence Interval* 95% untuk memvalidasi apakah perbedaan partisipasi antar kelompok (misalnya antara laki-laki dan perempuan) terbukti signifikan secara statistik.


* **Risk & Odds Analysis:** Mengkalkulasi *Relative Risk* (RR) dan *Odds Ratio* (OR) beserta nilai *Standard Error* untuk mengukur seberapa besar kecenderungan suatu kelompok mahasiswa untuk berpartisipasi dibandingkan kelompok lainnya.


* **Logistic Regression Modeling:** Membangun model algoritma Regresi Logistik (Keluarga Binomial) untuk memprediksi probabilitas mahasiswa mengikuti kegiatan ekstrakurikuler berdasarkan kombinasi prediktor Usia (*Age*) dan Status Pekerjaan Paruh Waktu (*PartTimeJob*) serta mengekstraksi koefisien distribusinya.



---

*Tertarik dengan proses analisis statistik tingkat lanjut dan kode pemrograman R di balik layar?*
Silakan telusuri tahapan lengkapnya melalui Jupyter Notebook di repositori ini. Jika Anda memiliki *feedback*, masukan, atau ingin berdiskusi mengenai peluang kolaborasi dan karir di bidang data, mari terhubung melalui [LinkedIn Saya](https://www.google.com/search?q=https://www.linkedin.com/in/deswita-nur-ardias-farsha-53a251284) atau jangkau saya melalui email di **deswitanaf.work@gmail.com**.
