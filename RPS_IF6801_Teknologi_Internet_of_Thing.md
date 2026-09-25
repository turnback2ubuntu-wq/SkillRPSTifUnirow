# RENCANA PEMBELAJARAN SEMESTER (RPS)
## PROGRAM STUDI S1 INFORMATIKA — FAKULTAS SAINS DAN TEKNOLOGI
### UNIVERSITAS PGRI RONGGOLAWE (UNIROW) TUBAN

**Kode Dokumen**: `RPS-INF-IF6801`  
**Tanggal Penyusunan**: `25 Agustus 2025`

---

## I. IDENTITAS MATA KULIAH

| Item | Keterangan |
| :--- | :--- |
| **Nama Mata Kuliah (MK)** | **Teknologi Internet of Thing** |
| **Kode Mata Kuliah** | **IF6801** |
| **Rumpun Mata Kuliah (RMK)** | Sistem Tertanam, Jaringan & Keamanan Komputer |
| **Bobot SKS** | **3 SKS** (Teori & Praktik Lab Terintegrasi) |
| **Semester** | 6 (Enam) / Peminatan IoT & Embedded Systems |
| **Dosen Pengembang RPS** | **Fitroh Amaluddin, M.Kom.** |
| **Koordinator RMK** | **Fitroh Amaluddin, M.Kom.** |
| **Ketua Program Studi** | **AMALUDIN ARIFIA, M.Kom.** |
| **Dosen Pengampu** | **Fitroh Amaluddin, M.Kom.** |
| **Mata Kuliah Prasyarat** | IF240224 Jaringan Komputer / Sistem Operasi |

---

## II. CAPAIAN PEMBELAJARAN

### A. Capaian Pembelajaran Lulusan (CPL-PRODI) yang Dibebankan pada MK
1. **CPL03**: Memiliki kemampuan memahami cara kerja sistem komputer serta menerapkan berbagai algoritma/metode untuk memecahkan masalah dalam suatu organisasi. `[C2, C3]`
2. **CPL04**: Memiliki kompetensi dalam menganalisis persoalan *computing* yang kompleks untuk mengidentifikasi solusi pengelolaan proyek teknologi di bidang informatika/ilmu komputer dengan mempertimbangkan perkembangan ilmu transdisiplin. `[C4]`
3. **CPL05**: Memiliki kemampuan merancang, mengimplementasikan, dan mengevaluasi solusi berbasis *computing* (sistem cerdas, embedded systems, IoT, cloud) yang memenuhi kebutuhan pengguna dengan pendekatan analitis dan saintifik. `[C5, C6]`
4. **CPL08**: Menunjukkan komitmen terhadap standar profesional, etika, tata kelola, dan kerja sama tim interdisipliner dalam pelaksanaan proyek teknologi. `[A3, A4]`

### B. Capaian Pembelajaran Mata Kuliah (CPMK) & Persentase Kontribusi
1. **CPMK1 (Kontribusi 100% terhadap CPL03)**:  
   *Mampu menjelaskan arsitektur referensi IoT, komponen sensor/aktuator, mikrokontroler (ESP32/Arduino), dan mengonfigurasi interkoneksi hardware serta interfacing I/O analog/digital dan komunikasi bus (I2C, SPI, UART) [C2, C3].*
2. **CPMK2 (Kontribusi 100% terhadap CPL04)**:  
   *Mampu menganalisis dan menerapkan protokol komunikasi IoT (MQTT, CoAP, HTTP REST, WebSocket) serta teknologi jaringan nirkabel (Wi-Fi, Bluetooth Low Energy, LoRaWAN) untuk pertukaran data telemetri yang hemat daya dan andal [C4].*
3. **CPMK3 (Kontribusi 100% terhadap CPL05)**:  
   *Mampu merancang dan mengintegrasikan platform cloud IoT (ThingsBoard, Firebase, Node-RED, InfluxDB/Grafana), dashboard analitik, dan inferensi Edge AI / TinyML sederhana [C5].*
4. **CPMK4 (Kontribusi 100% terhadap CPL08)**:  
   *Mampu bekerja sama dalam tim interdisipliner untuk merancang, mengimplementasikan, dan memvalidasi purwarupa sistem pintar IoT dunia nyata dengan memperhatikan aspek keamanan siber (TLS/SSL, autentikasi token) dan etika profesional [A4, C6].*

### C. Pemetaan Korelasi CPL, CPMK, Sub-CPMK, Bobot & Alokasi Waktu

| Sub-CPMK | CPL03 | CPL04 | CPL05 | CPL08 | CPMK Induk | Bobot Penilaian (%) | Alokasi Waktu |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Sub-CPMK 1**: Konsep IoT, arsitektur 4-layer, & studi kasus industri 4.0 `[C2]` | **V** | | | | CPMK1 | 3% | Minggu 1 (150' PB, 180' PT+BM) |
| **Sub-CPMK 2**: GPIO ESP32, sinyal analog ADC/DAC, PWM, & interfacing sensor `[C3]` | **V** | | | | CPMK1 | 4% | Minggu 2 (150' PB, 180' PT+BM) |
| **Sub-CPMK 3**: Protokol bus sensor cerdas: UART Serial, I2C Bus, & SPI `[C4]` | **V** | | | | CPMK1 | 7% | Minggu 3 (150' PB, 180' PT+BM) |
| **Sub-CPMK 4**: Konektivitas nirkabel Wi-Fi (STA/AP) & Bluetooth Low Energy (BLE) `[C3, C4]` | | **V** | | | CPMK2 | 6% | Minggu 4 (150' PB, 180' PT+BM) |
| **Sub-CPMK 5**: LPWAN, modulasi LoRa, & arsitektur LoRaWAN Gateway `[C4]` | | **V** | | | CPMK2 | 5% | Minggu 5 (150' PB, 180' PT+BM) |
| **Sub-CPMK 6**: Protokol publish-subscribe MQTT, topik hirarkis, & QoS `[C4]` | | **V** | | | CPMK2 | 5% | Minggu 6 (150' PB, 180' PT+BM) |
| **Sub-CPMK 7**: Protokol CoAP, WebSockets, & komparasi efisiensi telemetri `[C4]` | | **V** | | | CPMK2 | 5% | Minggu 7 (150' PB, 180' PT+BM) |
| **UTS (Evaluasi Tengah Semester)**: Ujian Teori & Live Coding Sirkuit Sensor | **V** | **V** | | | CPMK1,2 | 15% | Minggu 8 (150 Menit) |
| **Sub-CPMK 8**: Event-Driven Node-RED Flow Engine & UI Dashboard Otomasi `[C5]` | | | **V** | | CPMK3 | 5% | Minggu 9 (150' PB, 180' PT+BM) |
| **Sub-CPMK 9**: Integrasi Cloud ThingsBoard, Firebase, & Time-Series Grafana `[C5]` | | | **V** | | CPMK3 | 10% | Minggu 10–11 (300' PB, 360' PT+BM) |
| **Sub-CPMK 10**: Keamanan Komunikasi TLS/MQTTS, OTA Update, & Edge AI TinyML `[C4, C5]` | | | **V** | | CPMK3 | 8% | Minggu 12–13 (300' PB, 360' PT+BM) |
| **Sub-CPMK 11**: Integrasi Capstone IoT End-to-End, Validasi & Expo Tim `[A4, C6]` | | | | **V** | CPMK4 | 12% | Minggu 14–15 (300' PB, 360' PT+BM) |
| **UAS (Evaluasi Akhir Semester)**: Final Capstone Project Deliverable & Defense | | | **V** | **V** | CPMK3,4 | 15% | Minggu 16 (150 Menit) |
| **TOTAL** | | | | | | **100%** | **16 Minggu (48 Jam PB, 57.6 Jam PT+BM)** |

---

## III. DESKRIPSI SINGKAT MATA KULIAH

Mata kuliah **Teknologi Internet of Thing (IF6801)** membekali mahasiswa S1 Informatika dengan pemahaman teori mendalam dan keterampilan praktis komprehensif dalam merekayasa ekosistem Internet of Things (IoT) modern. Materi perkuliahan mencakup arsitektur 4-lapisan IoT, pemrograman sistem tertanam mikrokontroler modern (ESP32 SoC), interfacing aneka sensor/aktuator, protokol komunikasi bus (UART, I2C, SPI), serta jaringan nirkabel jarak pendek dan jarak jauh (Wi-Fi, Bluetooth Low Energy/BLE, dan LPWAN/LoRaWAN). Mahasiswa dilatih mengimplementasikan protokol perpesanan data telemetri hemat daya (MQTT, CoAP, HTTP REST, WebSocket), mengintegrasikan platform komputasi awan IoT (ThingsBoard, Firebase, Node-RED, InfluxDB/Grafana), menerapkan keamanan siber IoT (TLS/SSL, autentikasi berbasis token, pembaruan firmware nirkabel Over-The-Air/OTA), serta pengenalan komputasi tepi (Edge AI / TinyML). Perkuliahan menitikberatkan pada *Project-Based Learning* berbasis studi kasus nyata (*Smart Agriculture*, *Smart Environment*, *Smart Home*, *Industrial IoT*).

---

## IV. BAHAN KAJIAN & SUMBER PUSTAKA

### A. Bahan Kajian (Materi Pembelajaran)
1. Pengantar Ekosistem Internet of Things (IoT), Arsitektur Referensi 4-Lapisan, & Tren Industri 4.0
2. Arsitektur Mikrokontroler IoT (ESP32 SoC Architecture), GPIO, Interfacing Analog ADC/DAC, & PWM
3. Protokol Bus Komunikasi Periferal Sensor: UART Serial, I2C Bus Protocol, & SPI High-Speed Bus
4. Jaringan Nirkabel Jarak Pendek: Wi-Fi Networking (Station vs SoftAP) & Bluetooth Low Energy (BLE)
5. Jaringan Nirkabel Jarak Jauh Berdaya Rendah (LPWAN): Karakteristik Radio LoRa & Arsitektur LoRaWAN
6. Protokol Komunikasi Telemetri IoT: MQTT Broker Architecture, Topic Structure, & Quality of Service (QoS)
7. Protokol Ringan CoAP, HTTP REST, & WebSockets untuk Data Sensor Real-Time
8. Pemrosesan Data Event-Driven & Integrasi Middleware menggunakan Node-RED Flow Engine
9. Platform Komputasi Awan IoT: Arsitektur ThingsBoard (Rule Engine, Device Provisioning) & Firebase
10. Manajemen Data Sensor Time-Series: InfluxDB Database & Visualisasi Dashboard Interaktif Grafana
11. Keamanan Siber IoT: Enkripsi Komunikasi Data (MQTTS/HTTPS via TLS), Token Autentikasi, & Secure Boot
12. Pembaruan Firmware Nirkabel: Over-The-Air (OTA) Updates & Manajemen Daya Rendah (Deep Sleep Mode)
13. Pengenalan Edge Computing & TinyML: Inferensi Kecerdasan Buatan pada Mikrokontroler ESP32
14. Perancangan & Integrasi Purwarupa Produk Cerdas IoT Terpadu Berbasis Studi Kasus Nyata

### B. Daftar Referensi
**Pustaka Utama**:
1. Hanes, D., Salgueiro, G., Grossetete, P., Barton, R., & Henry, J. (2017). *IoT Fundamentals: Networking Technologies, Protocols, and Use Cases for the Internet of Things*. Cisco Press.
2. Buyya, R., & Dastjerdi, A. V. (2016). *Internet of Things: Principles and Paradigms*. Morgan Kaufmann / Elsevier.
3. Lea, P. (2020). *Internet of Things for Architects: Architecting IoT solutions by implementing sensors, communication infrastructure, edge computing, and cloud systems*. Packt Publishing.

**Pustaka Pendukung**:
1. Schwartz, M. (2018). *Internet of Things with ESP32*. Packt Publishing.
2. Warden, P., & Situnayake, D. (2019). *TinyML: Machine Learning with TensorFlow Lite on Arduino and Ultra-Low-Power Microcontrollers*. O'Reilly Media.
3. Al-Sarawi, S., Anbar, M., Alieyan, K., & Alzubi, M. (2017). *Internet of Things (IoT) communication protocols: Review*. IEEE IT.
4. Artikel Jurnal Ilmiah Bereputasi IEEE IoT Journal & ACM Transactions on Sensor Networks terkini.

---

## V. MATRIKS RENCANA PEMBELAJARAN 16 PERTEMUAN

| Mg | Sub-CPMK | Indikator Penilaian | Kriteria & Teknik | Bentuk & Metode Pembelajaran (Luring / Daring) | Materi Pembelajaran [Pustaka] | Bobot (%) |
| :---: | :--- | :--- | :--- | :--- | :--- | :---: |
| **1** | Sub-CPMK 1: Definisi, evolusi, arsitektur 4-layer IoT, dan studi kasus industri 4.0 `[C2]` | Ketepatan menjelaskan lapisan persepsi, jaringan, middleware, dan aplikasi | Kriteria: Kejelasan konsep; Teknik: Kuis interaktif | **Luring**: Kuliah interaktif, Diskusi, Studi Kasus Smart Agriculture Tuban (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Modul LMS, Video IoT | Pengenalan IoT, M2M vs IoT, Arsitektur 4-Lapisan, Tantangan IoT [Hanes Bab 1-2, Buyya Bab 1] | 3% |
| **2** | Sub-CPMK 2: GPIO ESP32, sinyal analog ADC/DAC, PWM, & interfacing sensor fisik `[C3]` | Keterampilan wiring pinout ESP32, pembacaan ADC, kontrol aktuator via PWM | Kriteria: Kebenaran rangkaian & kode firmware; Teknik: Praktikum Lab 1 | **Luring**: Praktikum Lab: Wiring Sensor/Aktuator & Serial Monitor (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Simulasi Wokwi di LMS | SoC ESP32, GPIO, Resolusi ADC/DAC, PWM Duty Cycle [Schwartz Bab 1-2] | 4% |
| **3** | Sub-CPMK 3: Komunikasi bus sensor: UART Serial, protokol I2C, dan antarmuka SPI `[C4]` | Baudrate UART, I2C address scanner, tampilan OLED, logging SPI MicroSD | Kriteria: Keberhasilan transmisi data bus; Teknik: Tugas Praktikum 2 | **Luring**: Praktikum Lab: I2C Scanner, OLED Display, Sensor BME280 & MicroSD (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Upload laporan praktikum di LMS | Protokol Bus: UART, I2C (SDA/SCL), SPI (MOSI, MISO, SCK, CS) [Lea Bab 3, Schwartz Bab 3] | 7% |
| **4** | Sub-CPMK 4: Konektivitas nirkabel Wi-Fi (STA/AP) & Bluetooth Low Energy (BLE) `[C3, C4]` | Koneksi ke AP, Web Server mandiri, BLE GATT Server (Service & Characteristic) | Kriteria: Stabilitas jaringan nirkabel & pairing; Teknik: Lembar Kerja Praktikum | **Luring**: Praktikum Pembuatan Web Server ESP32 & BLE Sensor Server (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Pengujian via nRF Connect di LMS | Wi-Fi 802.11 (STA vs SoftAP), BLE Architecture (GAP, GATT) [Hanes Bab 4, Schwartz Bab 4] | 6% |
| **5** | Sub-CPMK 5: Arsitektur LPWAN, modulasi radio LoRa, dan transmisi LoRaWAN `[C4]` | Pengaturan frekuensi 920-923 MHz AS923, Spreading Factor, pengujian jangkauan | Kriteria: Ketepatan link budget & packet loss; Teknik: Tugas Analisis Jaringan | **Luring**: Kuliah Interaktif, Demonstrasi Point-to-Point LoRa & Gateway di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Simulasi konsumsi daya LoRa di LMS | LPWAN, Modulasi LoRa (CSS), LoRaWAN Node & Gateway [Hanes Bab 4, Lea Bab 4] | 5% |
| **6** | Sub-CPMK 6: Protokol publish-subscribe MQTT, topik hirarkis, & QoS `[C4]` | Perancangan hirarki topik, retained message, LWT, klien Pub/Sub ESP32 | Kriteria: Integritas pengiriman telemetri & payload JSON; Teknik: Tugas MQTT | **Luring**: Praktikum Konfigurasi Broker Mosquitto & Publish-Subscribe Data Sensor (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Testing via MQTTX di LMS | Publish-Subscribe MQTT, Topik Hirarkis, Level QoS (0, 1, 2), Broker Mosquitto [Hanes Bab 5, Buyya Bab 4] | 5% |
| **7** | Sub-CPMK 7: Protokol CoAP, WebSockets, & komparasi efisiensi telemetri `[C4]` | Pengukuran overhead header paket, latensi pertukaran, streaming WebSocket | Kriteria: Analisis komparatif kinerja protokol; Teknik: Presentasi Benchmark | **Luring**: Kuliah Diskusi, Packet Sniffing Wireshark pada MQTT, CoAP, HTTP (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Review persiapan UTS di LMS | Protokol CoAP, HTTP REST vs CoAP vs MQTT, WebSocket Duplex [Hanes Bab 5, Al-Sarawi] | 5% |
| **8** | **UTS**: Evaluasi Tengah Semester (CPMK1, CPMK2) | Ketuntasan dan ketelitian merangkai sensor, memprogram bus, dan telemetri MQTT | Kriteria: Rubrik Ujian Tertulis & Live Coding (Skala 1-100); Teknik: Tes Tulis & Lab | **Ujian Terjadwal di Lab Komputer & Embedded Systems (150 Menit)**<br>**Daring**: Upload firmware & bukti telemetri di LMS | Seluruh Materi Perkuliahan Minggu 1 sampai Minggu 7 | **15%** |
| **9** | Sub-CPMK 8: Event-Driven Node-RED Flow Engine & UI Dashboard Otomasi `[C5]` | Flow data input MQTT, logic function node JavaScript, notifikasi Telegram, UI | Kriteria: Logika alur otomatisasi & kemudahan UI; Teknik: Tugas Node-RED | **Luring**: Workshop: Otomasi Kontrol Suhu Ruangan & Node-RED Dashboard di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Ekspor-impor flow JSON di LMS | Event-Driven Architecture, Node-RED Engine, Function Nodes, UI Dashboard [Lea Bab 6] | 5% |
| **10** | Sub-CPMK 9: Integrasi Cloud IoT ThingsBoard & Firebase Realtime Database `[C5]` | Device provisioning token, rule chain telemetri, remote RPC control aktuator | Kriteria: Integrasi awan & keandalan rule chain; Teknik: Portofolio Cloud IoT | **Luring**: Praktikum Konfigurasi ThingsBoard Cloud/Local Server & Widget Dashboard (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Akses server ThingsBoard di LMS | Cloud IoT Architecture, ThingsBoard Rule Engine, Firebase Realtime Database [Buyya Bab 6, Lea Bab 8] | 5% |
| **11** | Sub-CPMK 9: Database Time-Series InfluxDB & Visualisasi Grafana `[C5]` | Skema time-series (Bucket, Measurement, Tag, Field), query Flux, panel Grafana | Kriteria: Efisiensi penyimpanan data time-series; Teknik: Lembar Kerja Grafana | **Luring**: Workshop Lab: Integrasi Node-RED -> InfluxDB -> Grafana Server (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Diskusi optimasi retensi data di LMS | Time-Series Database (TSDB), InfluxDB Architecture, Grafana Dashboard [Lea Bab 8, Buyya Bab 7] | 5% |
| **12** | Sub-CPMK 10: Keamanan Komunikasi TLS/MQTTS, OTA Update, & Low-Power `[C4, C5]` | Enkripsi sertifikat TLS pada port 8883, token JWT, ArduinoOTA, deep sleep mode | Kriteria: Ketahanan keamanan data & update OTA; Teknik: Tugas Keamanan IoT | **Luring**: Praktik Pengamanan Komunikasi TLS/SSL dan Fitur ArduinoOTA ESP32 (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Checklist OWASP IoT Top 10 di LMS | Keamanan IoT, MQTTS/TLS, Token Auth, OWASP IoT Top 10, OTA Updates, Deep Sleep [Hanes Bab 10, Lea Bab 11] | 4% |
| **13** | Sub-CPMK 10: Edge Computing & Pengantar TinyML pada Mikrokontroler `[C4, C5]` | Pelatihan model klasifikasi sensor sederhana dan deployment model ke ESP32 | Kriteria: Akurasi model pada ESP32 berdaya rendah; Teknik: Lembar Kerja TinyML | **Luring**: Demonstrasi Ekstraksi Fitur & Deployment Model TinyML ke ESP32 (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Uji live inference Edge Impulse di LMS | Edge Computing, Konsep TinyML, Model Quantization INT8, TensorFlow Lite Micro [Warden & Situnayake Bab 1-3] | 4% |
| **14** | Sub-CPMK 11: Integrasi Purwarupa Produk Cerdas IoT Terpadu `[C5, C6]` | Integrasi perangkat keras, konektivitas nirkabel, middleware, dan cloud dashboard | Kriteria: Kematangan integrasi sistem & packaging; Teknik: Review Capstone 2 | **Luring**: Workshop Capstone: Troubleshooting, Packaging 3D Print / Box Akrilik (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Upload draf laporan teknis di LMS | Metodologi Rekayasa Produk IoT, Skematik Sirkuit, Packaging Enclosure [Lea Bab 12] | 5% |
| **15** | Sub-CPMK 11: Validasi Lapangan, Kalibrasi Sensor, & Presentasi Expo Tim `[A4, C6]` | Uji kondisi riil, kalibrasi sensor, pengujian baterai, live demo produk, tanya jawab | Kriteria: Rubrik Presentasi & Unjuk Kerja Alat; Teknik: Expo IoT Mahasiswa | **Luring**: Expo Pameran & Sidang Pleno Presentasi Proyek IoT, Live Demo Alat di Lab (PB: 3x50', PT: 3x60', BM: 3x60')<br>**Daring**: Unggah video demo alat di LMS | Komunikasi Profesional Rekayasa IoT, Dokumentasi Teknis GitHub & Wiring Diagram | 7% |
| **16** | **UAS**: Evaluasi Akhir Semester Berbasis Capstone Project IoT Terpadu | Purwarupa fisik berfungsi, transmisi telemetri stabil, naskah laporan IEEE lengkap | Kriteria: Rubrik Holistik Capstone IoT (Skala 1-100); Teknik: Penilaian Naskah & Portofolio | **Penyerahan Alat Fisik Terpadu, Naskah Laporan Akhir, & Sidang Evaluasi Akhir**<br>**Daring**: Final submission bundle di LMS UNIROW | Seluruh Bahan Kajian Teknologi Internet of Thing (Minggu 1 s.d. 15) | **15%** |
| **TOTAL** | | | | | | **100%** |

---

## VI. RANCANGAN TUGAS MAHASISWA & RUBRIK PENILAIAN OBE

### A. Rincian Tugas Terstruktur
1. **Tugas 1 (Minggu 3)**: Interfacing Multi-Sensor ESP32 & Serial/I2C Data Logging (Perancangan sirkuit sensor analog dan I2C BME280/OLED dengan kalibrasi data).
2. **Tugas 2 (Minggu 6)**: Rancang Bangun Sistem Telemetri MQTT Real-Time & Node-RED Flow (Koneksi Wi-Fi, publish payload JSON ke broker Mosquitto, dan notifikasi otomatis Telegram).
3. **Tugas 3 (Minggu 10–11)**: Integrasi Cloud IoT ThingsBoard, InfluxDB & Visualisasi Grafana (Penyimpanan telemetri time-series selama 3 hari pengamatan, rule chain, dan dashboard multi-panel).
4. **Tugas 4 (Minggu 12–15)**: Capstone Project: Rancang Bangun Produk Sistem Cerdas IoT Skala Industri/Masyarakat (Purwarupa fisik dengan packaging rapi, enkripsi MQTTS/TLS, cloud dashboard, laporan IEEE, dan repositori GitHub).

### B. Rubrik Penilaian OBE Skala 1–5

| Aspek Penilaian | Sangat Kurang (1) | Kurang (2) | Cukup (3) | Baik (4) | Sangat Baik (5) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Interfacing Hardware & Mikrokontroler (C3)** | Gagal membaca sensor, pengkabelan salah berisiko merusak komponen (`< 50`) | Sensor terbaca namun nilai tidak terkalibrasi dan sering hilang (`50-59`) | Interfacing sensor digital/analog berjalan dengan pembacaan cukup akurat (`60-69`) | Interfacing bus I2C/SPI sangat presisi, kalibrasi akurat dan cepat (`70-84`) | Skematik elektronik standar industri, efisiensi konsumsi daya teroptimasi (`85-100`) |
| **Implementasi Jaringan & Keamanan Telemetri (C4)** | Gagal menghubungkan mikrokontroler ke jaringan/broker (`< 50`) | Terhubung ke Wi-Fi tetapi payload tidak terformat & sering diskoneksi (`50-59`) | Protokol MQTT/HTTP berjalan normal dengan format JSON standar (`60-69`) | Protokol MQTT sangat stabil dengan hirarki topik rapi dan QoS tepat (`70-84`) | Arsitektur komunikasi andal, menerapkan enkripsi MQTTS/TLS, token auth & OTA (`85-100`) |
| **Integrasi Cloud IoT, Middleware & UI (C5-C6)** | Data sensor tidak tersimpan di cloud tanpa visualisasi (`< 50`) | Data masuk ke cloud tetapi tampilan dashboard rusak tanpa otomatisasi (`50-59`) | Dashboard ThingsBoard/Node-RED menampilkan data real-time standar (`60-69`) | Dashboard informatif, rule engine notifikasi aktif, kontrol dua arah berjalan (`70-84`) | Sistem cloud tingkat enterprise (InfluxDB + Grafana + ThingsBoard) memukau (`85-100`) |
| **Inovasi Capstone & Presentasi Tim (A4, C6)** | Purwarupa tidak berbentuk, laporan tidak selesai, tim pasif (`< 50`) | Purwarupa rapuh tanpa packaging, laporan kurang rapi (`50-59`) | Purwarupa berfungsi baik dalam kemasan standar, presentasi lancar (`60-69`) | Nilai guna tinggi bagi mitra, kemasan rapi 3D print/akrilik, presentasi meyakinkan (`70-84`) | Inovasi luar biasa siap hilirisasi/paten, repo GitHub standar open-source global (`85-100`) |

---

## VII. LEMBAR PENGESAHAN RPS

| Dosen Pengembang RPS | Koordinator Rumpun Mata Kuliah (RMK) | Ketua Program Studi S1 Informatika |
| :---: | :---: | :---: |
| <br><br>**Fitroh Amaluddin, M.Kom.**<br>NIDN: 07xxxxxxxx | <br><br>**Fitroh Amaluddin, M.Kom.**<br>NIDN: 07xxxxxxxx | <br><br>**AMALUDIN ARIFIA, M.Kom.**<br>NIDN: 07xxxxxxxx |
