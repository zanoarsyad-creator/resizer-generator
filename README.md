# 📷 Foto Resizer Generator

**Foto Resizer Generator** adalah aplikasi desktop modern berbasis Python dan **CustomTkinter** yang dirancang untuk mengubah ukuran foto ke standar pasfoto (2x3, 3x4, 4x6 cm) secara otomatis, cepat, dan presisi.

Aplikasi ini mendukung pemrosesan banyak foto sekaligus (*batch processing*), penyesuaian resolusi DPI cetak, serta fitur pemotongan pintar berbasis pemprosesan latar belakang (*multithreading*) agar antarmuka tetap responsif.

---

## ✨ Fitur Utama

- 📐 **Ukuran Pasfoto Standar**: Mendukung preset pasfoto **2x3 cm**, **3x4 cm**, dan **4x6 cm**.
- 🖨️ **Kustomisasi DPI**: Atur resolusi cetak sesuai kebutuhan (default: **300 DPI** untuk kualitas cetak optimal).
- 📁 **Pemrosesan Massal (Batch Processing)**: Pilih file foto secara acak (multi-select) atau impor seluruh foto langsung dari satu folder.
- ✂️ **Smart Crop & Auto Orientation**: Menggunakan algoritma *Lanczos Resampling* & `ImageOps.fit` untuk pemotongan presisi tanpa membuat foto gepeng/distorsi, serta mempertahankan orientasi EXIF foto.
- ⚡ **Ringan & Responsif**: Berjalan di atas antrean *multithreading* sehingga UI tidak membeku saat memproses ratusan gambar.
- 🎨 **Antarmuka Modern (Dark Mode)**: Tampilan visual elegan menggunakan GUI CustomTkinter.
- 🧹 **Manajemen Memori & Cache**: Pembersihan berkas sementara (*tempdir*) dan pengumpulan sampah memori secara otomatis setelah proses pemrosesan selesai.

---

## 🛠️ Persyaratan Sistem

- **Python 3.8+**
- Dependensi Python:
  - `customtkinter`
  - `Pillow` (PIL)
