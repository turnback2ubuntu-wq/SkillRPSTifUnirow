# RENCANA PEMBELAJARAN SEMESTER (RPS)
## PROGRAM STUDI S1 INFORMATIKA — FAKULTAS SAINS DAN TEKNOLOGI
### UNIVERSITAS PGRI RONGGOLAWE (UNIROW) TUBAN

**Kode Dokumen**: `RPS-INF-IF440524`  
**Tanggal Penyusunan**: `24 September 2026`

---

## I. IDENTITAS MATA KULIAH

| Item | Keterangan |
| :--- | :--- |
| **Nama Mata Kuliah (MK)** | **Basis Data Lanjut** |
| **Kode Mata Kuliah** | **IF440524** |
| **Rumpun Mata Kuliah (RMK)** | Rekayasa Perangkat Lunak & Data |
| **Bobot SKS** | **3 SKS** (Teori & Praktik Terintegrasi) |
| **Semester** | 4 (Empat) |
| **Dosen Pengembang RPS** | **ANDY HARYOKO, ST., MT** |
| **Koordinator RMK** | **ANDY HARYOKO, ST., MT** |
| **Ketua Program Studi** | **AMALUDIN ARIFIA, M.Kom.** |
| **Dosen Pengampu** | **ANDY HARYOKO, ST., MT** |
| **Mata Kuliah Prasyarat** | MK26 Basis Data, MK06 Algoritma Pemrograman |

---

## II. CAPAIAN PEMBELAJARAN

### A. Capaian Pembelajaran Lulusan (CPL-PRODI) yang Dibebankan pada MK
1. **CPL03**: Memiliki kemampuan memahami cara kerja sistem komputer serta menerapkan berbagai algoritma/metode untuk memecahkan masalah dalam suatu organisasi. `[C2, C3]`
2. **CPL04**: Memiliki kompetensi dalam menganalisis persoalan *computing* yang kompleks untuk mengidentifikasi solusi pengelolaan proyek teknologi di bidang informatika/ilmu komputer dengan mempertimbangkan perkembangan ilmu transdisiplin. `[C4]`
3. **CPL08**: Memiliki kemampuan untuk mengimplementasikan kebutuhan *computing* dengan menggunakan berbagai metode/algoritma yang sesuai dengan kebutuhan pengguna. `[C3, C4, C5]`

### B. Capaian Pembelajaran Mata Kuliah (CPMK) & Persentase Kontribusi
1. **CPMK1 (Kontribusi 100% terhadap CPL03)**:  
   *Mampu menganalisis arsitektur internal Database Management System (DBMS), struktur penyimpanan data fisik (indexing, B+ Tree, Hash), serta mekanisme pemrosesan dan optimasi query (query optimization & execution plans) `[C4]`.*
2. **CPMK2 (Kontribusi 100% terhadap CPL04)**:  
   *Mampu mengevaluasi manajemen transaksi ACID, protokol kontrol konkurensi (2PL, Timestamping, MVCC), teknik crash recovery (Write-Ahead Logging, ARIES), serta merancang tata kelola keamanan basis data enterprise `[C5]`.*
3. **CPMK3 (Kontribusi 100% terhadap CPL08)**:  
   *Mampu mengimplementasikan pemrograman basis data tingkat lanjut (Stored Procedures, Triggers, Views, CTE) serta merancang arsitektur basis data terdistribusi (sharding, replikasi) dan non-relasional (NoSQL: MongoDB, Redis) `[C6, P4]`.*

### C. Kemampuan Akhir Tiap Tahapan Belajar (Sub-CPMK)
- **Sub-CPMK 1**: Mahasiswa mampu menjelaskan arsitektur internal DBMS, hirarki penyimpanan memori-disk, organisasi file rekaman, dan algoritma indexing (B+ Tree & Hash Index) `[C2, A2]`. *(Bobot: 5%, 2 Minggu)*
- **Sub-CPMK 2**: Mahasiswa mampu mengimplementasikan pemrograman database tingkat lanjut menggunakan Stored Procedure, Triggers, Cursor, User-Defined Functions, dan Window Functions untuk otomatisasi logika bisnis `[C3, P4]`. *(Bobot: 10%, 2 Minggu)*
- **Sub-CPMK 3**: Mahasiswa mampu menganalisis rencana eksekusi query (EXPLAIN ANALYZE), mengestimasi cost operasi relasional, dan melakukan optimasi query (*query tuning*) berbasis strategi indeks `[C4, P4]`. *(Bobot: 10%, 2 Minggu)*
- **Sub-CPMK 4**: Mahasiswa mampu menganalisis siklus hidup transaksi ACID, anomali konkurensi (Dirty Read, Non-repeatable Read, Phantom Read), dan mekanisme penguncian Two-Phase Locking (2PL) serta deadlock handling `[C4]`. *(Bobot: 10%, 1 Minggu)*
- **Sub-CPMK 5**: Mahasiswa mampu mengevaluasi algoritma crash recovery (Write-Ahead Logging & Checkpointing) serta merancang tata kelola keamanan basis data (Role-Based Access Control, enkripsi data, dan proteksi SQL Injection) `[C5, A3]`. *(Bobot: 10%, 2 Minggu)*
- **Sub-CPMK 6**: Mahasiswa mampu merancang arsitektur basis data terdistribusi (fragmentasi horizontal/vertikal, replikasi data master-slave/multi-master, dan partisi/sharding) dengan mempertimbangkan Teorema CAP `[C6, P4]`. *(Bobot: 15%, 3 Minggu)*
- **Sub-CPMK 7**: Mahasiswa mampu mengimplementasikan dan mengevaluasi basis data non-relasional (NoSQL: Document Store MongoDB dan In-Memory Cache Redis) untuk penanganan data tak terstruktur dan kinerja tinggi `[C5, P4]`. *(Bobot: 10%, 2 Minggu)*
- **Sub-CPMK 8 (UTS & UAS)**: Mahasiswa mampu mendemonstrasikan evaluasi penguasaan teoretis melalui UTS tertulis (15%) dan unjuk kerja proyek optimasi serta integrasi basis data enterprise melalui UAS (15%) `[C5, C6, P5, A4]`. *(Bobot: 30%, 2 Minggu)*

---

## III. MATRIKS KORELASI CPL TERHADAP SUB-CPMK

| Sub-CPMK | CPL03 | CPL04 | CPL08 | Bobot Penilaian (%) | Jumlah Minggu |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Sub-CPMK 1** | **V** | | | 5% | 2 Minggu |
| **Sub-CPMK 2** | | | **V** | 10% | 2 Minggu |
| **Sub-CPMK 3** | **V** | | | 10% | 2 Minggu |
| **Sub-CPMK 4** | | **V** | | 10% | 1 Minggu |
| **Sub-CPMK 5** | | **V** | | 10% | 2 Minggu |
| **Sub-CPMK 6** | | | **V** | 15% | 3 Minggu |
| **Sub-CPMK 7** | | | **V** | 10% | 2 Minggu |
| **Sub-CPMK 8 (UTS & UAS)** | **V** | **V** | **V** | 30% | 2 Minggu |
| **Total Akumulasi** | | | | **100%** | **16 Minggu** |

---

## IV. DESKRIPSI SINGKAT & BAHAN KAJIAN

### Deskripsi Singkat Mata Kuliah
Mata kuliah **Basis Data Lanjut (IF440524)** membekali mahasiswa dengan kompetensi teoritis dan praktis mendalam mengenai arsitektur internal, optimasi, administrasi, dan skalabilitas sistem manajemen basis data (DBMS) tingkat lanjut. Pokok bahasan mencakup struktur penyimpanan fisik data, teknik indexing (B+ Tree dan Hash), pemrograman basis data prosedural (Stored Procedures, Triggers, Views, Window Functions), pemrosesan dan optimasi query (*Cost-Based Query Optimization & Execution Plans*), manajemen transaksi ACID, kontrol konkurensi (Two-Phase Locking & MVCC), sistem pemulihan kegagalan (Write-Ahead Logging & ARIES recovery), tata kelola keamanan basis data enterprise, arsitektur basis data terdistribusi (fragmentasi, replikasi, sharding, Teorema CAP), serta implementasi basis data non-relasional (NoSQL Document Store MongoDB dan In-Memory Caching Redis). Pembelajaran menggunakan pendekatan *Case Method* dan *Project-Based Learning* (PjBL) untuk menyelesaikan persoalan performa data berskala besar.

### Bahan Kajian (Materi Pembelajaran)
1. **Arsitektur Internal DBMS & Penyimpanan Fisik**: Hirarki memori, manajemen buffer pool, disk blocks, dan organisasi file rekaman (heap, sorted, hashed).
2. **Struktur Indeksasi Data**: Konsep indeks primer vs sekunder, B+ Tree indexing (pencarian, penyisipan, penghapusan), Hash Index, dan Bitmap Index.
3. **Pemrograman Basis Data Lanjut**: Stored Procedures, User-Defined Functions (UDF), Triggers (BEFORE/AFTER, Row-level vs Statement-level), Cursor, CTE, dan Window Functions.
4. **Pemrosesan & Optimasi Query (Query Processing & Optimization)**: Translasi query ke aljabar relasional, estimasi biaya operasi join (Nested-loop, Block, Hash Join), analisis EXPLAIN ANALYZE, dan query tuning.
5. **Manajemen Transaksi & Kontrol Konkurensi**: Konsep ACID, jadwal serializable, anomali konkurensi (Dirty Read, Phantom Read), protokol Two-Phase Locking (2PL), Deadlock detection & prevention, dan Multi-Version Concurrency Control (MVCC).
6. **Sistem Pemulihan (Database Crash Recovery)**: Klasifikasi kegagalan, prinsip Write-Ahead Logging (WAL), Checkpointing, dan algoritma ARIES (Analysis, Redo, Undo).
7. **Keamanan Basis Data & Audit**: Model otorisasi Role-Based Access Control (RBAC), enkripsi data (Transparent Data Encryption & SSL/TLS), audit logging, dan proteksi injeksi SQL.
8. **Basis Data Terdistribusi (Distributed DBMS)**: Arsitektur DDBMS, fragmentasi data (horizontal, vertikal, hibrid), replikasi sinkronus vs asinkronus, protokol Two-Phase Commit (2PC), dan Teorema CAP.
9. **Skalabilitas & Partisi Data**: Horizontal partitioning (Sharding), penentuan sharding key, rebalancing shard, dan konsistensi data terdistribusi.
10. **Basis Data Non-Relasional (NoSQL)**: Paradigma NoSQL vs RDBMS, Document Store (MongoDB: skema fleksibel, CRUD, aggregation pipeline, indexing NoSQL).
11. **In-Memory Database & Caching**: Arsitektur in-memory, Redis data structures (Strings, Hashes, Lists, Sets), caching pattern (Cache-Aside, Write-Through), dan session storage.
12. **Poliglot Persistence & Arsitektur Data Modern**: Mengintegrasikan RDBMS, NoSQL, dan Cache dalam satu solusi aplikasi terpadu berskala enterprise.

### Daftar Pustaka
#### Utama:
1. Silberschatz, A., Korth, H. F., & Sudarshan, S. (2020). *Database System Concepts* (7th ed.). New York: McGraw-Hill Education.
2. Elmasri, R., & Navathe, S. B. (2017). *Fundamentals of Database Systems* (7th ed.). Boston: Pearson Education.

#### Pendukung:
1. Celko, J. (2014). *Joe Celko's SQL for Smarties: Advanced SQL Programming* (5th ed.). Waltham, MA: Morgan Kaufmann.
2. Kleppmann, M. (2017). *Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems*. Sebastopol, CA: O'Reilly Media.
3. Chodorow, K. (2013). *MongoDB: The Definitive Guide: Powerful and Scalable Data Storage* (2nd ed.). O'Reilly Media.
4. PostgreSQL Global Development Group. (2024). *PostgreSQL 16 Documentation*. Online: https://www.postgresql.org/docs/16/

---

## V. MATRIKS PEMBELAJARAN 16 PERTEMUAN (FORMAT RPS UNIROW)

*Alokasi Waktu 3 SKS Kuliah:*  
`[PB (Proses Belajar): 1x(3x50') = 150 menit]`, `[PT (Penugasan Terstruktur): 1x(3x60') = 180 menit]`, `[KM (Kegiatan Mandiri): 1x(3x60') = 180 menit]`

| Mg Ke- | Kemampuan Akhir Tahapan Belajar (Sub-CPMK) | Penilaian: Indikator | Penilaian: Teknik & Kriteria | Bentuk & Metode SCL; Penugasan; [Estimasi Waktu] - Luring | Bentuk Pembelajaran; [Estimasi Waktu] - Daring | Materi Pembelajaran [Pustaka] | Bobot Penilaian (%) |
| :---: | :--- | :--- | :--- | :--- | :--- | :--- | :---: |
| **1** | **Sub-CPMK 1** `[C2, A2]` | Ketepatan dalam menjelaskan arsitektur internal DBMS, alur data dari disk ke buffer pool memori, organisasi blok penyimpanan, dan perbedaan strategi penyimpanan baris vs kolom. | Teknik non-tes: Tanya jawab interaktif & resume materi arsitektur storage.<br>Kriteria: Rubrik Partisipasi Kelas. | Kuliah interaktif, pemaparan RPS dan kontrak kuliah, diskusi arsitektur internal storage engine (InnoDB/Postgres).<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Mengunduh RPS, membaca materi Bab 12 Silberschatz, dan mengisi form komitmen belajar. | Arsitektur Penyimpanan DBMS: Hirarki storage (RAM, NVMe, HDD), manajemen buffer pool, struktur blok database, row vs columnar storage.<br>*[Silberschatz20: Bab 12], [Elmasri17: Bab 16]* | 2.5% |
| **2** | **Sub-CPMK 1** `[C2, A2]` | Ketepatan menganalisis struktur indeks pohon B+ Tree (node split, balancing, pencarian range query) dan membandingkannya dengan Hash Index. | Teknik non-tes: Latihan visualisasi struktur B+ Tree dan simulasi operasi insert/delete.<br>Kriteria: Marking Scheme Struktur Indeks. | Small Group Discussion & Tutorial: Simulasi manual penyeimbangan pohon B+ Tree pada berbagai skenario operasi manipulasi data.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Mengerjakan simulasi interaktif B+ Tree visualizer dan mengunggah hasil latihan. | Struktur Indeksasi Data: Konsep indexing primer vs sekunder, B+ Tree Index (struktur node, pencarian range), Hash Index, dan Bitmap Index.<br>*[Silberschatz20: Bab 14], [Elmasri17: Bab 17]* | 2.5% |
| **3** | **Sub-CPMK 2** `[C3, P4]` | Kemampuan menulis query SQL analitis kompleks menggunakan Window Functions (ROW_NUMBER, RANK, DENSE_RANK, LAG/LEAD) dan Recursive Common Table Expressions (CTE). | Teknik non-tes: Praktik lab penulisan query agregasi analitis lanjutan.<br>Kriteria: Rubrik Pemrograman SQL Analitis. | Praktik laboratorium komputer: Hands-on penulisan query analitik transaksi penjualan dan navigasi struktur hirarki data dengan Recursive CTE.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Pengunggahan skrip SQL latihan mandiri dan review kode query oleh dosen. | Advanced SQL I: Window Functions (Partition by, Order by, Frame clause), Common Table Expressions (CTE), dan hierarki data rekursif.<br>*[Celko14: Bab 23], [Postgres24]* | 5.0% |
| **4** | **Sub-CPMK 2** `[C3, P4]` | Kemampuan mengimplementasikan Stored Procedures, User-Defined Functions, Triggers, dan pengelolaan transaksi atomik di dalam kode prosedural (PL/pgSQL). | Teknik non-tes: **Tugas-1 (Pemrograman Database Tingkat Lanjut)**.<br>Kriteria: Rubrik Pemrograman Database Skala 1-5. | Workshop perancangan business logic di sisi database: Pembuatan trigger otomatisasi audit saldo rekening dan enkapsulasi prosedur transaksi.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Pengumpulan berkas Tugas-1 (File skrip .sql dan laporan pengujian fungsional). | Advanced SQL II & Prosedural: Sintaks PL/pgSQL, variabel, kontrol alur, exception handling, Stored Procedure vs Function, Trigger BEFORE/AFTER, Cursor.<br>*[Silberschatz20: Bab 5], [Celko14: Bab 28]* | **5.0%** |
| **5** | **Sub-CPMK 3** `[C4, P4]` | Ketepatan menjelaskan tahapan pemrosesan query (parsing, query tree rewrite, estimasi cost), algoritma join (Nested-loop, Hash Join, Merge Join), dan faktor penentu cost query. | Teknik non-tes: Analisis perbandingan algoritma join dan kalkulasi I/O cost.<br>Kriteria: Marking Scheme Algoritma Join. | Kuliah interaktif dan diskusi matematis: Menghitung jumlah transfer disk block pada Nested-loop Join vs Block Nested-loop vs Hash Join.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Mengakses video tutorial mengenai internal query execution engine. | Query Processing & Relational Algebra: Langkah query processing, query translation, representasi query tree, dan algoritma evaluasi operator.<br>*[Silberschatz20: Bab 15], [Elmasri17: Bab 18]* | 5.0% |
| **6** | **Sub-CPMK 3** `[C4, P4]` | Kemampuan membaca rencana eksekusi (EXPLAIN ANALYZE), mendeteksi Full Table Scan yang tidak efisien, dan melakukan query tuning dengan strategi indeks komposit. | Teknik non-tes: **Tugas-2 (Optimasi Query pada Dataset Skala Besar > 1 Juta Baris)**.<br>Kriteria: Rubrik Optimasi Query Skala 1-5. | Hands-on lab: Eksplorasi execution plan pada database PostgreSQL dengan dataset riil, benchmarking response time sebelum dan sesudah indexing.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Pengumpulan berkas laporan Tugas-2 (Grafik perbandingan execution time dan analisis query plan). | Cost-Based Query Optimization & Index Tuning: Membaca EXPLAIN plan, Sequential Scan vs Index Scan, Covering Index, Partial Index, refactoring subquery.<br>*[Silberschatz20: Bab 16], [Postgres24]* | **5.0%** |
| **7** | **Sub-CPMK 4** `[C4]` | Ketepatan menganalisis status transaksi, konsep jadwal serializability (Conflict vs View Serializability), dan pengujian jadwal transaksi dengan Precedence Graph. | Teknik non-tes: Latihan analisis Precedence Graph jadwal transaksi.<br>Kriteria: Marking Scheme Serializability. | Problem-Based Learning: Analisis skenario eksekusi transaksi konkuren, pembuatan Precedence Graph untuk mendeteksi siklus nonserializable.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Kuis latihan mandiri mengenai sifat ACID dan pengujian serializability. | Manajemen Transaksi: Status transaksi (Active, Failed, Committed), sifat ACID, Conflict Serializability, Precedence Graph.<br>*[Silberschatz20: Bab 17], [Elmasri17: Bab 20]* | 10.0% |
| **8** | **Sub-CPMK 1, 2, 3, 4** `[C4, C5]` | Penguasaan konsep teoritis arsitektur storage, struktur B+ Tree, query execution plan, optimasi indexing, dan serializability transaksi. | Teknik Tes: **Ujian Tertulis Tengah Semester (UTS)** berbentuk soal analisis kasus dan optimasi query.<br>Kriteria: Pedoman Penskoran Kunci Jawaban UTS. | **UJIAN TENGAH SEMESTER (UTS)**: Evaluasi Terjadwal Tertulis di Ruang Kelas.<br>`[PB: 1x(3x50')]` | LMS Unirow: Pengunggahan arsip lembar jawaban dan berita acara pelaksanaan UTS. | Evaluasi Komprehensif Materi Minggu 1 s.d. 7 (Storage, B+ Tree, Advanced SQL, Query Optimization, dan Transaksi Serializability).<br>*[Silberschatz20], [Elmasri17], [Celko14]* | **15.0%** |
| **9** | **Sub-CPMK 4** `[C4]` | Ketepatan menjelaskan protokol Two-Phase Locking (Strict/Rigorous 2PL), penanganan deadlock (Wait-Die, Wound-Wait), dan implementasi Multi-Version Concurrency Control (MVCC). | Teknik non-tes: Simulasi deadlock dan observasi isolasi transaksi di database.<br>Kriteria: Marking Scheme Concurrency Control. | Eksperimen lab: Membuka dua session transaksi simultan di PostgreSQL, mensimulasikan deadlock, dan memverifikasi cara kerja MVCC snapshot.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Forum diskusi mengenai perbandingan mekanisme penguncian pesimistik vs optimistik. | Kontrol Konkurensi: Lock types (Shared vs Exclusive), Two-Phase Locking (2PL), Deadlock prevention & detection (Wait-For Graph), dan MVCC.<br>*[Silberschatz20: Bab 18], [Kleppmann17: Bab 7]* | 5.0% |
| **10** | **Sub-CPMK 5** `[C5, A3]` | Ketepatan menganalisis pemulihan kegagalan sistem basis data menggunakan Write-Ahead Logging (WAL), Checkpointing, dan fasa algoritma ARIES (Analysis, Redo, Undo). | Teknik non-tes: Studi kasus rekonstruksi log transaksi pasca crash server.<br>Kriteria: Marking Scheme Crash Recovery. | Kuliah interaktif & latihan analisis: Merekonstruksi log file database setelah terjadi power outage menggunakan algoritma ARIES.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Mempelajari modul teknis Write-Ahead Logging pada mesin engine database. | Sistem Pemulihan (Recovery System): Klasifikasi kegagalan, log-based recovery, Write-Ahead Logging (WAL), Checkpointing, dan algoritma ARIES.<br>*[Silberschatz20: Bab 19], [Elmasri17: Bab 22]* | 5.0% |
| **11** | **Sub-CPMK 5** `[C5, A3]` | Kemampuan mengonfigurasi Role-Based Access Control (RBAC), enkripsi data (TDE & koneksi SSL/TLS), audit trail, dan teknik mitigasi serangan SQL Injection. | Teknik non-tes: Praktik lab konfigurasi user privileges, audit logging, dan secure parameterized queries.<br>Kriteria: Rubrik Keamanan Database. | Praktik lab: Konfigurasi RBAC (GRANT/REVOKE), pengujian celah keamanan injeksi SQL dan pencegahannya dengan prepared statements.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Submission laporan praktik pengamanan database dan berkas konfigurasi SSL. | Keamanan Basis Data: Hak akses pengguna (RBAC), Row-Level Security (RLS), enkripsi data at-rest & in-transit, database auditing, dan secure coding.<br>*[Silberschatz20: Bab 8], [Elmasri17: Bab 23]* | 5.0% |
| **12** | **Sub-CPMK 6** `[C6, P4]` | Ketepatan merancang fragmentasi data (horizontal & vertikal), arsitektur replikasi (Streaming Replication), dan menganalisis Teorema CAP pada sistem terdistribusi. | Teknik non-tes: Desain arsitektur basis data terdistribusi dan analisis trade-off konsistensi vs ketersediaan.<br>Kriteria: Marking Scheme Sistem Terdistribusi. | Kuliah interaktif & studi kasus: Merancang skema fragmentasi data cabang perbankan nasional dan strategi replikasi data multi-region.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Mengakses video materi mengenai Teorema CAP dan model konsistensi PACELC. | Basis Data Terdistribusi I: Homogeneous vs Heterogeneous DDBMS, fragmentasi (horizontal/vertikal), replikasi data, Teorema CAP.<br>*[Silberschatz20: Bab 20], [Kleppmann17: Bab 5 & 8]* | 5.0% |
| **13** | **Sub-CPMK 6** `[C6, P4]` | Kemampuan mengonfigurasi horizontal sharding, protokol Two-Phase Commit (2PC), dan load balancing read/write query pada kluster database. | Teknik non-tes: Praktik kluster database terdistribusi & demonstrasi failover otomatis.<br>Kriteria: Rubrik Implementasi Sharding/Replikasi. | Praktik lab: Konfigurasi Streaming Replication pada PostgreSQL / MySQL Group Replication dan simulasi failover master node.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Pengunggahan skrip setup kluster database dan log pengujian replikasi. | Basis Data Terdistribusi II: Distributed Transactions, Two-Phase Commit (2PC), Sharding strategi (Hash vs Range Sharding), Citus/Vitess overview.<br>*[Silberschatz20: Bab 21], [Kleppmann17: Bab 6 & 9]* | 5.0% |
| **14** | **Sub-CPMK 7** `[C5, P4]` | Kemampuan memodelkan dokumen JSON/BSON pada MongoDB, mengeksekusi query CRUD, membangun aggregation pipeline kompleks, dan merancang indeks NoSQL. | Teknik non-tes: **Tugas-3 (Proyek Basis Data Terdistribusi & Poliglot Persistence)**.<br>Kriteria: Rubrik Proyek Database Skala 1-5. | Hands-on lab MongoDB: Pemodelan data fleksibel (Embedding vs Referencing), aggregation pipeline (Match, Group, Project, Lookup), indexing dokumen.<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Pengumpulan berkas repositori proyek dan draf dokumen arsitektur Tugas-3. | Basis Data NoSQL Document Store: Paradigma NoSQL, MongoDB architecture, JSON/BSON, Aggregation Framework, indexing NoSQL.<br>*[Chodorow13: Bab 1-8], [Silberschatz20: Bab 22]* | **5.0%** |
| **15** | **Sub-CPMK 7** `[C5, P4]` | Kemampuan mengintegrasikan In-Memory Database (Redis) sebagai caching layer untuk mempercepat throughput baca data dan mengurangi beban database utama. | Teknik non-tes: Unjuk kerja benchmarking throughput aplikasi menggunakan pola Cache-Aside dengan Redis.<br>Kriteria: Marking Scheme In-Memory Cache. | Project mentoring: Integrasi arsitektur Poliglot Persistence (PostgreSQL relasional, MongoDB dokumen log, Redis in-memory cache).<br>`[PB: 1x(3x50')], [PT: 1x(3x60')], [KM: 1x(3x60')]` | LMS Unirow: Benchmark report throughput request/second dengan dan tanpa Redis caching. | In-Memory Database & Poliglot Persistence: Redis data structures (String, Hash, Set, ZSet), strategi cache-aside, cache invalidation.<br>*[Kleppmann17: Bab 11], [Silberschatz20: Bab 22]* | 5.0% |
| **16** | **Sub-CPMK 5, 6, 7, 8** `[C5, C6, P5, A4]` | Kualitas implementasi proyek basis data terdistribusi terpadu, efisiensi optimasi query, ketangguhan failover kluster, dan kemahiran dalam demonstrasi live demo serta tanya jawab. | Teknik Tes & Non-Tes: **Ujian Akhir Semester (UAS)** Expo Presentasi & Live Demo Proyek Basis Data Enterprise Berkelompok.<br>Kriteria: Rubrik Evaluasi Proyek Capstone Skala 1-5. | **UJIAN AKHIR SEMESTER (UAS)**: Sesi demo langsung sistem basis data terdistribusi di hadapan dosen penguji, evaluasi kinerja query, dan uji ketahanan sistem saat failover.<br>`[PB: 1x(3x50')]` | LMS Unirow: Pengumpulan repositori Git proyek lengkap, video demo, skrip DDL/NoSQL, dan dokumen Laporan Akhir Proyek. | Evaluasi Akhir: Kompilasi seluruh modul (Storage, Indexing, Query Optimization, Concurrency, Distributed DB, NoSQL, & Caching).<br>*Seluruh Pustaka* | **15.0%** |
| **Total** | | | | | | | **100.0%** |

---

## VI. RANCANGAN TUGAS TERSTRUKTUR MAHASISWA

### TUGAS 1: Pemrograman Basis Data Lanjut: Stored Procedures, Functions, & Complex Audit Triggers
- **Sub-CPMK yang Disasar**: Sub-CPMK 2 `[C3, P4]`
- **Bentuk Tugas / Alokasi Waktu**: Kelompok (3-4 Mahasiswa) | Minggu ke-3 s.d. ke-4 (2 Minggu)
- **Deskripsi Pengerjaan**: Mahasiswa secara berkelompok merancang dan mengimplementasikan serangkaian modul pemrograman basis data prosedural (PL/pgSQL) untuk studi kasus sistem keuangan/perbankan digital. Modul mencakup Stored Procedure pemrosesan transfer dana atomik, Triggers pencegahan saldo negatif dan pencatatan audit log otomatis ke tabel riwayat, serta Window Functions untuk laporan ringkasan pergerakan dana bulanan.
- **Indikator Penilaian**: Ketepatan enkapsulasi transaksi atomik, ketepatan penanganan exception/rollback, keabsahan fungsi trigger audit, dan efisiensi sintaks Window Functions.
- **Bentuk & Format Luaran**: Berkas skrip SQL executable (.sql) dan Dokumen Laporan Pengujian Fungsional (PDF). (Bobot: 10%)

### TUGAS 2: Benchmarking, Analisis Rencana Eksekusi (EXPLAIN ANALYZE), dan Optimasi Query pada Dataset Skala Besar
- **Sub-CPMK yang Disasar**: Sub-CPMK 3 `[C4, P4]`
- **Bentuk Tugas / Alokasi Waktu**: Kelompok (3-4 Mahasiswa) | Minggu ke-5 s.d. ke-6 (2 Minggu)
- **Deskripsi Pengerjaan**: Kelompok mengimpor dataset berskala besar (> 1.000.000 baris data transaksi nyata). Mahasiswa menyusun 5 skenario query kompleks multi-table join, melakukan profiling sebelum optimasi menggunakan EXPLAIN ANALYZE, mendeteksi sequential scans berbiaya tinggi, merancang strategi indeks komposit/partial yang optimal, serta membuktikan penurunan execution time secara empiris.
- **Indikator Penilaian**: Kedalaman analisis execution plan, ketepatan strategi pemilihan kolom indeks, eliminasi operasi berbiaya tinggi, dan validitas data perbandingan latency/execution time sebelum dan sesudah optimasi.
- **Bentuk & Format Luaran**: Dokumen Laporan Optimasi Query (PDF) disertai tangkapan layar EXPLAIN ANALYZE dan skrip DDL indexing. (Bobot: 10%)

### TUGAS 3: Perancangan Arsitektur Basis Data Terdistribusi dan Integrasi Poliglot Persistence (RDBMS + NoSQL + Redis)
- **Sub-CPMK yang Disasar**: Sub-CPMK 6 & 7 `[C6, P4]`
- **Bentuk Tugas / Alokasi Waktu**: Kelompok (3-4 Mahasiswa) | Minggu ke-12 s.d. ke-15 (4 Minggu)
- **Deskripsi Pengerjaan**: Kelompok membangun arsitektur data enterprise terpadu yang memadukan PostgreSQL Streaming Replication / Sharding untuk data transaksi utama, MongoDB Document Store untuk data katalog/log interaksi tak terstruktur, dan Redis In-Memory Cache untuk caching query berfrekuensi tinggi. Sistem diuji ketangguhannya terhadap peningkatan beban traffic (*load testing*) dan simulasi failover node database.
- **Indikator Penilaian**: Kebenaran konfigurasi replikasi/kluster, integrasi mulus antar tiga engine database (poliglot), efektivitas caching Redis dalam menaikkan throughput, dan ketahanan kluster saat simulasi kegagalan server.
- **Bentuk & Format Luaran**: Repositori GitHub berisi skrip provisioning (Docker Compose), skrip konfigurasi database, berkas benchmark performa, dan Laporan Akhir Proyek (PDF). (Bobot: 10%)

---

## VII. RUBRIK PENILAIAN OBE SKALA 1–5 (STANDAR APTIKOM & UNIROW)

| Skala | Kategori Mutu | Rentang Skor | Deskripsi Kinerja Ketercapaian |
| :---: | :---: | :---: | :--- |
| **5** | **Sangat Kompeten** | **81 – 100** | Mahasiswa menunjukkan penguasaan sangat mendalam terhadap arsitektur dan internal DBMS. Analisis execution plan query sangat tajam dan komprehensif, implementasi pemrograman database dan trigger bebas bug, arsitektur kluster terdistribusi dan NoSQL berjalan stabil dengan failover otomatis yang teruji, dokumentasi sangat sistematis, dan presentasi sangat meyakinkan. |
| **4** | **Kompeten** | **61 – 80** | Mahasiswa mampu menerapkan konsep basis data lanjut dengan baik. Analisis query optimization tepat dan mampu menurunkan waktu eksekusi secara nyata, trigger dan stored procedure berfungsi sesuai spesifikasi, kluster terdistribusi dan caching Redis terkonfigurasi dengan benar, laporan terstruktur rapi, dan kolaborasi tim berjalan efektif. |
| **3** | **Cukup Kompeten** | **41 – 60** | Mahasiswa memahami konsep dasar basis data lanjut. Query optimization mampu dijalankan namun indeks yang dirancang kurang optimal, fungsi prosedural berjalan untuk skenario normal namun minim error handling, kluster terdistribusi berjalan dasar tanpa uji beban yang memadai, dan dokumentasi memiliki beberapa kekurangan teknis. |
| **2** | **Kurang Kompeten** | **21 – 40** | Mahasiswa menunjukkan pemahaman terbatas mengenai basis data lanjut. Analisis rencana eksekusi keliru, stored procedure/trigger sering menghasilkan error, konfigurasi sistem terdistribusi atau NoSQL gagal dijalankan, dan dokumentasi penugasan sangat tidak lengkap. |
| **1** | **Tidak Kompeten** | **0 – 20** | Mahasiswa tidak mampu mendemonstrasikan capaian pembelajaran. Tidak mampu melakukan optimasi maupun perancangan basis data, tidak ada artefak kode skrip atau laporan yang diserahkan, atau terindikasi plagiarisme berat. |

---

## VIII. LEMBAR PENGESAHAN DAN VALIDASI

*RPS ini telah divalidasi pada tanggal 24 September 2026*

| Dosen Pengembang RPS & Koordinator RMK | Ketua Program Studi S1 Informatika | UJM Program Studi S1 Informatika |
| :---: | :---: | :---: |
| *(Tanda Tangan)* | *(Tanda Tangan)* | *(Tanda Tangan)* |
| **ANDY HARYOKO, ST., MT** | **AMALUDIN ARIFIA, M.Kom.** | **UJM Program Studi** |
| Dosen Pengampu | Ketua Program Studi | Penjaminan Mutu |
