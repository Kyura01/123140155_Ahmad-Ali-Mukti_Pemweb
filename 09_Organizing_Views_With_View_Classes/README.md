# 09: Organizing Views With View Classes

## Analysis

- **View classes mengelompokkan views yang terkait dan berbagi konfigurasi**
- **Decorator `@view_defaults` tingkat class menetapkan default untuk semua views dalam class**
- **Penanganan pola URL dan view predicates memungkinkan routing yang fleksibel**

## Jawaban Extra Credit

### Apa tujuan decorator `@view_defaults`?

- **Menetapkan opsi default untuk semua views dalam class, seperti renderer dan route name**

### Bagaimana view class berbagi state antar views?

- **Melalui instance variables yang ditetapkan dalam constructor (method `__init__`) dari view class**

### Apa peran property `full_name` dalam view class?

- **Mengenkapsulasi logika untuk membangun nama lengkap dari parameter URL**
- **Tersedia untuk semua views dan templates sebagai atribut**

### Bagaimana view predicates bekerja?

- **View predicates adalah kondisi yang harus dipenuhi agar view dapat dipanggil**
- **Dapat mencocokkan pada request method, parameters, headers, dan atribut lainnya**

### Apa perbedaan antara `route_path` dan `route_url`?

- **`route_path`: Mengembalikan path dari URL (contoh: `/howdy/First/Last`)**
- **`route_url`: Mengembalikan URL lengkap, termasuk scheme dan host (contoh: `http://localhost:6543/howdy/First/Last`)**
