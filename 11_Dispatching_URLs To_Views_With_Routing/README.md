# 11: Dispatching URLs To Views With Routing

## Analysis

- **Routing mencocokkan URLs yang masuk dengan view yang sesuai berdasarkan konfigurasi**
- **Pyramid memungkinkan pengurutan eksplisit dari routes untuk menghindari ambiguitas**
- **Pola route dapat mengekstrak bagian-bagian URL sebagai parameter**

## Jawaban Extra Credit

### Apa tujuan dari method `add_route`?

**Method `add_route` berperan penting dalam mendaftarkan route baru dengan nama dan pola tertentu. Selain itu, method ini juga mengasosiasikan route tersebut dengan view atau view class yang spesifik.**

### Bagaimana Pyramid mencocokkan URLs yang masuk dengan routes?

**Proses pencocokan dilakukan dengan cara membandingkan URL yang masuk terhadap pola-pola route yang telah terdaftar. Setelah itu, sistem akan mengekstrak parameter dari URL berdasarkan pola yang telah ditetapkan.**

### Apa peran atribut `matchdict` dalam request?

**Atribut `matchdict` berfungsi sebagai wadah yang berisi parameter-parameter yang telah diekstrak dari route yang cocok. Parameter-parameter ini dapat diakses dalam view melalui `request.matchdict`.**

### Bagaimana cara mendefinisikan parameter opsional dalam pola route?

**Parameter opsional dapat didefinisikan dengan menggunakan tanda tanya `?` setelah nama parameter dalam pola. Sebagai contoh: `/howdy/{first}/{last}?` akan membuat parameter `last` menjadi opsional.**

### Apa yang terjadi jika tidak ada route yang cocok dengan URL yang masuk?

**Ketika tidak ada route yang cocok, Pyramid akan mengembalikan response 404 Not Found kepada client. Apabila terdapat aplikasi lain dalam WSGI stack, maka request akan diteruskan ke aplikasi berikutnya.**