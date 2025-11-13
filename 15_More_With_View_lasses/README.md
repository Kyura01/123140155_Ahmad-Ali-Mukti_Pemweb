# 15: More With View Classes Analysis

## Analysis

- **View classes memungkinkan pengorganisasian views yang terkait secara bersamaan**
- **Konfigurasi tingkat class dengan decorator `@view_defaults`**
- **Penanganan pola URL dan view predicates memungkinkan routing yang fleksibel**

## Jawaban Extra Credit

### Apa tujuan dari decorator `@view_defaults`?

**Decorator `@view_defaults` berperan dalam menetapkan opsi-opsi default untuk seluruh views yang berada dalam suatu class. Melalui decorator ini, konfigurasi seperti renderer dan route name dapat didefinisikan sekali saja dan secara otomatis diterapkan pada semua views dalam class tersebut.**

### Bagaimana view class berbagi state antar views?

**Pembagian state antar views dalam suatu class dapat dicapai melalui penggunaan instance variables yang ditetapkan dalam constructor (method `__init__`) dari view class. Pendekatan ini memungkinkan setiap view dalam class yang sama untuk mengakses dan memanipulasi data yang telah diinisialisasi sebelumnya.**

### Apa peran property `full_name` dalam view class?

**Property `full_name` berfungsi sebagai enkapsulasi logika untuk membangun nama lengkap berdasarkan parameter-parameter URL yang diterima. Keunggulan dari property ini adalah ketersediaannya untuk semua views dan templates sebagai atribut yang dapat langsung diakses, sehingga meningkatkan efisiensi dan konsistensi kode.**

### Bagaimana cara kerja view predicates?

**View predicates beroperasi sebagai kondisi-kondisi yang harus terpenuhi agar suatu view dapat dipanggil oleh sistem. Mekanisme ini sangat fleksibel karena dapat melakukan pencocokan berdasarkan berbagai aspek seperti request method, parameters, headers, dan atribut-atribut lainnya yang relevan dengan request yang masuk.**

### Apa perbedaan antara `route_path` dan `route_url`?

**Kedua fungsi ini memiliki tujuan yang serupa namun menghasilkan output yang berbeda dalam hal kelengkapan informasi. `route_path` menghasilkan hanya bagian path dari URL seperti `/howdy/First/Last`, sedangkan `route_url` menghasilkan URL yang lengkap mencakup scheme dan host, contohnya `http://localhost:6543/howdy/First/Last`.**