# Analisis

- **Packages mengorganisir kode lebih baik daripada file tunggal**
- **Instalasi mode pengembangan memungkinkan iterasi cepat**
- **Struktur package mengikuti konvensi Python**
- **Memisahkan aplikasi dari konfigurasi**

## Jawaban Extra Credit

### Tanpa __init__.py:

- **Direktori tidak dikenali sebagai package**
- **Import gagal**
- **Namespace packages memungkinkan tetapi eksplisit lebih baik**

### Isi __init__.py:

- **Dapat berisi kode inisialisasi**
- **Sering menyimpan import tingkat package**
- **Dieksekusi saat package diimpor**

### Manfaat setup.py:

- **Mengelola dependensi**
- **Memungkinkan instalasi yang dapat direproduksi**
- **Mengikuti standar profesional**

### Perbedaan mode instalasi:

- **Regular menyalin file**
- **Editable membuat link**
- **Pengembangan membutuhkan editable**