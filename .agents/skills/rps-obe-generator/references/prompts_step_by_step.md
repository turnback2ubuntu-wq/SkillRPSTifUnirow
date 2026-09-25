# Panduan 6 Langkah Prompt Penyusunan RPS Berbasis OBE

Dokumen ini memuat kumpulan prompt resmi, alur berpikir, dan tips penerapan dari **Buku Saku Penyusunan RPS Berbasis OBE dengan Modul Prompt Engineering untuk Dosen (Format RPS UNIROW)**.

---

## Ikhtisar Alur 6 Langkah

```text
[Langkah 1: CPL & CPMK]
        │  (Menentukan kompetensi lulusan & CPMK dengan Taksonomi Bloom)
        ▼
[Langkah 2: Sub-CPMK & Bobot]
        │  (Memecah tahapan belajar, korelasi CPL-SubCPMK, bobot total 100%)
        ▼
[Langkah 3: Integrasi Bahan Kajian]
        │  (Memetakan bab buku ajar/referensi ke topik Sub-CPMK)
        ▼
[Langkah 4: Matriks 16 Pertemuan]
        │  (Menyusun jadwal mingguan: Mg 8 UTS, Mg 16 UAS, alokasi jam SKS, metode SCL)
        ▼
[Langkah 5: Perancangan Tugas & Rubrik]
        │  (Merancang tugas terstruktur & rubrik OBE skala 1-5)
        ▼
[Langkah 6: Kompilasi Laporan Final]
           (Menyajikan dokumen lengkap ke Format Standar RPS UNIROW)
```

---

## Langkah 1: Membangun Fondasi (Definisi CPL dan CPMK)

### Tujuan
Menentukan arah kompetensi lulusan berdasarkan standar kurikulum nasional/asosiasi (APTIKOM 2024 / Kurikulum S1 Informatika) dan menurunkan profil lulusan menjadi Capaian Pembelajaran Mata Kuliah (CPMK) yang terukur.

### Teks Prompt Asli
```text
Bertindaklah sebagai Pakar Kurikulum Perguruan Tinggi berbasis Outcome-Based Education (OBE). Gunakan rujukan kurikulum [Sebutkan Nama Panduan Kurikulum, misal: APTIKOM 2024] dalam panel sumber. Definisikan Capaian Pembelajaran Lulusan (CPL) yang relevan untuk mata kuliah [Masukkan Nama Mata Kuliah]. Selanjutnya, turunkan CPL tersebut menjadi Capaian Pembelajaran Mata Kuliah (CPMK) yang terukur. Gunakan Kata Kerja Operasional (KKO) Taksonomi Bloom dan pastikan setiap CPMK memberikan kontribusi persentase yang jelas terhadap CPL induknya hingga total 100%.
```

### Penjelasan Penerapan
1. Langkah ini merupakan fondasi seluruh RPS. Kesalahan perumusan CPL dan CPMK akan membuat matriks pembelajaran dan asesmen melenceng.
2. Gunakan CPL resmi dari panduan kurikulum program studi (misalnya CPL01–CPL10 dari APTIKOM).
3. Setiap CPL yang dibebankan pada mata kuliah harus diturunkan menjadi 1 atau lebih CPMK.
4. Total persentase kontribusi CPMK terhadap CPL induknya harus tepat 100% untuk kebutuhan akuntabilitas asesmen akreditasi (IABEE/LAM INFOKOM).

### Tips Praktis
- Ganti parameter `[Sebutkan Nama Panduan Kurikulum]` (misal: "Buku Kurikulum Prodi S1 Informatika Versi 2.0 APTIKOM") dan `[Masukkan Nama Mata Kuliah]` (misal: "Rekayasa Perangkat Lunak").
- Jika CPL terlalu luas, gunakan prompt tindak lanjut: *"Persempit CPL agar lebih spesifik pada konteks mata kuliah ini."*

---

## Langkah 2: Memecah Kompetensi Menjadi Tahapan Belajar (Penjabaran Sub-CPMK & Bobot Penilaian)

### Tujuan
Memecah kompetensi besar (CPMK) menjadi tahapan belajar yang lebih kecil, spesifik, bertahap, dan terukur (Sub-CPMK) serta menentukan alokasi bobot evaluasi.

### Teks Prompt Asli
```text
Berdasarkan CPMK yang telah didefinisikan, jabarkan menjadi Sub-CPMK untuk setiap tahapan pembelajaran. Pastikan setiap Sub-CPMK memenuhi unsur Kemampuan (Behavior), Bahan Kajian (Subject Matter), dan Konteks. Sertakan tabel Korelasi CPL terhadap Sub-CPMK dan tentukan bobot penilaian (%) untuk setiap tahapan tersebut berdasarkan tingkat kesulitan dan beban belajarnya.
```

### Penjelasan Penerapan
1. Sub-CPMK adalah anak tangga menuju CPMK. Setiap Sub-CPMK harus memenuhi unsur:
   - **Kemampuan (Behavior)**: KKO yang teramati (misal: merancang, menganalisis, mengimplementasikan).
   - **Bahan Kajian (Subject Matter)**: Topik/isi keilmuan yang dipelajari.
   - **Konteks & Batasan (Condition/Degree)**: Situasi, metode, lingkungan kerja, atau standar ketercapaian.
2. Tabel Korelasi CPL terhadap Sub-CPMK merupakan bukti keterlacakan (*traceability matrix*) yang wajib ada pada Format RPS UNIROW.
3. Bobot penilaian (%) dialokasikan proporsional sesuai tingkat kesulitan dan beban belajar, bukan dibagi rata begitu saja.

### Tips Praktis
- Jumlah Sub-CPMK ideal untuk 1 semester berkisar antara 6 sampai 10 Sub-CPMK.
- Jika Sub-CPMK terlalu banyak, gabungkan yang temanya berdekatan dengan instruksi: *"Gabungkan Sub-CPMK minggu ke-X dan ke-Y karena temanya saling berkaitan."*
- Pastikan total bobot penilaian akumulatif Sub-CPMK tepat **100%**.

---

## Langkah 3: Memastikan Keakuratan Isi Pengajaran (Integrasi Materi dari Sumber Referensi)

### Tujuan
Memastikan materi perkuliahan benar-benar bersumber dari buku teks rujukan dan literatur ilmiah yang valid, bukan sekadar rangkuman generik.

### Teks Prompt Asli
```text
Tinjau buku referensi dan materi yang telah saya unggah di NotebookLM ini. Identifikasi bab atau topik kunci yang mendukung setiap Sub-CPMK yang telah kita susun. Integrasikan materi tersebut ke dalam Bahan Kajian mata kuliah secara sistematis, mulai dari konsep dasar hingga penerapan tingkat lanjut. Sebutkan pula fungsi atau konsep spesifik yang menjadi ciri khas mata kuliah ini sesuai dengan isi buku tersebut.
```

### Penjelasan Penerapan
1. Langkah ini menyusun **Bahan Kajian** mata kuliah secara sistematis: dari pengantar/fundamental, konsep inti, implementasi teknis, hingga evaluasi/studi kasus lanjut.
2. Mengidentifikasi bab-bab buku teks rujukan (Pustaka Utama dan Pustaka Pendukung).
3. Menampilkan fitur/konsep khas (misal: pustaka/framework modern, metodologi standar industri seperti Agile/Scrum, arsitektur microservices, dsb.).

### Tips Praktis
- Tentukan minimal 1–2 Pustaka Utama (buku teks standar internasional atau nasional bereputasi edisi terbaru) dan 2–3 Pustaka Pendukung (jurnal, artikel ilmiah, atau dokumentasi resmi).
- Tuliskan kode sitasi singkat pada setiap rujukan (misal: `[Pressman20]`, `[Sommerville20]`).

---

## Langkah 4: Menyusun Jadwal Aktivitas Satu Semester (Matriks Pembelajaran 16 Pertemuan)

### Tujuan
Menyusun matriks aktivitas perkuliahan mingguan dari Minggu ke-1 hingga Minggu ke-16 yang lengkap dengan metode *Student-Centered Learning* (SCL) dan estimasi alokasi waktu.

### Teks Prompt Asli
```text
Buatlah Matriks Pembelajaran 16 Pertemuan dengan format tabel sesuai Format RPS UNIROW. Tetapkan Minggu ke-8 sebagai UTS dan Minggu ke-16 sebagai UAS. Untuk setiap pertemuan, isi kolom: 1) Sub-CPMK, 2) Indikator Penilaian, 3) Bentuk & Teknik Penilaian, 4) Metode Pembelajaran SCL (seperti Project-Based Learning atau Case Method), dan 5) Materi Pembelajaran beserta rujukan pustakanya. Gunakan estimasi waktu sesuai bobot [Masukkan Jumlah SKS] SKS.
```

### Penjelasan Penerapan
1. Format tabel matriks mingguan mengikuti Tabel 2 Format RPS UNIROW dengan 8 kolom:
   - Kolom 1: Minggu Ke- (1–16)
   - Kolom 2: Kemampuan akhir tiap tahapan belajar (Sub-CPMK)
   - Kolom 3: Penilaian - Indikator
   - Kolom 4: Penilaian - Kriteria & Bentuk/Teknik
   - Kolom 5: Bentuk Pembelajaran; Metode Pembelajaran; Penugasan Mahasiswa; [Estimasi Waktu] - **Luring**
   - Kolom 6: Bentuk Pembelajaran; Metode Pembelajaran; Penugasan Mahasiswa; [Estimasi Waktu] - **Daring**
   - Kolom 7: Materi Pembelajaran [Pustaka]
   - Kolom 8: Bobot Penilaian (%)
2. **Minggu ke-8 WAJIB dialokasikan untuk UTS** dan **Minggu ke-16 WAJIB dialokasikan untuk UAS**. Tidak boleh diisi materi baru biasa.
3. Estimasi waktu pembelajaran mengacu pada Permendikbudristek / SN-Dikti:
   - **Kuliah 1 SKS**:
     * Proses Belajar / Tatap Muka (PB) = 50 menit/minggu
     * Penugasan Terstruktur (PT) = 60 menit/minggu
     * Kegiatan Mandiri (KM) = 60 menit/minggu
   - **Kuliah 2 SKS**: `PB: 2x50' = 100'`, `PT: 2x60' = 120'`, `KM: 2x60' = 120'`
   - **Kuliah 3 SKS**: `PB: 3x50' = 150'`, `PT: 3x60' = 180'`, `KM: 3x60' = 180'`
   - **Kuliah 4 SKS**: `PB: 4x50' = 200'`, `PT: 4x60' = 240'`, `KM: 4x60' = 240'`
   - **Praktikum 1 SKS**: 170 menit praktikum per minggu.
4. Terapkan variasi metode SCL modern: Case Method (PBL berbasis studi kasus), Project-Based Learning (PjBL), Small Group Discussion, Discovery Learning, Collaborative Learning.

---

## Langkah 5: Menyusun Instrumen Evaluasi yang Objektif (Perancangan Tugas & Rubrik Skala 1–5)

### Tujuan
Menyusun instrumen evaluasi tugas terstruktur dan rubrik penilaian OBE berskala 1–5 yang transparan dan dapat diverifikasi asesor.

### Teks Prompt Asli
```text
Rancanglah [Sebutkan Jumlah, misal: 3] Tugas Terstruktur yang didistribusikan secara strategis sepanjang semester. Definisikan jenis tugasnya (individu/kelompok) dan deskripsi pengerjaannya. Buatkan Indikator Penilaian yang detail untuk setiap tugas, mencakup aspek ketepatan teknis, akurasi analisis, dan kualitas hasil akhir. Sertakan Rubrik Penilaian Skala 1-5 (Sangat Kompeten hingga Tidak Kompeten) yang merujuk pada standar penilaian OBE di sumber panduan.
```

### Penjelasan Penerapan
1. Distribusikan tugas terstruktur secara merata, misalnya:
   - **Tugas 1 (Formatif/Awal)**: Penguasaan konsep dasar dan analisis kebutuhan (Minggu ke-3 atau ke-4).
   - **Tugas 2 (Pengembangan/Tengah)**: Perancangan arsitektur / implementasi model (Minggu ke-6 atau ke-7 menjelang UTS).
   - **Tugas 3 (Proyek/Akhir)**: Proyek integrasi berbasis tim (PjBL) atau penyelesaian studi kasus komprehensif (Minggu ke-12 s.d. ke-15).
2. Format uraian tugas mencakup:
   - Judul Tugas
   - Sub-CPMK yang disasar
   - Jenis tugas: Individu / Kelompok
   - Objek Garapan & Batasan Masalah
   - Metodologi / Cara Pengerjaan
   - Bentuk & Format Luaran (Source code, dokumen laporan, video demo, slide presentasi)
3. Rubrik Penilaian Standar OBE Skala 1–5 (APTIKOM & UNIROW):
   - **Skala 5 (Sangat Kompeten, Skor 81–100)**: Analisis komprehensif, implementasi sempurna tanpa eror, struktur sistematis, inovatif.
   - **Skala 4 (Kompeten, Skor 61–80)**: Analisis tepat, implementasi berfungsi baik dengan sedikit catatan minor, dokumentasi rapi.
   - **Skala 3 (Cukup Kompeten, Skor 41–60)**: Konsep dasar terpenuhi, fungsi utama berjalan namun ada beberapa kekurangan teknis atau analisis terbatas.
   - **Skala 2 (Kurang Kompeten, Skor 21–40)**: Pemahaman terbatas, banyak kesalahan fungsional/teknis, dokumentasi kurang lengkap.
   - **Skala 1 (Tidak Kompeten, Skor 0–20)**: Tidak memenuhi kriteria penugasan, hasil tidak dapat diverifikasi, atau tidak mengumpulkan.

---

## Langkah 6: Generasi Laporan Final (Format Standar RPS UNIROW)

### Tujuan
Menyatukan dan mengompilasi seluruh hasil dari Langkah 1 sampai 5 ke dalam satu dokumen resmi yang utuh dan siap divalidasi serta ditandatangani.

### Teks Prompt Asli
```text
Sajikan seluruh hasil pembahasan dari langkah 1 sampai 5 ke dalam satu laporan utuh menggunakan template 'Format RPS UNIROW'. Pastikan seluruh bagian mulai dari identitas mata kuliah, otorisasi pengesahan, pemetaan korelasi CPL, matriks mingguan, hingga rincian tugas dan daftar pustaka terisi secara presisi, sistematis, dan profesional sesuai standar akreditasi.
```

### Penjelasan Penerapan & Checklist Validasi
Pastikan dokumen final memuat seluruh komponen wajib:
- [x] Kop Universitas PGRI Ronggolawe, Fakultas Sains dan Teknologi, Program Studi S1 Informatika, Kode Dokumen.
- [x] Rencana Pembelajaran Semester (RPS).
- [x] Identitas Mata Kuliah (Nama, Kode, Rumpun MK, Bobot SKS, Semester, Tanggal Penyusunan).
- [x] Lembar Otorisasi Pengesahan (Dosen Pengembang, Koordinator RMK, Ka PRODI).
- [x] Rumusan CPL-PRODI yang dibebankan pada MK.
- [x] Rumusan CPMK beserta persentase kontribusi terhadap CPL (Total 100%).
- [x] Rumusan Sub-CPMK dengan kode taksonomi Bloom `[C..., A..., P...]`.
- [x] Tabel Korelasi CPL terhadap Sub-CPMK (Beserta bobot % dan jumlah minggu, total 100%).
- [x] Deskripsi Singkat Mata Kuliah.
- [x] Bahan Kajian: Materi Pembelajaran yang tersusun hierarkis.
- [x] Daftar Pustaka (Utama dan Pendukung) format sitasi akademik.
- [x] Dosen Pengampu & Mata Kuliah Prasyarat.
- [x] Matriks Pembelajaran Mingguan 16 Pertemuan (Tabel 8 kolom, UTS di Minggu 8, UAS di Minggu 16, total bobot 100%).
- [x] Rencana Tugas Terstruktur & Rubrik Penilaian OBE Skala 1–5.
- [x] Lembar Pengesahan Validasi (Tanggal validasi, Ketua Program Studi, UJM Program Studi).
