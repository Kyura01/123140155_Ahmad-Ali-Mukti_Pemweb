# Aplikasi Web Pyramid dengan Waitress

Aplikasi web Pyramid sederhana yang mendemonstrasikan setup web server dasar menggunakan Waitress sebagai WSGI server.

## Fitur

- **Proses konfigurasi dan startup yang sederhana**
- **Menggunakan Waitress sebagai WSGI server**
- **Fungsi view dasar yang mengembalikan respons HTML**
- **Menunjukkan persyaratan minimal setup Pyramid**

## Instalasi

1. Install dependensi yang diperlukan:
```bash
pip install pyramid waitress
```

## Penggunaan

Jalankan aplikasi:
```bash
python App.py
```

Server akan berjalan pada `http://0.0.0.0:6543` dan menampilkan "Hello World!" ketika diakses.

## Struktur Kode

- Fungsi view sederhana yang mengembalikan respons HTML
- Setup konfigurasi Pyramid dengan routing
- Waitress WSGI server untuk serving yang siap produksi
- Boilerplate minimal untuk pengembangan cepat

## Jawaban Extra Credit

### Perbedaan print statement:

- **Versi dengan tanda kurung adalah sintaks Python 3**
- **Tanpa tanda kurung adalah sintaks lama Python 2**

### Alternatif nilai return:

- **String HTML memerlukan pembungkus Response()**
- **Urutan integer bukanlah respons yang valid**

### Dampak kode yang tidak valid:

- **NameError menunjukkan penanganan error**
- **Mendemonstrasikan kemampuan debugging**

### Warisan WSGI:

- **Berdasarkan standar CGI**
- **Menstandardisasi antarmuka web server/aplikasi**

## Catatan Teknis

Aplikasi ini mendemonstrasikan:
- Persyaratan minimal setup framework Pyramid
- Integrasi WSGI server dengan Waitress
- Penanganan HTTP request/response dasar
- Konfigurasi server yang siap produksi