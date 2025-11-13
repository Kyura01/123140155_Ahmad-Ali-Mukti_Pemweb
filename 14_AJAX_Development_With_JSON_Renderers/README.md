# 14: AJAX Development With JSON Renderers

## Analysis

- **JSON renderers mengkonversi data Python ke JSON dan menetapkan content type response**
- **Pyramid menyediakan built-in JSON renderer, dan custom renderers dapat dibuat**
- **AJAX views dapat diimplementasikan dengan mudah menggunakan JSON renderers**

## Jawaban Extra Credit

### Apa tujuan dari JSON renderer?

**JSON renderer berperan dalam melakukan konversi data Python ke format JSON yang standar. Selain itu, renderer ini juga secara otomatis menetapkan response content type menjadi `application/json`, memastikan client dapat menginterpretasi data dengan benar.**

### Bagaimana cara mendefinisikan view yang mengembalikan JSON?

**Definisi view yang mengembalikan JSON dapat dilakukan dengan menggunakan decorator `@view_config` yang dilengkapi opsi `renderer='json'`. Selanjutnya, view function tersebut perlu mengembalikan struktur data Python seperti dictionary atau list yang akan secara otomatis dikonversi menjadi JSON.**

### Apa keuntungan menggunakan JSON untuk AJAX responses?

**Penggunaan JSON dalam AJAX responses menawarkan beberapa keunggulan signifikan. Pertama, JSON memiliki format yang lightweight dan mudah di-parse oleh JavaScript. Kedua, Python menyediakan dukungan native melalui modul `json`. Ketiga, JSON mampu merepresentasikan struktur data yang kompleks dengan efisien.**

### Bagaimana cara mengkustomisasi proses JSON rendering?

**Kustomisasi proses JSON rendering dapat dicapai melalui dua pendekatan utama. Pendekatan pertama adalah dengan memperluas built-in JSON renderer yang sudah tersedia. Alternatif lainnya adalah dengan membuat custom renderer sepenuhnya, yang memungkinkan developer untuk mendefinisikan logika serialisasi khusus untuk tipe-tipe data tertentu.**

### Apa perbedaan antara `json.dumps` dan `json.dump`?

**Kedua fungsi ini memiliki tujuan yang serupa namun dengan mekanisme output yang berbeda. `json.dumps` berfungsi untuk melakukan serialisasi objek menjadi string berformat JSON yang dapat langsung digunakan dalam kode. Sementara itu, `json.dump` melakukan serialisasi objek dan langsung menuliskannya ke file-like object, cocok untuk penyimpanan data ke file.**