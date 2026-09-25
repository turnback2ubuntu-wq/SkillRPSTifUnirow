# Panduan Struktur & Format Standar RPS UNIROW (Universitas PGRI Ronggolawe)

Dokumen ini memuat panduan lengkap tata letak, struktur tabel, konvensi penomoran, aturan perhitungan alokasi waktu SKS, dan validasi dokumen sesuai dengan template resmi **Format RPS UNIROW.docx**.

---

## 1. Tata Letak Halaman (Page Layout)
- **Orientasi Bagian 1, 2, 3**: **Landscape** (A4: 297 mm x 210 mm) untuk memuat tabel lebar (khususnya Matriks Mingguan 8 kolom).
  - Margin: Atas ~0.76 in, Bawah ~0.2 in, Kiri ~0.71 in, Kanan ~0.89 in.
- **Orientasi Bagian 4 (Lembar Validasi & Catatan)**: **Portrait** (A4: 210 mm x 297 mm).
  - Margin: Atas ~1.10 in, Bawah ~0.57 in, Kiri ~0.71 in, Kanan ~0.71 in.

---

## 2. Anatomi Tabel Dokumen RPS UNIROW

### TABEL 0: Kop, Identitas Mata Kuliah, Otorisasi, dan Capaian Pembelajaran
Tabel pembuka dengan 6 kolom utama:

1. **Header Kop (Baris 0)**:
   - Kolom 0: Tempat Logo Resmi Perguruan Tinggi (Logo UNIROW).
   - Kolom 1-4 (Merged): `UNIVERSITAS PGRI RONGGOLAWE` / `FAKULTAS SAINS DAN TEKNOLOGI` / `PROGRAM STUDI S1 INFORMATIKA`.
   - Kolom 5: `Kode Dokumen: RPS-INF-XXX`.
2. **Judul Dokumen (Baris 1)**:
   - Merged 6 kolom: `RENCANA PEMBELAJARAN SEMESTER (RPS)`.
3. **Baris Identitas MK (Baris 2 & 3)**:
   - Baris 2 (Header): `MATA KULIAH (MK)` | `KODE` | `Rumpun MK` | `BOBOT (sks)` | `SEMESTER` | `Tgl Penyusunan`
   - Baris 3 (Isi): [Nama MK] | [Kode MK] | [Rumpun MK, misal: Software Engineering / AI] | [X sks] | [Semester] | [dd-mm-yyyy]
4. **Baris Otorisasi / Pengesahan (Baris 4 & 5)**:
   - Baris 4 (Jabatan): `OTORISASI / PENGESAHAN` | `Dosen Pengembang RPS` | `Koordinator RMK` | `Ka PRODI`
   - Baris 5 (Tanda Tangan & Nama): Tanda tangan, nama lengkap dengan gelar, dan NIDN/NUPTK.
5. **Baris Capaian Pembelajaran (Baris 6 s.d. 14)**:
   - `Capaian Pembelajaran`:
     * **CPL-PRODI yang dibebankan pada MK**: Daftar kode CPL (misal: CPL03, CPL04, CPL08) beserta deskripsi lengkapnya.
     * **Capaian Pembelajaran Mata Kuliah (CPMK)**: Penurunan dari CPL yang spesifik pada MK, dilengkapi persentase kontribusi terhadap CPL (misal: CPMK 1 berkontribusi 40% pada CPL03, CPMK 2 berkontribusi 60% pada CPL03).
     * **Kemampuan akhir tiap tahapan belajar MK (Sub-CPMK)**: Penjabaran CPMK ke Sub-CPMK bertingkat disertai kode Taksonomi Bloom (contoh: `[C3, P2, A2]`).

---

### TABEL 1: Korelasi CPL-SubCPMK, Deskripsi, Bahan Kajian, Pustaka, Dosen & Prasyarat

1. **Korelasi CPL terhadap Sub-CPMK (Baris 0 & 1)**:
   - Memuat matriks *traceability* (tabel bersarang / *nested table*):
     * Kolom Header: `Sub-CPMK` | `CPL... (%)` | `CPL... (%)` | `Bobot Penilaian (%)` | `Jumlah Minggu`
     * Setiap baris Sub-CPMK menunjukkan kontribusi terhadap CPL yang sesuai.
     * Baris Total: Jumlah Bobot Penilaian wajib tepat **100%**, dan total jumlah minggu terdistribusi dalam **14 minggu aktif materi + 2 minggu ujian (UTS & UAS) = 16 minggu**.
2. **Deskripsi Singkat MK (Baris 2)**:
   - Ringkasan komprehensif tentang ruang lingkup mata kuliah, urgensi kompetensi, alur materi dari awal hingga akhir, dan proyek/luaran utama.
3. **Bahan Kajian: Materi Pembelajaran (Baris 3)**:
   - Daftar pokok dan sub-pokok bahasan yang terstruktur secara logis dan runtut.
4. **Pustaka (Baris 4 s.d. 7)**:
   - **Utama**: Buku ajar / textbook inti edisi terbaru (cantumkan Penulis, Tahun, Judul, Penerbit, Kode Sitasi).
   - **Pendukung**: Jurnal ilmiah, proceeding, handbook industri, modul lab, atau dokumentasi resmi perangkat lunak/API.
5. **Dosen Pengampu (Baris 8)**:
   - Nama dosen pengampu utama dan dosen tim *team-teaching* (bila ada).
6. **Mata Kuliah Syarat (Baris 9)**:
   - Prasyarat yang harus sudah ditempuh (lulus) mahasiswa sebelum mengambil mata kuliah ini (misal: "Struktur Data" untuk mata kuliah "Algoritma Pemrograman"). Tuliskan "Tidak Ada" jika merupakan mata kuliah dasar.

---

### TABEL 2: Matriks Pembelajaran 16 Pertemuan (Jadwal Aktivitas Semester)
Tabel 8 Kolom:

| Kolom | Nama Kolom | Aturan Pengisian Standar OBE |
| :---: | :--- | :--- |
| **(1)** | **Mg Ke-** | Diisi angka 1 sampai 16 secara berurutan.<br>- **Minggu ke-8**: Wajib **UTS (Ujian Tengah Semester)**.<br>- **Minggu ke-16**: Wajib **UAS (Ujian Akhir Semester)**. |
| **(2)** | **Kemampuan akhir tiap tahapan belajar (Sub-CPMK)** | Sub-CPMK yang disasar pada minggu bersangkutan. Cantumkan kode Bloom `[C..., P..., A...]`. |
| **(3)** | **Penilaian: Indikator** | Pernyataan terukur mengenai bukti kinerja atau hasil belajar mahasiswa (misal: "Ketepatan dalam merancang diagram UML use-case dan class diagram sesuai studi kasus"). |
| **(4)** | **Penilaian: Teknik & Kriteria** | - **Teknik**: Tes tulis, kuis lisan/coding, observasi unjuk kerja, portofolio, presentasi.<br>- **Kriteria**: Rubrik analitik, pedoman penskoran (*Marking Scheme*). |
| **(5)** | **Bentuk Pembelajaran; Metode Pembelajaran; Penugasan Mahasiswa; [Estimasi Waktu] - LURING** | - Bentuk: Kuliah, responsi, praktikum lab.<br>- Metode SCL: *Case Method, Project-Based Learning (PjBL), Small Group Discussion*.<br>- Penugasan: Tugas-1, Latihan Lab, Resume.<br>- Estimasi Waktu: Tuliskan rincian `PB`, `PT`, `KM`. |
| **(6)** | **Bentuk Pembelajaran; Metode Pembelajaran; Penugasan Mahasiswa; [Estimasi Waktu] - DARING** | Aktivitas sinkronus (Zoom/Google Meet) atau asinkronus via LMS (e-learning/moodle), forum diskusi daring, pengumpulan tugas daring. |
| **(7)** | **Materi Pembelajaran [Pustaka]** | Rincian pokok bahasan pertemuan dan kode rujukan pustaka (misal: `[Pressman20, Bab 3, Hal 45-60]`). Pada pertemuan 1 sertakan "Penjelasan RPS, Kontrak Perkuliahan". |
| **(8)** | **Bobot Penilaian (%)** | Persentase kontribusi evaluasi minggu tersebut terhadap nilai akhir semester. Baris paling bawah menjumlahkan total bobot menjadi **100%**. |

---

## 3. Standar Alokasi Waktu SKS (SN-Dikti / Permendikbudristek)

Keterangan singkatan resmi di dokumen UNIROW:
- **PB**: Proses Belajar / Kegiatan Belajar Terbimbing (Tatap Muka di kelas/lab)
- **PT**: Kegiatan Penugasan Terstruktur (Tugas rumah, kuis, resume, laporan lab)
- **KM**: Kegiatan Mandiri (Mempelajari materi ajar, referensi, eksplorasi kode)

### Formula Alokasi Waktu per SKS (Bentuk Kuliah / Teori):
- 1 SKS = 50 menit PB + 60 menit PT + 60 menit KM per minggu.

### Rincian Alokasi Berdasarkan Beban SKS Mata Kuliah:
1. **Mata Kuliah 2 SKS (Total 340 menit/minggu)**:
   - `PB: 2 x 50 menit = 100 menit`
   - `PT: 2 x 60 menit = 120 menit`
   - `KM: 2 x 60 menit = 120 menit`
   - *Format penulisan RPS*: `[PB: 1x(2x50')], [PT: 1x(2x60')], [KM: 1x(2x60')]`
2. **Mata Kuliah 3 SKS (Total 510 menit/minggu)**:
   - `PB: 3 x 50 menit = 150 menit`
   - `PT: 3 x 60 menit = 180 menit`
   - `KM: 3 x 60 menit = 180 menit`
   - *Format penulisan RPS*: `[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]`
3. **Mata Kuliah 4 SKS (Total 680 menit/minggu)**:
   - `PB: 4 x 50 menit = 200 menit`
   - `PT: 4 x 60 menit = 240 menit`
   - `KM: 4 x 60 menit = 240 menit`
   - *Format penulisan RPS*: `[PB: 1x(4x50')], [PT: 1x(4x60')], [KM: 1x(4x60')]`
4. **Bentuk Praktikum / Praktik Bengkel / Studio (1 SKS = 170 menit)**:
   - Praktikum 1 SKS: `[Praktikum: 1x(1x170')]`
   - Praktikum 2 SKS: `[Praktikum: 1x(2x170')] = 340 menit/minggu`

---

## 4. Lembar Validasi Dokumen
Pada bagian akhir dokumen RPS, terdapat lembar pengesahan dan penjaminan mutu:
- Kalimat: `RPS ini telah divalidasi pada tanggal [dd Bulan YYYY]`
- Kolom Tanda Tangan:
  * Kiri: `Ketua Program Studi [Nama Prodi]`, `(Nama Kaprodi lengkap gelar)`, `NIDN: ...`
  * Kanan: `UJM Program Studi [Nama Prodi]`, `(Nama Ketua UJM lengkap gelar)`, `NIDN: ...`
