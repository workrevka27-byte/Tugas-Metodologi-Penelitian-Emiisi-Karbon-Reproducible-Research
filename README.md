TUGAS METODOLOGI (LATIHAN DENGAN R STUDIO)

🌧️ Emisi Karbon Reproducible Research
Analisis Emisi Karbon kendaraan menggunakan R Programming sebagai implementasi konsep Reproducible Research pada mata kuliah Metodologi Penelitian.

📖 Deskripsi
Repository ini berisi tahapan analisis data curah hujan harian menjadi curah hujan maksimum tahunan (Rmax), kemudian dilakukan analisis statistik deskriptif, analisis distribusi probabilitas, pengujian kesesuaian distribusi, hingga perhitungan curah hujan rencana.

Seluruh analisis dilakukan menggunakan bahasa pemrograman R sehingga setiap proses dapat direproduksi kembali hanya dengan menjalankan script yang tersedia.

🎯 Tujuan
Mengolah data curah hujan harian.
Membentuk data curah hujan maksimum tahunan (Rmax).
Menghitung statistik deskriptif.
Menentukan CDF empiris.
Membandingkan beberapa distribusi probabilitas.
Menentukan distribusi terbaik.
Melakukan uji Chi-Square.
Melakukan uji Kolmogorov-Smirnov.
Menghitung curah hujan rencana untuk berbagai periode ulang.
📁 Struktur Repository
Rainfall-Reproducible-Research
│
├── data/
│   └── Curah Hujan.csv
│
├── script/
│   ├── 01_import_dan_rmax.R
│   ├── 02_statistik_deskriptif.R
│   ├── 03_cdf_empiris.R
│   ├── 04_distribusi_normal.R
│   ├── 05_perbandingan_distribusi.R
│   ├── 06_uji_chisquare.R
│   ├── 07_uji_smirnov.R
│   ├── 08_curah_hujan_rencana.R
│   └── 09_plot_distribusi.R
│
├── output/
│
├── report/
│
└── README.md
💻 Software
R
RStudio
📦 Packages
Project ini menggunakan package berikut:

readr
dplyr
lubridate
ggplot2
e1071
fitdistrplus
writexl
Install package dengan:

install.packages(c(
"readr",
"dplyr",
"lubridate",
"ggplot2",
"e1071",
"fitdistrplus",
"writexl"
))
▶️ Alur Analisis
Jalankan script secara berurutan.

No	Script	Fungsi
01	Import Data dan Rmax	Mengimpor data serta membentuk curah hujan maksimum tahunan
02	Statistik Deskriptif	Menghitung statistik dasar data Rmax
03	CDF Empiris	Menghitung peluang empiris menggunakan plotting position
04	Distribusi Normal	Menghitung probabilitas teoritis distribusi Normal
05	Perbandingan Distribusi	Membandingkan Normal, Log Normal, Gumbel, dan Weibull
06	Uji Chi-Square	Menguji kesesuaian distribusi terbaik
07	Uji Kolmogorov-Smirnov	Validasi distribusi terbaik
08	Curah Hujan Rencana	Menghitung hujan rencana berbagai periode ulang
09	Visualisasi	Membuat grafik distribusi
📊 Hasil Analisis
Analisis menunjukkan bahwa beberapa distribusi probabilitas dibandingkan menggunakan nilai SSE dan koefisien determinasi (R²).

Distribusi terbaik kemudian diuji menggunakan:

Chi-Square Test
Kolmogorov-Smirnov Test
Distribusi yang memenuhi kedua pengujian digunakan untuk menghitung curah hujan rencana.

📈 Output
Program menghasilkan beberapa file output, antara lain:

rmax_tahunan.csv
statistik_deskriptif.csv
cdf_empiris.csv
hasil_r2.csv
hasil_chisquare.csv
hasil_smirnov.csv
curah_hujan_rencana.csv
plot_distribusi.png
🔄 Workflow
Data Curah Hujan Harian
            │
            ▼
Import Data
            │
            ▼
Curah Hujan Maksimum Tahunan (Rmax)
            │
            ▼
Statistik Deskriptif
            │
            ▼
CDF Empiris
            │
            ▼
Analisis Distribusi
(Normal, Log Normal,
 Gumbel, Weibull)
            │
            ▼
Perbandingan Distribusi
            │
            ▼
Distribusi Terbaik
            │
      ┌─────┴─────┐
      ▼           ▼
Chi-Square      Kolmogorov
      │           │
      └─────┬─────┘
            ▼
Curah Hujan Rencana
            │
            ▼
Visualisasi
👨‍💻 Penulis
Fayyad Faizatama

Program Studi Teknik Sipil

Universitas ...

📚 Mata Kuliah
Metodologi Penelitian

📄 Lisensi
Repository ini dibuat untuk keperluan akademik sebagai tugas mata kuliah Metodologi Penelitian.