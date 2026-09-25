---
name: rps-obe-generator
description: >-
  Panduan dan alur kerja otomatis untuk menyusun Rencana Pembelajaran Semester (RPS) berbasis Outcome-Based Education (OBE) standar kurikulum APTIKOM Versi 2.0 dan format resmi RPS UNIROW (Universitas PGRI Ronggolawe). Gunakan skill ini setiap kali dosen atau pengguna ingin menyusun, mengembangkan, merevisi, memvalidasi, atau mengekspor RPS perguruan tinggi, merumuskan CPL/CPMK/Sub-CPMK dengan Taksonomi Bloom, menyusun matriks pembelajaran 16 pertemuan (UTS minggu 8, UAS minggu 16), alokasi waktu SKS SN-Dikti, merancang tugas terstruktur, serta rubrik penilaian skala 1-5 hingga file .docx siap cetak.
---

# RPS-OBE Generator — Panduan Penyusunan RPS Berbasis OBE

Skill ini dirancang untuk mendampingi dosen dalam menyusun **Rencana Pembelajaran Semester (RPS)** yang berkualitas tinggi, taat asas kurikulum **Outcome-Based Education (OBE)**, memenuhi standar akreditasi nasional/internasional (**APTIKOM, LAM INFOKOM, IABEE/ASIIN**), dan disajikan dalam format resmi **Format RPS UNIROW (Universitas PGRI Ronggolawe)**.

Struktur metodologi skill ini diadopsi dari **Buku Saku Penyusunan RPS Berbasis OBE dengan Modul Prompt Engineering untuk Dosen**.

---

## Tiga Dokumen Landasan Utama

Skill ini beroperasi dengan mengintegrasikan 3 pilar dokumen:

```text
┌─────────────────────────────────┐   ┌─────────────────────────────────┐
│     Buku Saku RPS OBE           │   │    Buku Kurikulum APTIKOM 2.0   │
│ (Alur 6 Langkah Prompt Dosen)   │   │  (Standar CPL, BK, MK, Asesmen) │
└────────────────┬────────────────┘   └────────────────┬────────────────┘
                 │                                     │
                 └──────────────────┬──────────────────┘
                                    ▼
                 ┌─────────────────────────────────────┐
                 │       Format RPS UNIROW             │
                 │ (Template Resmi Tabel & Dokumen)    │
                 └──────────────────┬──────────────────┘
                                    ▼
                 ┌─────────────────────────────────────┐
                 │  Dokumen RPS OBE Lengkap (.docx/.md)│
                 └─────────────────────────────────────┘
```

1. **Buku Saku RPS OBE**: Menyediakan 6 tahapan prompt berurutan dari perumusan fondasi hingga laporan final.
2. **Buku Kurikulum Prodi S1 Informatika Versi 2.0 (APTIKOM)**: Menyediakan basis data 10 CPL standar, 22 Bahan Kajian (BK01–BK22), susunan mata kuliah (MK01–MK37), taksonomi Bloom, dan standar rubrik asesmen.
3. **Format RPS UNIROW**: Menyediakan template tabel resmi, kop institusi, otorisasi pengesahan, matriks korelasi CPL-SubCPMK, matriks mingguan 16 pertemuan, dan lembar validasi.

---

## Pilihan Alur Kerja (Mode Operasi)

Skill ini mendukung 3 cara kerja yang fleksibel:

### Mode 1: Interaktif Terpandu (Langkah 1 s.d. 6 Step-by-Step)
Cocok digunakan saat dosen ingin menyusun RPS secara dialogis tahap demi tahap, meninjau hasil rumusan di setiap langkah sebelum melangkah ke tahap berikutnya.

### Mode 2: Generasi Cepat Sekaligus (All-in-One Full Generation)
Cocok jika dosen memberikan informasi mata kuliah (nama, SKS, semester, fokus topik) dan menginginkan draf lengkap 16 minggu yang langsung terkompilasi utuh.

### Mode 3: Ekspor Dokumen Resmi (.docx)
Mengubah data RPS yang telah disepakati menjadi file Microsoft Word (`.docx`) siap cetak menggunakan template asli UNIROW via skrip python [generate_rps_docx.py](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/scripts/generate_rps_docx.py).

---

## Alur 6 Langkah Terpandu (Buku Saku RPS OBE)

Jika menjalankan proses penyusunan, ikuti 6 langkah ini secara tertib:

```text
[Langkah 1: CPL & CPMK] ──> [Langkah 2: Sub-CPMK & Bobot] ──> [Langkah 3: Integrasi Bahan Kajian]
                                                                        │
[Langkah 6: Laporan Final] <── [Langkah 5: Tugas & Rubrik 1-5] <── [Langkah 4: Matriks 16 Pertemuan]
```

---

### Langkah 1: Definisi CPL dan CPMK (Membangun Fondasi)

*Tujuan: Menentukan CPL yang relevan dari standar kurikulum dan menurunkannya menjadi CPMK yang terukur.*

1. **Instruksi Eksekusi**:
   - Telusuri CPL yang relevan dari [aptikom_curriculum_cs2024.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/aptikom_curriculum_cs2024.md) (pilih 2 sampai 4 CPL yang dibebankan pada mata kuliah).
   - Turunkan setiap CPL menjadi 1 atau lebih CPMK.
   - Terapkan Kata Kerja Operasional (KKO) Taksonomi Bloom level C2 s.d. C6 dari [bloom_taxonomy_kko.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/bloom_taxonomy_kko.md).
   - Pastikan setiap CPMK memiliki kontribusi persentase yang jelas terhadap CPL induknya hingga **total tepat 100%**.
2. **Template Prompt Buku Saku**:
   ```text
   Bertindaklah sebagai Pakar Kurikulum Perguruan Tinggi berbasis Outcome-Based Education (OBE). Gunakan rujukan kurikulum [Sebutkan Nama Panduan Kurikulum, misal: APTIKOM 2024] dalam panel sumber. Definisikan Capaian Pembelajaran Lulusan (CPL) yang relevan untuk mata kuliah [Masukkan Nama Mata Kuliah]. Selanjutnya, turunkan CPL tersebut menjadi Capaian Pembelajaran Mata Kuliah (CPMK) yang terukur. Gunakan Kata Kerja Operasional (KKO) Taksonomi Bloom dan pastikan setiap CPMK memberikan kontribusi persentase yang jelas terhadap CPL induknya hingga total 100%.
   ```

---

### Langkah 2: Penjabaran Sub-CPMK dan Bobot Penilaian

*Tujuan: Memecah CPMK menjadi tahapan belajar (Sub-CPMK) yang bertingkat dan menentukan bobot penilaian.*

1. **Instruksi Eksekusi**:
   - Pecah setiap CPMK menjadi Sub-CPMK bertahap (biasanya 6 sampai 9 Sub-CPMK untuk 1 semester).
   - Terapkan kaidah **ABCD**:
     * **Audience**: Mahasiswa
     * **Behavior**: Kemampuan terukur (KKO Bloom: C..., P..., A...)
     * **Condition/Subject Matter**: Bahan kajian, tools, atau studi kasus
     * **Degree**: Standar mutu atau tingkat ketercapaian
   - Susun **Tabel Korelasi CPL terhadap Sub-CPMK** (matriks keterlacakan).
   - Tetapkan bobot penilaian (%) untuk setiap Sub-CPMK berdasarkan tingkat kesulitan materi sehingga **total akumulasi tepat 100%**.
2. **Template Prompt Buku Saku**:
   ```text
   Berdasarkan CPMK yang telah didefinisikan, jabarkan menjadi Sub-CPMK untuk setiap tahapan pembelajaran. Pastikan setiap Sub-CPMK memenuhi unsur Kemampuan (Behavior), Bahan Kajian (Subject Matter), dan Konteks. Sertakan tabel Korelasi CPL terhadap Sub-CPMK dan tentukan bobot penilaian (%) untuk setiap tahapan tersebut berdasarkan tingkat kesulitan dan beban belajarnya.
   ```

---

### Langkah 3: Integrasi Materi dari Sumber Referensi

*Tujuan: Memastikan keakuratan isi pengajaran berbasis buku ajar dan literatur ilmiah bereputasi.*

1. **Instruksi Eksekusi**:
   - Identifikasi bab atau topik kunci dari buku teks rujukan utama yang mendukung setiap Sub-CPMK.
   - Susun **Bahan Kajian (Materi Pembelajaran)** secara sistematis: mulai dari konsep dasar/fundamental, konsep inti, implementasi teknis, hingga penerapan lanjut/studi kasus.
   - Cantumkan konsep spesifik, framework, algoritma, atau metodologi industri yang menjadi ciri khas mata kuliah.
   - Cantumkan minimal **1–2 Pustaka Utama** dan **2–4 Pustaka Pendukung** (jurnal, standar internasional IEEE/ISO, atau dokumentasi resmi).
2. **Template Prompt Buku Saku**:
   ```text
   Tinjau buku referensi dan materi yang telah saya unggah di NotebookLM ini. Identifikasi bab atau topik kunci yang mendukung setiap Sub-CPMK yang telah kita susun. Integrasikan materi tersebut ke dalam Bahan Kajian mata kuliah secara sistematis, mulai dari konsep dasar hingga penerapan tingkat lanjut. Sebutkan pula fungsi atau konsep spesifik yang menjadi ciri khas mata kuliah ini sesuai dengan isi buku tersebut.
   ```

---

### Langkah 4: Penyusunan Matriks Pembelajaran 16 Pertemuan

*Tujuan: Menyusun jadwal aktivitas satu semester lengkap dengan metode pembelajaran aktif (SCL) dan alokasi waktu SKS.*

1. **Instruksi Eksekusi**:
   - Gunakan format tabel 8 kolom sesuai Tabel 2 [unirow_rps_template_guide.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/unirow_rps_template_guide.md):
     1. `Mg Ke-` (1 s.d. 16)
     2. `Kemampuan akhir tiap tahapan belajar (Sub-CPMK)`
     3. `Penilaian: Indikator`
     4. `Penilaian: Teknik & Kriteria`
     5. `Bentuk & Metode SCL; Penugasan; [Estimasi Waktu] - Luring`
     6. `Bentuk Pembelajaran; [Estimasi Waktu] - Daring`
     7. `Materi Pembelajaran [Pustaka]`
     8. `Bobot Penilaian (%)`
   - **ATURAN MUTLAK**:
     * **Minggu ke-8 WAJIB UTS (Ujian Tengah Semester)**.
     * **Minggu ke-16 WAJIB UAS (Ujian Akhir Semester)**.
     * **Total bobot penilaian pertemuan 1 s.d. 16 wajib tepat 100%**.
   - **Alokasi Waktu SKS (SN-Dikti)**:
     * **2 SKS**: `[PB: 1x(2x50')], [PT: 1x(2x60')], [KM: 1x(2x60')]`
     * **3 SKS**: `[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]`
     * **4 SKS**: `[PB: 1x(4x50')], [PT: 1x(4x60')], [KM: 1x(4x60')]`
     * Keterangan: `PB` = Proses Belajar / Tatap Muka, `PT` = Penugasan Terstruktur, `KM` = Kegiatan Mandiri.
   - Variasikan metode SCL: *Case Method, Project-Based Learning (PjBL), Small Group Discussion, Discovery Learning, Collaborative Learning*.
2. **Template Prompt Buku Saku**:
   ```text
   Buatlah Matriks Pembelajaran 16 Pertemuan dengan format tabel sesuai Format RPS UNIROW. Tetapkan Minggu ke-8 sebagai UTS dan Minggu ke-16 sebagai UAS. Untuk setiap pertemuan, isi kolom: 1) Sub-CPMK, 2) Indikator Penilaian, 3) Bentuk & Teknik Penilaian, 4) Metode Pembelajaran SCL (seperti Project-Based Learning atau Case Method), dan 5) Materi Pembelajaran beserta rujukan pustakanya. Gunakan estimasi waktu sesuai bobot [Masukkan Jumlah SKS] SKS.
   ```

---

### Langkah 5: Perancangan Tugas dan Indikator Penilaian Detail

*Tujuan: Merancang instrumen tugas terstruktur yang objektif dan rubrik penilaian OBE berskala 1–5.*

1. **Instruksi Eksekusi**:
   - Rancang 2 sampai 4 Tugas Terstruktur yang tersebar strategis sepanjang semester (misal: Tugas 1 formasi kebutuhan, Tugas 2 perancangan/arsitektur, Tugas 3 implementasi/pengujian/proyek akhir).
   - Format komponen tugas:
     * Judul Tugas & Sub-CPMK yang disasar
     * Jenis: Individu / Kelompok
     * Uraian Tugas: Objek garapan, batasan, metodologi pengerjaan
     * Bentuk & Format Luaran (PDF, repositori GitHub, video presentasi)
     * Indikator Penilaian: Ketepatan teknis (40%), akurasi analisis (35%), kualitas dokumentasi/komunikasi (25%)
   - Sertakan **Rubrik Penilaian OBE Standar Skala 1–5** (rujuk [assessment_rubric_scale5.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/assessment_rubric_scale5.md)):
     * Skala 5: Sangat Kompeten (81 – 100)
     * Skala 4: Kompeten (61 – 80)
     * Skala 3: Cukup Kompeten (41 – 60)
     * Skala 2: Kurang Kompeten (21 – 40)
     * Skala 1: Tidak Kompeten (0 – 20)
2. **Template Prompt Buku Saku**:
   ```text
   Rancanglah [Sebutkan Jumlah, misal: 3] Tugas Terstruktur yang didistribusikan secara strategis sepanjang semester. Definisikan jenis tugasnya (individu/kelompok) dan deskripsi pengerjaannya. Buatkan Indikator Penilaian yang detail untuk setiap tugas, mencakup aspek ketepatan teknis, akurasi analisis, dan kualitas hasil akhir. Sertakan Rubrik Penilaian Skala 1-5 (Sangat Kompeten hingga Tidak Kompeten) yang merujuk pada standar penilaian OBE di sumber panduan.
   ```

---

### Langkah 6: Generasi Laporan Final (Format Standar RPS UNIROW)

*Tujuan: Menyatukan seluruh hasil pembahasan menjadi dokumen RPS resmi utuh.*

1. **Instruksi Eksekusi**:
   - Kompilasi seluruh bagian ke format standar RPS UNIROW:
     1. Kop: Universitas PGRI Ronggolawe, Fakultas Sains dan Teknologi, Prodi S1 Informatika, Kode Dokumen
     2. Identitas MK: Nama, Kode, Rumpun, SKS, Semester, Tgl Penyusunan
     3. Otorisasi Pengesahan: Dosen Pengembang, Koordinator RMK, Ka PRODI
     4. Capaian Pembelajaran: CPL-PRODI, CPMK, Sub-CPMK
     5. Tabel Korelasi CPL terhadap Sub-CPMK (dengan Bobot % dan Jumlah Minggu, total 100%)
     6. Deskripsi Singkat MK & Bahan Kajian
     7. Daftar Pustaka (Utama & Pendukung)
     8. Dosen Pengampu & Mata Kuliah Prasyarat
     9. Matriks 16 Pertemuan (Tabel 8 kolom, UTS Mg 8, UAS Mg 16, total bobot 100%)
     10. Lembar Rancangan Tugas Terstruktur
     11. Rubrik Penilaian OBE Skala 1–5
     12. Lembar Pengesahan Validasi (Kaprodi & UJM Program Studi)
2. **Template Prompt Buku Saku**:
   ```text
   Sajikan seluruh hasil pembahasan dari langkah 1 sampai 5 ke dalam satu laporan utuh menggunakan template 'Format RPS UNIROW'. Pastikan seluruh bagian mulai dari identitas mata kuliah, otorisasi pengesahan, pemetaan korelasi CPL, matriks mingguan, hingga rincian tugas dan daftar pustaka terisi secara presisi, sistematis, dan profesional sesuai standar akreditasi.
   ```

---

## Ekspor Dokumen Word (.docx) Otomatis

Untuk menghasilkan file `.docx` berstandar resmi UNIROW, jalankan skrip Python:

```bash
python3 "/run/media/andy/512/Uncategories/Skill RPS/.agents/skills/rps-obe-generator/scripts/generate_rps_docx.py" --input <file_rps.json> --output <output_rps.docx>
```

Atau uji coba menggunakan contoh RPS Rekayasa Perangkat Lunak:
```bash
python3 "/run/media/andy/512/Uncategories/Skill RPS/.agents/skills/rps-obe-generator/scripts/generate_rps_docx.py" --example
```

Skrip ini akan memelihara logo resmi UNIROW, format tata letak landscape tabel, serta seluruh struktur sel sesuai dokumen template asli.

---

## Aturan Kualitas & Validasi Wajib (Quality Checklist)

Sebelum menyerahkan RPS kepada pengguna/dosen, pastikan Anda memverifikasi:
- [x] **Keterlacakan CPL-CPMK-SubCPMK**: Setiap Sub-CPMK jelas induk CPMK dan CPL-nya.
- [x] **Taksonomi Bloom Terukur**: Menggunakan KKO operasional, tidak menggunakan kata terlarang ("mengetahui", "memahami" tanpa bukti unjuk kerja).
- [x] **Total Bobot Tepat 100%**: Jumlah bobot pada Tabel Korelasi Sub-CPMK dan Kolom 8 Matriks 16 Pertemuan harus tepat 100%.
- [x] **Minggu Ujian Tepat**: Minggu ke-8 = UTS, Minggu ke-16 = UAS.
- [x] **Format Waktu SN-Dikti**: Estimasi waktu perkuliahan memuat komponen `PB`, `PT`, dan `KM` sesuai beban SKS.
- [x] **Format Institusi**: Menggunakan identitas Universitas PGRI Ronggolawe (UNIROW), Fakultas Sains dan Teknologi, dan Program Studi S1 Informatika.

---

## Daftar File Referensi & Asset Pendukung

- [prompts_step_by_step.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/prompts_step_by_step.md) — 6 Langkah prompt asli Buku Saku RPS OBE.
- [aptikom_curriculum_cs2024.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/aptikom_curriculum_cs2024.md) — Standar kurikulum APTIKOM (CPL01-CPL10, BK01-BK22, MK01-MK37).
- [bloom_taxonomy_kko.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/bloom_taxonomy_kko.md) — Panduan Kata Kerja Operasional Taksonomi Bloom & formula ABCD.
- [unirow_rps_template_guide.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/unirow_rps_template_guide.md) — Struktur tabel, format kolom, dan rumus SKS dokumen UNIROW.
- [assessment_rubric_scale5.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/references/assessment_rubric_scale5.md) — Format tugas terstruktur dan rubrik OBE skala 1–5.
- [generate_rps_docx.py](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/scripts/generate_rps_docx.py) — Skrip generator file Word `.docx` siap cetak.
- [rps_contoh_rekayasa_perangkat_lunak.json](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/examples/rps_contoh_rekayasa_perangkat_lunak.json) — Contoh data JSON lengkap RPS 16 pertemuan.
- [rps_contoh_rekayasa_perangkat_lunak.md](file:///run/media/andy/512/Uncategories/Skill%20RPS/.agents/skills/rps-obe-generator/examples/rps_contoh_rekayasa_perangkat_lunak.md) — Contoh dokumen RPS lengkap format Markdown.
