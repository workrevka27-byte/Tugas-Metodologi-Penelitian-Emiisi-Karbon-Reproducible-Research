# TUGAS METODOLOGI PENELITIAN (LATIHAN DENGAN R STUDIO)

# 🚗 Carbon Emission Reproducible Research

Analisis **Emisi Karbon Kendaraan Bermotor** menggunakan metode **Vehicle Kilometers Travelled (VKT)** dan **R Programming** sebagai implementasi konsep **Reproducible Research** pada mata kuliah **Metodologi Penelitian**.

---

# 📖 Deskripsi

Repository ini berisi tahapan analisis data volume kendaraan untuk menghitung **emisi karbon kendaraan bermotor** menggunakan pendekatan **Vehicle Kilometers Travelled (VKT)**.

Tahapan analisis meliputi proses **import data**, **data preparation**, **perhitungan VKT**, **perhitungan emisi karbon**, **analisis statistik**, **visualisasi hasil**, hingga **dokumentasi lingkungan komputasi** sehingga seluruh proses penelitian dapat direproduksi kembali.

Seluruh analisis dilakukan menggunakan bahasa pemrograman **R**, sehingga setiap proses dapat dijalankan kembali hanya dengan menggunakan data mentah dan script yang tersedia.

---

# 🎯 Tujuan

- Mengimpor data volume kendaraan.
- Memeriksa kualitas data.
- Membersihkan data (Data Cleaning).
- Menghitung **Vehicle Kilometers Travelled (VKT)**.
- Menghitung emisi karbon kendaraan.
- Melakukan analisis statistik deskriptif.
- Menganalisis emisi berdasarkan ruas jalan.
- Menganalisis emisi berdasarkan jenis kendaraan.
- Membuat visualisasi hasil analisis.
- Menerapkan konsep **Reproducible Research** menggunakan R.

---

# 📁 Struktur Repository

```text
Carbon-Emission-Reproducible-Research
│
├── data/
│   └── data_emisi.csv
│
├── notebook/
│   ├── 01_import_data.ipynb
│   ├── 02_perhitungan_emisi.ipynb
│   ├── 03_analisis_visualisasi.ipynb
│   └── 04_export_output.ipynb
│
├── output/
│   ├── data_clean.csv
│   ├── hasil_emisi.csv
│   ├── ringkasan_ruas.csv
│   ├── ringkasan_kendaraan.csv
│   ├── ringkasan_penelitian.xlsx
│   ├── grafik_emisi_ruas.png
│   ├── grafik_emisi_kendaraan.png
│   ├── grafik_kontribusi_ruas.png
│   ├── package_version.csv
│   ├── sessionInfo_01.txt
│   ├── sessionInfo_02.txt
│   ├── sessionInfo_03.txt
│   └── sessionInfo_04.txt
│
├── report/
│
└── README.md
```

---

# 💻 Software

Project ini dibuat menggunakan:

- R
- RStudio
- Jupyter Notebook (IRkernel)

---

# 📦 Packages

Project ini menggunakan package berikut:

- readr
- dplyr
- ggplot2
- writexl

Install package dengan:

```r
install.packages(c(
  "readr",
  "dplyr",
  "ggplot2",
  "writexl"
))
```

---

# ▶️ Alur Analisis

Jalankan notebook secara berurutan.

| No | Notebook | Fungsi |
|:--:|----------|--------|
| 01 | Import Data | Mengimpor data, memeriksa kualitas data, dan menghasilkan dataset bersih |
| 02 | Perhitungan Emisi | Menghitung Vehicle Kilometers Travelled (VKT) dan emisi karbon kendaraan |
| 03 | Analisis Statistik & Visualisasi | Melakukan analisis statistik deskriptif dan visualisasi hasil |
| 04 | Export Output | Mengekspor hasil penelitian dan mendokumentasikan lingkungan komputasi |

---

# 🧮 Metode Perhitungan

## Vehicle Kilometers Travelled (VKT)

\[
VKT = Volume \times Panjang\ Jalan
\]

dimana:

- **Volume** = jumlah kendaraan (kendaraan/jam)
- **Panjang Jalan** = panjang ruas jalan (km)

---

## Emisi Karbon

\[
Emisi = VKT \times Faktor\ Emisi
\]

dimana:

- **VKT** = Vehicle Kilometers Travelled (kendaraan-km)
- **Faktor Emisi** = faktor emisi kendaraan (gram CO₂/kendaraan-km)

---

## Konversi Satuan

Gram → Kilogram

\[
Kilogram = \frac{Gram}{1000}
\]

Kilogram → Ton

\[
Ton = \frac{Kilogram}{1000}
\]

---

# 📊 Hasil Analisis

Analisis menghasilkan informasi mengenai:

- Total Vehicle Kilometers Travelled (VKT).
- Total emisi karbon kendaraan.
- Emisi karbon pada setiap ruas jalan.
- Emisi karbon berdasarkan jenis kendaraan.
- Persentase kontribusi emisi tiap ruas jalan.
- Grafik distribusi emisi karbon.

---

# 📈 Output

Program menghasilkan beberapa file output, yaitu:

- `data_clean.csv`
- `hasil_emisi.csv`
- `ringkasan_ruas.csv`
- `ringkasan_kendaraan.csv`
- `ringkasan_penelitian.xlsx`
- `grafik_emisi_ruas.png`
- `grafik_emisi_kendaraan.png`
- `grafik_kontribusi_ruas.png`
- `package_version.csv`
- `sessionInfo_01.txt`
- `sessionInfo_02.txt`
- `sessionInfo_03.txt`
- `sessionInfo_04.txt`

---

# 🔄 Workflow

```text
Data Volume Kendaraan
          │
          ▼
 Import Data
          │
          ▼
 Data Cleaning
          │
          ▼
 Perhitungan VKT
          │
          ▼
 Perhitungan Emisi Karbon
          │
          ▼
 Analisis Statistik
          │
          ▼
 Analisis Berdasarkan
 Ruas Jalan &
 Jenis Kendaraan
          │
          ▼
 Visualisasi
          │
          ▼
 Export Output
          │
          ▼
 Dokumentasi
 Reproducible Research
```

---

# 🔁 Prinsip Reproducible Research

Repository ini menerapkan prinsip **Reproducible Research**, yaitu:

- Data mentah disimpan pada folder `data`.
- Seluruh analisis dilakukan menggunakan script R.
- Setiap tahapan analisis dipisahkan ke dalam notebook sesuai fungsi.
- Seluruh output dihasilkan secara otomatis melalui script.
- Informasi versi package dan lingkungan komputasi disimpan menggunakan `sessionInfo()`.
- Analisis dapat direproduksi kembali menggunakan data dan script yang tersedia.

---

# 🚀 Cara Menjalankan

1. Clone repository ini.

2. Letakkan file **data_emisi.csv** ke dalam folder **data/**.

3. Jalankan notebook secara berurutan:

```
01_import_data.ipynb

↓

02_perhitungan_emisi.ipynb

↓

03_analisis_visualisasi.ipynb

↓

04_export_output.ipynb
```

4. Seluruh hasil analisis akan tersimpan otomatis pada folder **output/**.

---

# 👨‍💻 Penulis

**Revka Saputro**

Program Studi Teknik Sipil dan Lingkungan

Sekolah Pascasarjana

IPB University

---

# 📚 Mata Kuliah

**Metodologi Penelitian**

---

# 📄 Lisensi

Repository ini dibuat untuk keperluan akademik sebagai tugas mata kuliah **Metodologi Penelitian**.

Data dan script yang tersedia hanya digunakan untuk kepentingan pembelajaran, penelitian, dan implementasi konsep **Reproducible Research**.
