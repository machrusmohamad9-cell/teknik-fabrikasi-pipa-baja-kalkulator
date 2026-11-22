# Panduan Teknik Fabrikasi Pipa Baja, Rumus Bentangan & Kalkulator Engineering (ASME / SNI)

[![Portal Teknik Machrus Notes](https://img.shields.io/badge/Portal%20Resmi-MachrusNotes.com-0f4c81?style=for-the-badge)](https://www.machrusnotes.com/)
[![Kalkulator Fabrikasi](https://img.shields.io/badge/Kalkulator%20Online-Fabrikasi%20%26%20Berat%20Baja-16a34a?style=for-the-badge)](https://www.machrusnotes.com/kalkulator-fabrikasi-baja/)

Repositori referensi terbuka oleh **[Machrus Notes](https://www.machrusnotes.com/)** untuk *pipe fitter*, *steel fabricator*, *drafter* AutoCAD, *welding inspector*, dan *estimator* konstruksi industri di Indonesia. Dokumentasi ini merangkum rumus inti fabrikasi perpipaan (ASME B31.3 / B36.10M / B16.5), perhitungan berat profil baja (SNI / JIS), serta tautan langsung menuju kalkulator teknik online gratis.

---

## 1. Rumus Inti Fabrikasi Pipa & Perpipaan Industri

### A. Mitered Elbow Cut-Back Formula (Segmented Bend)
Untuk menghitung tinggi potong ordinat (*cut-back*) pada pembuatan *mitered elbow* multi-segmen:

```text
θ = α / (2 × N)
h(φ) = [ R - (D / 2) × cos(φ) ] × tan(θ)
C = r × tan(θ)
```

- **α**: Sudut total belokan elbow (derajat, mis. 90°, 60°, 45°)
- **N**: Jumlah pengelasan / bidang potong miter
- **R**: Radius kelengkungan garis tengah (*centerline radius*)
- **D, r**: Diameter luar pipa (*OD*) dan jari-jari luar pipa (`D / 2`)
- **φ**: Sudut pembagian keliling pipa (`0°` hingga `360°`)

### B. Eccentric Reducer 3D Triangulation (Bentangan Kerucut Miring)
Pada pembuatan *eccentric reducer* dari plat roll, panjang garis elemen sejati (*true length* $L_n$) antar titik keliling lingkaran besar ($R_1$) dan kecil ($R_2$) dengan tinggi aksial $H$ dan eksentrisitas $e = R_1 - R_2$:

```text
x1 = R1 × cos(φ),   y1 = R1 × sin(φ)
x2 = e + R2 × cos(φ), y2 = R2 × sin(φ)
L_true = sqrt( (x1 - x2)^2 + (y1 - y2)^2 + H^2 )
```

### C. Berat Pipa Baja per Meter (ASME B36.10M / API 5L)
Menggunakan massa jenis baja karbon standar $\rho = 7.850\text{ kg/m}^3$:

```text
W (kg/m) = 0.0246615 × (OD - t) × t
```

- **OD**: Diameter luar pipa (mm)
- **t**: Ketebalan dinding pipa / *wall thickness* (mm)

### D. 45° Rolling Offset Piping
Untuk menghitung panjang pipa miring (*travel*) pada *rolling offset* 3D dengan jarak vertikal ($V$), horizontal ($H$), dan maju ($R$):

```text
True Offset = sqrt(V^2 + H^2)
Travel (45°) = True Offset × 1.4142
```

### E. Tebal Dinding Pipa Minimum (ASME B31.3 — Rumus Barlow)

```text
t_m = [ P × D / (2 × (S × E × W + P × Y)) ] + c
```

- **P**: Tekanan desain internal, **D**: Diameter luar pipa, **S**: Tegangan izin material (*allowable stress*), **E**: Faktor kualitas sambungan, **W**: *Weld joint strength reduction factor*, **Y**: Koefisien temperatur, **c**: *Corrosion & mechanical allowance*.

---

## 2. Suite Kalkulator Fabrikasi & Berat Baja Online (Gratis)

Gunakan kalkulator interaktif berbasis web di **[Machrus Notes](https://www.machrusnotes.com/)** langsung dari browser laptop maupun HP lapangan:

| Kategori | Nama Kalkulator | Tautan Langsung |
| :--- | :--- | :--- |
| **Hub Fabrikasi** | **Kalkulator Fabrikasi Baja Online (Hub)** | [Buka Hub Fabrikasi](https://www.machrusnotes.com/kalkulator-fabrikasi-baja/) |
| **Layout Pipa** | **Kalkulator Elbow Pipa (Segmented Bend)** | [Hitung Mitered Elbow](https://www.machrusnotes.com/kalkulator-fabrikasi-baja/kalkulator-elbow-pipa-segmented-bend/) |
| **Layout Plat** | **Kalkulator Fabrikasi Reducer (Concentric Flat Pattern)** | [Hitung Bentangan Reducer](https://www.machrusnotes.com/kalkulator-fabrikasi-baja/kalkulator-fabrikasi-reducer-flat-pattern/) |
| **Cabang Pipa** | **Kalkulator Y Simetris (Model Celana / True Wye)** | [Hitung Pola Y-Pipa](https://www.machrusnotes.com/kalkulator-fabrikasi-baja/kalkulator-y-simetris-model-celana/) |
| **Hub Berat Baja** | **Kalkulator Hitung Berat Baja Online (Hub)** | [Buka Hub Berat Baja](https://www.machrusnotes.com/kalkulator-hitung-berat-baja/) |
| **Profil Struktur** | **Kalkulator Berat Baja IWF** | [Hitung Berat IWF](https://www.machrusnotes.com/kalkulator-hitung-berat-baja/kalkulator-hitung-berat-baja-iwf/) |
| **Profil Struktur** | **Kalkulator Berat Baja H-Beam** | [Hitung Berat H-Beam](https://www.machrusnotes.com/kalkulator-hitung-berat-baja/kalkulator-hitung-berat-baja-h-beam/) |
| **Material Plat** | **Kalkulator Hitung Berat Plat Baja (Plate)** | [Hitung Berat Plat](https://www.machrusnotes.com/kalkulator-hitung-berat-baja/kalkulator-hitung-berat-plate/) |
| **Profil Siku** | **Kalkulator Berat Baja Siku (Angle Bar)** | [Hitung Berat Besi Siku](https://www.machrusnotes.com/kalkulator-hitung-berat-baja-siku-angle-bar/) |

---

## 3. Indeks Lengkap Panduan Teknik Fabrikasi Pipa, Pengelasan & AutoCAD

### Panduan Utama (Pillar Guide)
- **[Panduan Lengkap Teknik Fabrikasi Pipa Baja: Rumus Layout, Bentangan & Standar Industri](https://www.machrusnotes.com/panduan-teknik-fabrikasi-pipa-baja/)**

### Layout, Bentangan & Geometri Fabrikasi Pipa
1. [Rumus & Cara Layout Mitered Elbow Pipa Multi-Segmen](https://www.machrusnotes.com/rumus-layout-mitered-elbow-pipa/)
2. [Rumus & Cara Membuat Bentangan Eccentric Reducer Pipa](https://www.machrusnotes.com/cara-membuat-eccentric-reducer-pipa/)
3. [Rumus & Cara Membuat Bentangan Cabang Pipa (Y-Branch Model Celana & Tee 90°/45°)](https://www.machrusnotes.com/rumus-bentangan-cabang-pipa-y-branch-tee/)
4. [Rumus Bentangan Kerucut Terpancung & Hopper Plat Baja (Cone Flat Pattern)](https://www.machrusnotes.com/rumus-bentangan-kerucut-terpancung-plat-baja/)
5. [Rumus Offset Pipa 45° & Rolling Offset 3D untuk Pipe Fitter](https://www.machrusnotes.com/rumus-offset-pipa-45-derajat-rolling-offset/)

### Tabel Standar Pipa, Flange, Material & Berat Baja (ASME / SNI)
6. [Tabel Ukuran Pipa Baja ASME B36.10M & B36.19M Lengkap (NPS, OD, Schedule 10–160)](https://www.machrusnotes.com/tabel-ukuran-pipa-baja-asme-b36-10m-schedule/)
7. [Tabel Ukuran Flange Pipa ASME B16.5 Class 150 & Class 300 Lengkap](https://www.machrusnotes.com/tabel-ukuran-flange-pipa-asme-b16-5-class-150-300/)
8. [Panduan Pemilihan Material Pipa Baja Industri (ASTM A106 Gr.B, A53, API 5L, SS304/316L)](https://www.machrusnotes.com/panduan-material-pipa-baja-astm-a106-api-5l-ss316/)
9. [Jenis Pipe Support & Tabel Jarak Tumpuan Pipa Maksimum (Pipe Span ASME B31.3)](https://www.machrusnotes.com/jenis-pipe-support-tabel-jarak-tumpuan-pipa-asme/)
10. [Tabel Berat Besi Baja Lengkap: IWF, H-Beam, Plat Baja & Besi Siku (SNI/JIS)](https://www.machrusnotes.com/tabel-berat-besi-baja-iwf-hbeam-plat-siku/)
11. [Tabel Berat Besi Kanal UNP & CNP Standar SNI/JIS (6 Meter) Beserta Rumus Hitungnya](https://www.machrusnotes.com/tabel-berat-besi-kanal-unp-cnp-standar-sni/)
12. [Tabel Berat Besi Hollow (RHS/SHS) & Besi Beton Polos/Ulir Standar SNI](https://www.machrusnotes.com/tabel-berat-besi-hollow-besi-beton-sni-rumus/)
13. [Analisis Komprehensif Teknologi Katup Industri (Valve Classification & Material)](https://www.machrusnotes.com/analisis-komprehensif-teknologi-katup-industri/)

### Pengelasan (Welding), Fit-Up, NDT & Hydrotest (ASME IX & B31.3)
14. [Standar Bevel Pipa ASME B31.3, Fit-Up, Root Gap & Inspeksi NDT Las](https://www.machrusnotes.com/standar-bevel-pipa-asme-b31-3-fit-up-ndt-las/)
15. [Posisi Pengelasan Pipa 1G, 2G, 5G & 6G serta Cara Membaca WPS (ASME Section IX)](https://www.machrusnotes.com/posisi-pengelasan-pipa-1g-2g-5g-6g-wps-asme/)
16. [Rumus Menghitung Kebutuhan Kawat Las SMAW & GTAW (Consumable Estimation)](https://www.machrusnotes.com/rumus-menghitung-kebutuhan-kawat-las-smaw-gtaw/)
17. [10 Jenis Cacat Las Pipa Baja, Penyebab & Kriteria Penerimaan ASME B31.3](https://www.machrusnotes.com/jenis-cacat-las-pipa-baja-penyebab-kriteria-asme/)
18. [Prosedur Hydrotest & Pneumatic Test Pipa Industri Standar ASME B31.3](https://www.machrusnotes.com/prosedur-hydrotest-pipa-industri-asme-b31-3/)

### AutoCAD, Gambar Isometrik, Spool Drawing & P&ID
19. [Cara Menggambar Layout & Bentangan Pipa di AutoCAD untuk Fabrikasi](https://www.machrusnotes.com/cara-menggambar-layout-bentangan-pipa-autocad/)
20. [Cara Membaca Gambar Isometric Piping & Simbol Fitting Industri](https://www.machrusnotes.com/cara-membaca-gambar-isometric-piping-simbol/)
21. [Cara Membuat Gambar Spool Pipa (Isometric Spool Drawing) & Weld Map di AutoCAD](https://www.machrusnotes.com/cara-membuat-gambar-spool-pipa-weld-map-autocad/)
22. [Cara Membaca Gambar P&ID (Piping and Instrumentation Diagram) & Simbol ISA 5.1](https://www.machrusnotes.com/cara-membaca-gambar-pid-simbol-perpipaan/)
23. [Daftar Lengkap Shortcut & Perintah AutoCAD 2D/3D untuk Drafter Piping & Baja](https://www.machrusnotes.com/daftar-shortcut-perintah-autocad-2d-3d-drafter/)

---

## Portal & Kontak Resmi
- **Website Utama**: [https://www.machrusnotes.com/](https://www.machrusnotes.com/)
- **Kategori Piping & Fabrikasi**: [https://www.machrusnotes.com/category/piping/](https://www.machrusnotes.com/category/piping/)
- **Tentang Penulis**: [https://www.machrusnotes.com/tentang/](https://www.machrusnotes.com/tentang/)
