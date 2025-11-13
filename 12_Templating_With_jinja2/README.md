# 12: Templating With jinja2

## Analysis

- **Jinja2 merupakan sistem templating populer yang dapat digunakan dengan Pyramid**
- **Templates didefinisikan dalam file terpisah dengan ekstensi `.jinja2`**
- **Sintaks template mirip dengan Chameleon, dengan penyisipan variabel menggunakan `{{ }}`**

## Jawaban Extra Credit

### Apa tujuan dari package `pyramid_jinja2`?

**Package `pyramid_jinja2` bertugas mengaktifkan fungsionalitas templating Jinja2 dalam aplikasi Pyramid. Untuk dapat berfungsi dengan baik, package ini harus diinstall terlebih dahulu dan disertakan dalam konfigurasi aplikasi.**

### Bagaimana cara mendefinisikan template dalam Jinja2?

**Pembuatan template Jinja2 dilakukan dengan membuat file yang memiliki ekstensi `.jinja2`, kemudian mendefinisikan struktur HTML dengan embedded Python expressions di dalamnya. Pendekatan ini memungkinkan integrasi yang seamless antara logika Python dan presentation layer.**

### Apa keuntungan menggunakan sistem templating?

**Sistem templating menawarkan berbagai keunggulan, terutama dalam hal pemisahan presentation logic dari business logic. Selain itu, penggunaan templating juga meningkatkan organisasi kode dan maintainability secara signifikan, serta memungkinkan proses testing dan debugging yang lebih mudah.**

### Bagaimana cara beralih antara sistem template yang berbeda dalam Pyramid?

**Perpindahan antar sistem template dapat dilakukan dengan menginstall package sistem template yang diinginkan, seperti `pyramid_jinja2` untuk Jinja2. Setelah instalasi, langkah selanjutnya adalah menyertakannya dalam konfigurasi dan menentukan ekstensi file template yang sesuai.**

### Apa perbedaan antara `render_template` dan `render_to_response`?

**Kedua fungsi ini memiliki tujuan yang berbeda dalam proses rendering template. `render_template` berfungsi untuk merender template dan mengembalikan hasilnya dalam bentuk string, sedangkan `render_to_response` merender template dan mengembalikannya dalam bentuk objek `Response` yang siap dikirim ke client.**
