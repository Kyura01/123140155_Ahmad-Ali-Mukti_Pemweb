# Analisis: Unit Tests dan pytest

## Analisis

- **Unit tests memverifikasi komponen individual secara terisolasi**
- **Komunitas Pyramid lebih menyukai pytest karena fitur-fitur canggihnya**
- **Organisasi dan struktur test penting untuk maintainability**

## Jawaban Extra Credit

### Mengapa kita perlu menambahkan pytest sebagai development dependency?

- **Pytest tidak termasuk dalam standard library, jadi harus ditambahkan sebagai dependency**
- **Menyediakan pengalaman testing yang lebih baik dengan fitur seperti fixtures dan plugins**
- **Menambahkannya ke dev_requires memastikan tersedia di development tapi tidak di production**

### Apa tujuan direktori `tests` dalam package?

- **Berisi unit tests untuk aplikasi**
- **Diorganisir berdasarkan modul atau fitur yang ditest**
- **Membantu memastikan kualitas kode dan menangkap regresi**

### Bagaimana cara menjalankan tests untuk aplikasi?

- **Gunakan perintah `pytest` di terminal**
- **Dapat menentukan opsi seperti `--cov` untuk laporan coverage**
- **Terintegrasi dengan CI/CD pipelines untuk automated testing**

### Apa signifikansi file `__init__.py` dalam direktori tests?

- **Menandai direktori sebagai Python package**
- **Memungkinkan relative imports dalam modul test**
- **Dapat kosong atau berisi fixtures dan imports tingkat package**

### Bagaimana cara mentest skenario berbeda untuk fungsi view?

- **Gunakan parameter request atau headers yang berbeda dalam tests**
- **Mock dependencies atau services yang digunakan oleh view**
- **Assert pada status response, headers, dan konten body**