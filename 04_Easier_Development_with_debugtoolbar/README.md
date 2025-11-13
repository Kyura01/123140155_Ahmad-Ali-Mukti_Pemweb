# Analisis: Pengembangan Lebih Mudah dengan Debug Toolbar

## Analisis

- **Debug toolbar memberikan wawasan tentang request, response, dan performa**
- **Terintegrasi dengan Pyramid melalui konfigurasi**
- **Setuptools extras digunakan untuk dependensi opsional**

## Jawaban Extra Credit

### Apa tujuan `dev_requires` dalam setup.py?

- **Mendaftar dependensi pengembangan, seperti pyramid_debugtoolbar dan pytest**
- **Diinstall dengan `pip install -e ".[dev]"`**
- **Menjaga lingkungan produksi tetap bersih**

### Bagaimana menginstall package dengan extras menggunakan pip?

- **Gunakan sintaks `pip install -e ".[nama_extra]"`**
- **Contoh: `pip install -e ".[dev]"` menginstall dependensi pengembangan**

### Apa perbedaan antara `pip install .` dan `pip install -e .`?

- **`pip install .` menyalin file ke site-packages**
- **`pip install -e .` membuat symbolic link ke source code**
- **Editable installs mencerminkan perubahan kode secara langsung**

### Bagaimana Debug Toolbar terintegrasi dengan Pyramid?

- **Dikonfigurasi melalui file .ini atau secara programatik dalam setup.py**
- **Menyediakan antarmuka visual untuk informasi debugging**
- **Menawarkan fitur seperti inspeksi request/response dan analisis SQL query**

### Apa manfaat menggunakan `dev_requires` untuk dependensi pengembangan?

- **Menjaga deployment produksi lebih kecil dan cepat**
- **Mengurangi risiko keamanan dengan tidak menginstall package yang tidak perlu**
- **Memungkinkan pemisahan concern yang lebih bersih**