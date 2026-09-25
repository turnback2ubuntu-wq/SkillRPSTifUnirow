# Skill Generator RPS Berbasis OBE — Prodi S1 Informatika UNIROW

Repositori ini berisi **Skill AI Agent** (`rps-obe-generator`), modul otomasi, serta kumpulan dokumen **Rencana Pembelajaran Semester (RPS)** berbasis **Outcome-Based Education (OBE)** untuk Program Studi S1 Informatika, Fakultas Sains dan Teknologi, **Universitas PGRI Ronggolawe (UNIROW) Tuban**.

Pengembangan RPS ini mengacu pada:
1. **Buku Kurikulum Prodi S1 Informatika atau Ilmu Komputer Versi 2.0 (APTIKOM, CS2024 / KKNI Level 6)**.
2. **Format Dokumen Resmi RPS UNIROW** (Tabel Identitas, Matriks CPL-CPMK-SubCPMK, Matriks 16 Pertemuan, Rancangan Tugas Terstruktur, Rubrik Penilaian Skala 1–5, dan Lembar Pengesahan).
3. **Buku Saku Penyusunan RPS Berbasis OBE dengan Modul Prompt Engineering untuk Dosen** (Alur 6 Langkah Penyusunan).

---

## 📂 Struktur Repositori

```text
├── .agents/
│   └── skills/
│       └── rps-obe-generator/           # Folder Skill Utama untuk AI Agent
│           ├── SKILL.md                 # Definisi instruksi dan SOP penyusunan RPS
│           ├── scripts/
│           │   └── generate_rps_docx.py # Engine injeksi data JSON ke Format Word (.docx)
│           ├── references/              # Buku acuan, KKO Bloom, Panduan Format & Prompts
│           │   ├── aptikom_curriculum_cs2024.md
│           │   ├── bloom_taxonomy_kko.md
│           │   ├── prompts_step_by_step.md
│           │   ├── assessment_rubric_scale5.md
│           │   └── unirow_rps_template_guide.md
│           └── examples/                # Contoh acuan RPS OBE standar
├── Buku_Saku_RPS_OBE.docx               # Panduan modul prompt engineering dosen
├── Buku Kurikulum ... aptikom.pdf       # Standar Kurikulum APTIKOM Versi 2.0
├── Format RPS UNIROW.docx               # Template master resmi UNIROW
│
├── RPS_IF260624_Sistem_Informasi_Bisnis.*    (JSON, MD, DOCX)
├── RPS_IF440524_Basis_Data_Lanjut.*          (JSON, MD, DOCX)
├── RPS_IF640424_Statistik_Teknik.*           (JSON, MD, DOCX)
└── RPS_IF6802_Analisa_Data_Multivariat.*     (JSON, MD, DOCX)
```

---

## 🎯 6 Langkah Metodologi Penyusunan RPS (Buku Saku OBE)

1. **Langkah 1**: Perumusan CPL dan CPMK berbasis Kurikulum APTIKOM 2.0 dan Taksonomi Bloom (KKO C2-C6). Bobot kontribusi CPMK ke CPL berjumlah 100%.
2. **Langkah 2**: Perumusan Sub-CPMK dengan formula ABCD (*Audience, Behavior, Condition, Degree*) serta penentuan bobot asesmen tiap Sub-CPMK (Total 100%).
3. **Langkah 3**: Integrasi Bahan Kajian & Pustaka Terkini (Pustaka Utama dan Pendukung bereputasi).
4. **Langkah 4**: Penyusunan Matriks Pembelajaran 16 Pertemuan (Pertemuan 8 UTS, Pertemuan 16 UAS, alokasi waktu 150 menit Tatap Muka + 180 menit Tugas Terstruktur/Mandiri per minggu untuk 3 SKS sesuai SN-Dikti).
5. **Langkah 5**: Perancangan Tugas Terstruktur Mahasiswa & Rubrik Penilaian OBE Skala 1–5 (Sangat Kurang, Kurang, Cukup, Baik, Sangat Baik).
6. **Langkah 6**: Integrasi ke Dokumen Resmi UNIROW dan Pengesahan (Dosen Pengembang, Koordinator RMK, dan Ketua Program Studi).

---

## 📚 Dokumen RPS yang Telah Selesai Disusun

| Kode MK | Nama Mata Kuliah | Bobot SKS | Dosen Pengembang | Format Tersedia |
| :--- | :--- | :---: | :--- | :---: |
| **IF260624** | Sistem Informasi Bisnis | 3 SKS | Andy Haryoko, S.T., M.T. | `.json`, `.md`, `.docx` |
| **IF440524** | Basis Data Lanjut | 3 SKS | Andy Haryoko, S.T., M.T. | `.json`, `.md`, `.docx` |
| **IF640424** | Statistik Teknik | 3 SKS | Andy Haryoko, S.T., M.T. | `.json`, `.md`, `.docx` |
| **IF6802** | Analisa Data Multivariat | 3 SKS | Andy Haryoko, S.T., M.T. | `.json`, `.md`, `.docx` |

---

## ⚙️ Cara Menggunakan Generator Otomatis DOCX

Pastikan `python3` dan `python-docx` sudah terinstal:

```bash
pip install python-docx
```

Jalankan script generator dengan menyertakan file data JSON mata kuliah:

```bash
python3 .agents/skills/rps-obe-generator/scripts/generate_rps_docx.py \
  --input RPS_IF6802_Analisa_Data_Multivariat.json \
  --output RPS_IF6802_Analisa_Data_Multivariat_UNIROW.docx
```

---

## 👨‍🏫 Dosen Pengembang & Pimpinan Prodi

- **Dosen Pengembang / Pengampu**: Andy Haryoko, S.T., M.T.
- **Ketua Program Studi S1 Informatika**: AMALUDIN ARIFIA, M.Kom.
- **Institusi**: Program Studi S1 Informatika, Fakultas Sains dan Teknologi, Universitas PGRI Ronggolawe (UNIROW) Tuban
