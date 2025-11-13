# Analisis: Penanganan Web Dasar dengan Views

## Analisis

- **Views menangani web requests dan mengembalikan responses**
- **Views sekarang berada dalam modul `views.py` yang terpisah**
- **Konfigurasi menggunakan decorator `@view_config` untuk registrasi view deklaratif**

## Jawaban Extra Credit

### Apa tujuan decorator `@view_config`?

- **Mendaftarkan fungsi atau method view dengan route dan renderer spesifik**
- **Dapat menentukan opsi tambahan seperti request method dan parameters**

### Bagaimana Pyramid mencocokkan URLs dengan views?

- **Pyramid menggunakan konfigurasi routing untuk mencocokkan URLs yang masuk dengan view yang sesuai**
- **View kemudian dipanggil dengan objek request, dan response dikembalikan**

### Apa peran renderer dalam konfigurasi view?

- **Renderer bertanggung jawab mengkonversi data response view menjadi format response akhir**
- **Dapat berupa file template, JSON, atau format lainnya**

### Bagaimana cara mentest skenario berbeda untuk fungsi view?

- **Gunakan parameter request atau headers yang berbeda dalam tests**
- **Mock dependencies atau services yang digunakan oleh view**
- **Assert pada status response, headers, dan konten body**

### Apa keuntungan memisahkan views ke dalam modul yang berbeda?

- **Meningkatkan organisasi kode dan maintainability**
- **Memisahkan concerns antara konfigurasi dan logika aplikasi**
- **Memungkinkan testing dan debugging yang lebih mudah**