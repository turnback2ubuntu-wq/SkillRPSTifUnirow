# RENCANA PEMBELAJARAN SEMESTER (RPS)
## PROGRAM STUDI S1 INFORMATIKA — FAKULTAS SAINS DAN TEKNOLOGI
### UNIVERSITAS PGRI RONGGOLAWE (UNIROW) TUBAN

**Kode Dokumen**: `RPS-INF-IF6802`  
**Tanggal Penyusunan**: `25 Agustus 2025`

---

## I. IDENTITAS MATA KULIAH

| Item | Keterangan |
| :--- | :--- |
| **Nama Mata Kuliah (MK)** | **Analisa Data Multivariat** |
| **Kode Mata Kuliah** | **IF6802** |
| **Rumpun Mata Kuliah (RMK)** | Kecerdasan Komputasional & Sains Data |
| **Bobot SKS** | **3 SKS** (Teori & Praktik Komputasi Terintegrasi) |
| **Semester** | 6 (Enam) / Peminatan Data Science |
| **Dosen Pengembang RPS** | **Andy Haryoko, S.T., M.T.** |
| **Koordinator RMK** | **Andy Haryoko, S.T., M.T.** |
| **Ketua Program Studi** | **AMALUDIN ARIFIA, M.Kom.** |
| **Dosen Pengampu** | **Andy Haryoko, S.T., M.T.** |
| **Mata Kuliah Prasyarat** | IF640424 Statistik Teknik / Aljabar Linier & Matriks |

---

## II. CAPAIAN PEMBELAJARAN

### A. Capaian Pembelajaran Lulusan (CPL-PRODI) yang Dibebankan pada MK
1. **CPL03**: Memiliki kemampuan memahami cara kerja sistem komputer serta menerapkan berbagai algoritma/metode untuk memecahkan masalah dalam suatu organisasi. `[C2, C3]`
2. **CPL04**: Memiliki kompetensi dalam menganalisis persoalan *computing* yang kompleks untuk mengidentifikasi solusi pengelolaan proyek teknologi di bidang informatika/ilmu komputer dengan mempertimbangkan perkembangan ilmu transdisiplin. `[C4]`
3. **CPL05**: Memiliki kemampuan merancang, mengimplementasikan, dan mengevaluasi solusi berbasis *computing* (sistem cerdas, data analytics, machine learning) yang memenuhi kebutuhan pengguna dengan pendekatan analitis dan saintifik. `[C5, C6]`

### B. Capaian Pembelajaran Mata Kuliah (CPMK) & Persentase Kontribusi
1. **CPMK1 (Kontribusi 100% terhadap CPL03)**:  
   *Mampu menerapkan konsep dasar aljabar linier multivariat, vektor rata-rata, matriks varians-kovarians/korelasi, serta pengujian asumsi normalitas multivariat dan deteksi outlier (Mahalanobis distance) dalam eksplorasi data berdimensi tinggi [C3].*
2. **CPMK2 (Kontribusi 50% terhadap CPL04)**:  
   *Mampu menganalisis dan mereduksi dimensi data menggunakan teknik Principal Component Analysis (PCA) dan Exploratory/Confirmatory Factor Analysis (EFA/CFA) untuk ekstraksi fitur data kompleks [C4].*
3. **CPMK3 (Kontribusi 50% terhadap CPL04)**:  
   *Mampu menganalisis hubungan ketergantungan dan perbedaan grup multivariat melalui Regresi Linier Berganda, Regresi Logistik Multivariat, dan MANOVA (Multivariate Analysis of Variance) [C4].*
4. **CPMK4 (Kontribusi 100% terhadap CPL05)**:  
   *Mampu merancang, mengimplementasikan, dan mengevaluasi model klasifikasi dan segmentasi data menggunakan Analisis Diskriminan, Cluster Analysis (Hierarkis & K-Means), Multidimensional Scaling (MDS), serta visualisasi interaktif dengan Python/R untuk studi kasus industri/sains [C5, C6].*

### C. Pemetaan Korelasi CPL, CPMK, Sub-CPMK, Bobot & Alokasi Waktu

| Sub-CPMK | CPL03 | CPL04 | CPL05 | CPMK Induk | Bobot Penilaian (%) | Alokasi Waktu |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Sub-CPMK 1**: Konsep multivariat, matriks data, mean vektor, kovarians `[C2]` | **V** | | | CPMK1 | 3% | Minggu 1 (150' PB, 180' PT+BM) |
| **Sub-CPMK 2**: Uji normalitas multivariat & jarak Mahalanobis outlier `[C3]` | **V** | | | CPMK1 | 4% | Minggu 2 (150' PB, 180' PT+BM) |
| **Sub-CPMK 3**: Principal Component Analysis (PCA), eigen, scree, biplot `[C4]` | | **V** | | CPMK2 | 7% | Minggu 3 (150' PB, 180' PT+BM) |
| **Sub-CPMK 4**: Exploratory Factor Analysis (EFA), rotasi Varimax/Promax `[C4]` | | **V** | | CPMK2 | 6% | Minggu 4 (150' PB, 180' PT+BM) |
| **Sub-CPMK 5**: Regresi Linier Berganda multivariat & diagnosa asumsi VIF `[C4]` | | **V** | | CPMK3 | 5% | Minggu 5 (150' PB, 180' PT+BM) |
| **Sub-CPMK 6**: Regresi Logistik Biner & Multinomial multivariat `[C4]` | | **V** | | CPMK3 | 5% | Minggu 6 (150' PB, 180' PT+BM) |
| **Sub-CPMK 7**: MANOVA, Wilks' Lambda, Hotelling's T², Box's M `[C4, C5]` | | **V** | | CPMK3 | 5% | Minggu 7 (150' PB, 180' PT+BM) |
| **UTS (Evaluasi Tengah Semester)**: Ujian Teori & Kasus Komputasi | **V** | **V** | | CPMK1,2,3 | 15% | Minggu 8 (150 Menit) |
| **Sub-CPMK 8**: Linear & Quadratic Discriminant Analysis (LDA/QDA) `[C5]` | | | **V** | CPMK4 | 5% | Minggu 9 (150' PB, 180' PT+BM) |
| **Sub-CPMK 9**: Hierarchical Agglomerative Clustering & K-Means (Silhouette) `[C5, C6]` | | | **V** | CPMK4 | 10% | Minggu 10–11 (300' PB, 360' PT+BM) |
| **Sub-CPMK 10**: Multidimensional Scaling (MDS) & Correspondence Analysis `[C5]` | | | **V** | CPMK4 | 8% | Minggu 12–13 (300' PB, 360' PT+BM) |
| **Sub-CPMK 11**: Integrasi Pipeline & Presentasi Ilmiah Capstone Data `[C5, C6]` | | | **V** | CPMK4 | 12% | Minggu 14–15 (300' PB, 360' PT+BM) |
| **UAS (Evaluasi Akhir Semester)**: Final Capstone Report & Code Review | | | **V** | CPMK3,4 | 15% | Minggu 16 (150 Menit) |
| **TOTAL** | | | | | **100%** | **16 Minggu (48 Jam PB, 57.6 Jam PT+BM)** |

---

## III. DESKRIPSI SINGKAT MATA KULIAH

Mata kuliah **Analisa Data Multivariat (IF6802)** merupakan mata kuliah keahlian peminatan Sains Data dan Kecerdasan Komputasional yang membekali mahasiswa S1 Informatika dengan landasan teori dan keterampilan komputasi dalam menganalisis kumpulan data kompleks berdimensi tinggi (*multi-variable*). Mahasiswa diajarkan untuk memahami dan menerapkan teknik reduksi dimensi (*Principal Component Analysis* dan *Factor Analysis*), pemodelan dependensi multivariat (*Multiple Regression*, *Logistic Regression*, dan *MANOVA*), serta metode klasifikasi dan segmentasi (*Discriminant Analysis*, *Cluster Analysis*, *Multidimensional Scaling*, dan *Correspondence Analysis*). Perkuliahan mengintegrasikan pendekatan analitis berbasis matriks dengan pemrograman praktis menggunakan Python (*NumPy, SciPy, Pandas, Scikit-learn, Statsmodels*) dan R, serta diakhiri dengan pengerjaan Proyek Analitik Data Multivariat Skala Industri.

---

## IV. BAHAN KAJIAN & SUMBER PUSTAKA

### A. Bahan Kajian (Materi Pembelajaran)
1. Pengantar Analisa Multivariat, Vektor Mean, Matriks Kovarians & Korelasi
2. Uji Asumsi Normalitas Multivariat & Deteksi Outlier (Mahalanobis Distance)
3. Principal Component Analysis (PCA): Ekstraksi Eigen, Scree Plot, & Biplot
4. Exploratory Factor Analysis (EFA): Ekstraksi Faktor, Rotasi (Varimax/Promax), & Skor Faktor
5. Regresi Linier Berganda Multivariat & Diagnosa Asumsi Klasik
6. Regresi Logistik Multivariat (Binary & Multinomial Logistic Regression)
7. Uji Vektor Rata-rata Hotelling's T² & MANOVA (One-way dan Two-way)
8. Linear & Quadratic Discriminant Analysis (LDA & QDA)
9. Analisis Klaster Hierarkis (Agglomerative) & Klaster Non-Hierarkis (K-Means Clustering)
10. Evaluasi Validitas Klaster (Elbow Method, Silhouette Analysis, Davies-Bouldin)
11. Multidimensional Scaling (MDS) Metrik & Non-Metrik
12. Simple & Multiple Correspondence Analysis (CA & MCA)
13. Proyek Analitik Sains Data Multivariat Berbasis Industri Menggunakan Python/R

### B. Daftar Referensi
**Pustaka Utama**:
1. Johnson, R. A., & Wichern, D. W. (2019). *Applied Multivariate Statistical Analysis* (6th ed.). Pearson Education.
2. Hair, J. F., Black, W. C., Babin, B. J., & Anderson, R. E. (2019). *Multivariate Data Analysis* (8th ed.). Cengage Learning.
3. Everitt, B., & Hothorn, T. (2011). *An Introduction to Applied Multivariate Analysis with R*. Springer Science & Business Media.

**Pustaka Pendukung**:
1. James, G., Witten, D., Hastie, T., & Tibshirani, R. (2021). *An Introduction to Statistical Learning with Applications in R/Python* (2nd ed.). Springer.
2. Rencher, A. C., & Christensen, W. F. (2012). *Methods of Multivariate Analysis* (3rd ed.). John Wiley & Sons.
3. VanderPlas, J. (2016). *Python Data Science Handbook: Essential Tools for Working with Data*. O'Reilly Media.
4. Artikel Jurnal Ilmiah IEEE TPAMI & ACM TKDD terkini.

---

## V. MATRIKS RENCANA PEMBELAJARAN 16 PERTEMUAN

| Mg | Sub-CPMK | Indikator Penilaian | Kriteria & Teknik | Bentuk & Metode Pembelajaran (Luring / Daring) | Materi Pembelajaran [Pustaka] | Bobot (%) |
| :---: | :--- | :--- | :--- | :--- | :--- | :---: |
| **1** | Sub-CPMK 1: Konsep dasar analisa multivariat, matriks data, vektor mean, matriks kovarians `[C2]` | Ketepatan menjelaskan taksonomi dependensi vs interdependensi, representasi matriks data | Kriteria: Ketepatan matematis; Teknik: Kuis eksplorasi | **Luring**: Kuliah interaktif, Diskusi, Praktik Matriks Python/R (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Modul LMS, Video tutorial | Pengenalan Multivariat, Vektor Mean, Matriks Kovarians & Korelasi [Johnson Bab 1-2, Hair Bab 1] | 3% |
| **2** | Sub-CPMK 2: Uji normalitas multivariat & deteksi outlier Mahalanobis `[C3]` | Keakuratan Mardia's test, Q-Q plot, diagnosa outlier berjarak Mahalanobis | Kriteria: Kebenaran diagnosa; Teknik: Tugas Lab 1 | **Luring**: Kuliah, Praktikum Uji Normalitas & Mahalanobis di Lab Komputer (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Akses dataset & upload script di LMS | Distribusi Normal Multivariat, Elips Kontur, Mahalanobis Distance [Johnson Bab 4-5] | 4% |
| **3** | Sub-CPMK 3: Principal Component Analysis (PCA), nilai/vektor eigen, scree plot, biplot `[C4]` | Kemampuan dekomposisi nilai eigen, memilih jumlah komponen optimal, interpretasi biplot | Kriteria: Ketajaman analisis reduksi; Teknik: Portofolio PCA | **Luring**: Problem-Based Learning: Reduksi Dimensi Fitur Citra/Sensor di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Visualisasi interaktif 3D di Colab | PCA, Dekomposisi Spektral, Nilai & Vektor Eigen, Biplot [Johnson Bab 8, Hair Bab 3] | 7% |
| **4** | Sub-CPMK 4: Exploratory Factor Analysis (EFA), rotasi Varimax/Promax, loading faktor `[C4]` | Uji kelayakan KMO & Bartlett, ekstraksi faktor, rotasi ortogonal/oblik, penamaan faktor | Kriteria: Logika interpretasi konstruk laten; Teknik: Tugas EFA Survei | **Luring**: Diskusi Studi Kasus Survei TI, Praktik EFA R/Python (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Forum diskusi perbedaan PCA vs EFA di LMS | Exploratory Factor Analysis, KMO Test, Rotasi Varimax/Promax, Factor Scores [Hair Bab 3] | 6% |
| **5** | Sub-CPMK 5: Regresi Linier Berganda multivariat & diagnosa asumsi VIF `[C4]` | Estimasi parameter OLS matriks, uji simultan/parsial, diagnosa multikolinieritas & residual | Kriteria: Kelengkapan diagnosa asumsi; Teknik: Tugas Terstruktur | **Luring**: Ceramah Pemodelan Multivariat, Simulasi Matriks Regresi (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Submit laporan regresi di LMS | Multiple Regression Notasi Matriks, R², VIF, Diagnosa Residual [Johnson Bab 7, Hair Bab 4] | 5% |
| **6** | Sub-CPMK 6: Regresi Logistik Biner & Multinomial multivariat `[C4]` | Estimasi MLE, Odds Ratio, Hosmer-Lemeshow test, matriks konfusi klasifikasi | Kriteria: Ketepatan rasio odds & akurasi; Teknik: Praktikum Lab | **Luring**: Praktikum Kasus Deteksi Churn Nasabah di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Asistensi coding di LMS | Regresi Logistik Biner & Multinomial, Logit, Confusion Matrix [Hair Bab 5, James Bab 4] | 5% |
| **7** | Sub-CPMK 7: MANOVA, Wilks' Lambda, Hotelling's T², Box's M `[C4, C5]` | Perumusan hipotesis vektor mean, Box's M homogenitas kovarians, 4 statistik uji MANOVA | Kriteria: Kedalaman analisis varians; Teknik: Presentasi A/B Testing | **Luring**: Kuliah Diskusi, Praktik MANOVA Komputasi di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Review persiapan UTS di LMS | Uji Vektor Mean Multivariat, Hotelling's T², One-Way MANOVA, Box's M [Johnson Bab 6, Hair Bab 6] | 5% |
| **8** | **UTS**: Evaluasi Tengah Semester (CPMK1, CPMK2, CPMK3) | Ketepatan analisis matematis dan pengolahan data multivariat (Mg 1-7) | Kriteria: Rubrik Ujian Tertulis & Lab (Skala 1-100); Teknik: Tes Tulis & Lab | **Ujian Terjadwal Luring di Lab Komputer (150 Menit)**<br>**Daring**: Upload lembar jawaban & script di LMS | Seluruh Materi Pembelajaran Minggu 1 s.d. Minggu 7 | **15%** |
| **9** | Sub-CPMK 8: Linear & Quadratic Discriminant Analysis (LDA/QDA) `[C5]` | Perhitungan fungsi diskriminan Fisher, evaluasi Wilk's Lambda, perbandingan LDA vs QDA | Kriteria: Akurasi pemodelan klasifikasi; Teknik: Tugas Proyek Mandiri 1 | **Luring**: Case-Based Learning: Analisis Risiko Kredit di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Tutorial boundary decision di LMS | Discriminant Analysis, Fisher's LDA, QDA, Bayesian Decision Rule [Johnson Bab 11, Hair Bab 5] | 5% |
| **10** | Sub-CPMK 9: Hierarchical Agglomerative Clustering & Dendrogram `[C5]` | Matriks jarak, linkage method (Ward, Single, Complete), pemotongan dendrogram | Kriteria: Validitas klaster dendrogram; Teknik: Lembar Kerja Praktikum | **Luring**: Kuliah, Praktikum Klastering Segmentasi Pelanggan (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Diskusi metrik jarak di LMS | Cluster Analysis, Proximity Matrix, Linkage Methods, Dendrogram [Johnson Bab 12, Hair Bab 7] | 5% |
| **11** | Sub-CPMK 9: K-Means Clustering & Evaluasi Silhouette `[C5, C6]` | Algoritma Lloyd, penentuan k optimal (Elbow & Silhouette), profiling klaster | Kriteria: Ketajaman profiling klaster; Teknik: Portofolio Unsupervised | **Luring**: Kuliah Interaktif, Praktikum K-Means & Validasi Silhouette (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Visualisasi 3D Klaster Plotly di LMS | Non-Hierarchical Clustering, K-Means, Silhouette Coefficient [Hair Bab 7, James Bab 10] | 5% |
| **12** | Sub-CPMK 10: Multidimensional Scaling (MDS) Metrik & Non-Metrik `[C5]` | Rekonstruksi ruang geometri dari matriks dissimilaritas, evaluasi Stress | Kriteria: Kebenaran perceptual map; Teknik: Tugas Brand Positioning | **Luring**: Demonstrasi Perhitungan MDS Metrik/Non-Metrik (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Studi kasus perceptual map di LMS | Multidimensional Scaling, STRESS Value, Perceptual Map [Johnson Bab 12, Hair Bab 8] | 4% |
| **13** | Sub-CPMK 10: Correspondence Analysis (CA & MCA) data kategori `[C5]` | Tabel kontingensi, profil baris/kolom, dekomposisi SVD matriks inersia | Kriteria: Ketepatan asosiasi kategori; Teknik: Tugas Analisis Fitur Software | **Luring**: Praktikum CA & Multiple CA (MCA) di R/Python (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Kuis inersia total di LMS | Correspondence Analysis, MCA, SVD, Contingency Matrix [Hair Bab 8, Everitt Bab 5] | 4% |
| **14** | Sub-CPMK 11: Integrasi Pipeline Analisis Multivariat Riil `[C5, C6]` | Integrasi preprocessing, reduksi dimensi, pemodelan dependensi & klastering | Kriteria: Kematangan pipeline & efisiensi kode; Teknik: Review Progres | **Luring**: Project-Based Learning Workshop & Asistensi Kode (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Upload draf repo GitHub di LMS | Pipeline End-to-End Sains Data Multivariat [Pustaka Utama 1 & 2] | 5% |
| **15** | Sub-CPMK 11: Presentasi Ilmiah & Diseminasi Temuan Multivariat `[C5, C6]` | Komunikasi saintifik, visualisasi interaktif data berdimensi tinggi, respon tanya jawab | Kriteria: Rubrik Presentasi 5 Skala; Teknik: Penilaian Seminar Proyek | **Luring**: Seminar Presentasi Proyek Akhir & Sesi Tanya Jawab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Peer-review feedback di LMS | Diseminasi Ilmiah Data Science & Storytelling with Data | 7% |
| **16** | **UAS**: Evaluasi Akhir Semester Berbasis Capstone Proyek Analitik | Naskah laporan ilmiah, repositori GitHub, kebaruan dataset, reliabilitas model | Kriteria: Rubrik Holistik Laporan & Kode (Skala 1-100); Teknik: Asesmen Deliverables | **Evaluasi Akhir & Pengumpulan Berkas Laporan Terjadwal**<br>**Daring**: Final submission bundle di LMS UNIROW | Seluruh Bahan Kajian Analisa Data Multivariat (Minggu 1 s.d. 15) | **15%** |
| **TOTAL** | | | | | | **100%** |

---

## VI. RANCANGAN TUGAS MAHASISWA & RUBRIK PENILAIAN OBE

### A. Rincian Tugas Terstruktur
1. **Tugas 1 (Minggu 2)**: Eksplorasi Matriks Data & Pengujian Asumsi Normalitas Multivariat (Mardia's test, Q-Q plot, deteksi outlier Mahalanobis pada dataset kontinu riil).
2. **Tugas 2 (Minggu 4)**: Studi Komparasi Reduksi Dimensi: PCA vs Exploratory Factor Analysis (Perbandingan dekomposisi eigen PCA vs rotasi Varimax EFA dalam menemukan konstruk laten).
3. **Tugas 3 (Minggu 6)**: Pemodelan Dependensi: Regresi Logistik Multivariat & Eksperimen MANOVA (Uji efek perlakuan interface pengguna multivariat).
4. **Tugas 4 (Minggu 10–15)**: Capstone Project: Klasifikasi & Segmentasi Data Skala Industri (Pipeline gabungan PCA + K-Means + Analisis Diskriminan / MDS pada dataset industri riil, dipresentasikan dan diunggah ke GitHub).

### B. Rubrik Penilaian OBE Skala 1–5

| Aspek Penilaian | Sangat Kurang (1) | Kurang (2) | Cukup (3) | Baik (4) | Sangat Baik (5) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Penguasaan Teori Aljabar Multivariat (C2-C3)** | Gagal memahami konsep matriks, salah perhitungan mean vektor & kovarians (`< 50`) | Rumus dihafal namun salah dalam perhitungan manual/script (`50-59`) | Perhitungan matriks benar dengan sedikit koreksi (`60-69`) | Menguasai operasi matriks, normalitas, dan jarak Mahalanobis (`70-84`) | Sempurna dalam teori matriks & penalaran matematis multivariat (`85-100`) |
| **Keterampilan Reduksi Dimensi (C4)** | Tidak memahami nilai eigen dan tujuan reduksi varians (`< 50`) | Menjalankan PCA/EFA tanpa kriteria penentuan komponen yang valid (`50-59`) | Menggunakan kriteria Kaiser dengan cukup baik (`60-69`) | Reduksi dimensi akurat, rotasi faktor tepat, biplot terinterpretasi (`70-84`) | Analisis reduksi dimensi sangat tajam, penamaan faktor laten inovatif (`85-100`) |
| **Pemodelan Dependensi & Uji Hipotesis (C4-C5)** | Salah memilih metode uji, mengabaikan asumsi statistik (`< 50`) | Menerapkan uji statistik namun diagnosa asumsi diabaikan (`50-59`) | Diagnosa asumsi standar terpenuhi (`60-69`) | Estimasi parameter tepat, uji asumsi lengkap, interpretasi akurat (`70-84`) | Evaluasi goodness of fit mendalam, interpretasi bisnis/sains luar biasa (`85-100`) |
| **Solusi Klasifikasi & Klastering (C5-C6)** | Algoritma segmentasi gagal atau menghasilkan output tidak valid (`< 50`) | Model klaster berjalan tanpa validasi koefisien Silhouette (`50-59`) | Segmentasi terbentuk, metrik validasi dihitung standar (`60-69`) | Model klaster & diskriminan optimal, perbandingan linkage mendalam (`70-84`) | Solusi klasifikasi/klastering canggih, profil klaster berdampak nyata, kode modular (`85-100`) |
| **Kualitas Laporan Ilmiah & Presentasi** | Format rusak, indikasi plagiarisme, kode tidak bisa dijalankan (`< 50`) | Laporan kurang rapi, dokumentasi kode minim (`50-59`) | Format ilmiah standar, kode berjalan normal (`60-69`) | Format rapi standar IEEE, dokumentasi kode di GitHub sangat baik (`70-84`) | Kualitas publikasi prosiding/jurnal, visualisasi interaktif memukau (`85-100`) |

---

## VII. LEMBAR PENGESAHAN RPS

| Dosen Pengembang RPS | Koordinator Rumpun Mata Kuliah (RMK) | Ketua Program Studi S1 Informatika |
| :---: | :---: | :---: |
| <br><br>**Andy Haryoko, S.T., M.T.**<br>NIDN: 07xxxxxxxx | <br><br>**Andy Haryoko, S.T., M.T.**<br>NIDN: 07xxxxxxxx | <br><br>**AMALUDIN ARIFIA, M.Kom.**<br>NIDN: 07xxxxxxxx |
