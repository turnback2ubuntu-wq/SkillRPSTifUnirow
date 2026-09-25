# Panduan Perancangan Tugas Terstruktur & Rubrik Penilaian OBE Skala 1–5

Dokumen ini memuat standar penyusunan instrumen evaluasi pembelajaran berbasis *Outcome-Based Education* (OBE) mengacu pada standar kurikulum APTIKOM Versi 2.0 (Tabel H & Tabel I) dan Buku Saku RPS OBE.

---

## 1. Prinsip Evaluasi Hasil Belajar Berbasis OBE

Dalam paradigma OBE, evaluasi tidak semata-mata menguji hafalan (*content-based*), melainkan menilai bukti unjuk kinerja (*performance-based*) mahasiswa dalam mencapai Sub-CPMK dan CPMK.

Prinsip utama:
1. **Validitas (Construct Alignment)**: Teknik dan instrumen penilaian harus menguji kemampuan sesuai level KKO pada Sub-CPMK (misal: Sub-CPMK C4 dievaluasi dengan studi kasus analisis, bukan pilihan ganda C1).
2. **Keterlacakan (Traceability)**: Setiap butir soal, tugas, atau unjuk kerja harus dapat dilacak langsung ke Sub-CPMK dan CPMK yang dinilai.
3. **Objektivitas & Transparansi**: Menggunakan kriteria rubrik yang jelas dengan skala bertingkat (Skala 1–5), sehingga mahasiswa memahami ekspektasi kinerja sejak awal.

---

## 2. Struktur Format Rancangan Tugas Terstruktur

Setiap tugas terstruktur dirancang dengan komponen berikut:

```text
Nama Mata Kuliah       : [Nama MK]
Kode Mata Kuliah / SKS : [Kode MK] / [X] SKS
Tugas Ke-              : [1 / 2 / 3]
Bentuk Tugas           : [Individu / Kelompok (misal: 3-4 mahasiswa)]
Alokasi Waktu          : [X Minggu / Terstruktur]
Sub-CPMK yang Disasar  : [Sub-CPMK X]
Bobot Nilai Tugas      : [X]% dari Total Nilai Semester

1. Judul Tugas:
   [Judul spesifik dan aplikatif, contoh: "Analisis Kebutuhan & Perancangan Arsitektur Sistem E-Commerce"]

2. Tujuan Tugas:
   [Kemampuan operasional yang akan dicapai mahasiswa setelah menyelesaikan tugas]

3. Uraian Tugas:
   a. Objek Garapan: [Studi kasus, dataset, sistem, atau problem riil yang diselesaikan]
   b. Yang Harus Dikerjakan & Batasan: [Instruksi langkah demi langkah, batasan fungsional, dan batasan teknologi]
   c. Metode/Cara Pengerjaan: [Tahapan riset, diskusi kelompok, perancangan diagram, implementasi kode, pengujian]
   d. Acuan / Rujukan: [Buku teks utama, standar IEEE SRS/SDDs, dokumentasi API]

4. Bentuk & Format Luaran:
   a. Laporan Tertulis (PDF): Format terstruktur, memuat pendahuluan, analisis, diagram, hasil, kesimpulan.
   b. Repositori Source Code: Git repository (GitHub/GitLab) dengan commit history yang rapi dan README lengkap.
   c. Video Demo / Presentasi: Durasi 5-10 menit mempresentasikan arsitektur dan simulasi kerja sistem.

5. Kriteria & Indikator Penilaian:
   - Ketepatan Teknis & Fungsionalitas (Bobot 40%)
   - Akurasi Analisis & Perancangan (Bobot 35%)
   - Kualitas Dokumentasi & Komunikasi (Bobot 25%)
```

---

## 3. Rubrik Penilaian OBE Standar APTIKOM Skala 1–5

Rubrik analitik menggunakan 5 tingkatan mutu kompetensi:

| Skala Mutu | Kategori Ketercapaian | Rentang Skor | Deskripsi Kinerja Umum |
| :---: | :---: | :---: | :--- |
| **5** | **Sangat Kompeten** (*Exceptional*) | **81 – 100** | Mahasiswa menunjukkan penguasaan sangat mendalam, akurat tanpa kesalahan konseptual/teknis, solusi komprehensif, orisinal, serta didukung argumentasi yang sangat logis dan terstruktur. |
| **4** | **Kompeten** (*Good/Proficient*) | **61 – 80** | Mahasiswa mampu menerapkan konsep dan metode dengan tepat, solusi berfungsi baik dengan sedikit kekurangan minor, analisis relevan dan terorganisir dengan baik. |
| **3** | **Cukup Kompeten** (*Satisfactory/Adequate*) | **41 – 60** | Mahasiswa memahami konsep dasar dan mampu menyelesaikan tugas pada tingkat fungsional standar, namun terdapat beberapa kelemahan pada analisis mendalam atau efisiensi teknis. |
| **2** | **Kurang Kompeten** (*Developing/Poor*) | **21 – 40** | Mahasiswa menunjukkan pemahaman terbatas, banyak terjadi kesalahan teknis/konseptual yang signifikan, solusi belum berjalan atau argumentasi tidak logis. |
| **1** | **Tidak Kompeten** (*Unacceptable/Failed*) | **0 – 20** | Mahasiswa tidak menunjukkan bukti pencapaian kompetensi, hasil kerja tidak sesuai instruksi tugas, tidak mengumpulkan, atau terindikasi plagiarisme berat. |

---

## 4. Matriks Rubrik Analitik Spesifik Bidang Informatika

Berikut adalah kriteria penilaian multidimensi untuk tugas perancangan/proyek perangkat lunak:

### Dimensi 1: Ketepatan Teknis & Kualitas Implementasi (Bobot: 40%)
- **Skala 5 (Sangat Kompeten / 81-100)**: Kode program atau konfigurasi sistem berjalan 100% sempurna tanpa bug, menerapkan *clean code architecture*, penanganan eror (*exception handling*) tangguh, efisien, dan aman.
- **Skala 4 (Kompeten / 61-80)**: Sistem berjalan baik untuk kasus utama (*happy path*), eror handling dasar terpasang, struktur kode rapi dengan komentar yang memadai.
- **Skala 3 (Cukup Kompeten / 41-60)**: Fungsi utama sistem dapat berjalan, namun masih terdapat bug pada *edge cases*, redundansi kode, atau efisiensi rendah.
- **Skala 2 (Kurang Kompeten / 21-40)**: Sistem sering mengalami *crash* / fatal error, banyak fungsi tidak berjalan, struktur kode tidak terorganisir.
- **Skala 1 (Tidak Kompeten / 0-20)**: Kode program tidak dapat dikompilasi atau dijalankan sama sekali.

### Dimensi 2: Akurasi Analisis & Perancangan Arsitektur (Bobot: 35%)
- **Skala 5 (Sangat Kompeten / 81-100)**: Perancangan arsitektur, diagram UML / ERD sangat presisi, konsisten, mematuhi standar notasi baku, serta menyelesaikan persoalan komputasi kompleks secara optimal.
- **Skala 4 (Kompeten / 61-80)**: Analisis kebutuhan tepat, diagram perancangan memadai dan merepresentasikan solusi dengan benar meskipun ada ketidaktepatan minor pada relasi antar elemen.
- **Skala 3 (Cukup Kompeten / 41-60)**: Analisis mencakup kebutuhan dasar namun kurang mendalam, beberapa notasi perancangan tidak konsisten dengan implementasi.
- **Skala 2 (Kurang Kompeten / 21-40)**: Analisis salah sasaran, perancangan tidak menjawab kebutuhan masalah, diagram membingungkan.
- **Skala 1 (Tidak Kompeten / 0-20)**: Tidak ada analisis atau perancangan arsitektur yang disajikan.

### Dimensi 3: Kualitas Dokumentasi, Presentasi, & Kerja Tim (Bobot: 25%)
- **Skala 5 (Sangat Kompeten / 81-100)**: Laporan disusun dengan kaidah ilmiah yang sangat baik, tata bahasa baku, grafik/diagram jelas, presentasi lisan menarik dan meyakinkan, pembagian peran dalam tim terlihat sangat solid.
- **Skala 4 (Kompeten / 61-80)**: Laporan rapi dan lengkap sesuai template, presentasi runtut dan mampu menjawab pertanyaan penguji dengan baik, kolaborasi tim berjalan lancar.
- **Skala 3 (Cukup Kompeten / 41-60)**: Laporan memenuhi format minimal namun terdapat kesalahan tipografi atau tata letak, presentasi lisan terbata-bata atau kurang percaya diri.
- **Skala 2 (Kurang Kompeten / 21-40)**: Laporan tidak lengkap, banyak bagian penting yang kosong, presentasi tidak menguasai materi yang dibuat.
- **Skala 1 (Tidak Kompeten / 0-20)**: Tidak ada laporan atau presentasi yang diserahkan.
