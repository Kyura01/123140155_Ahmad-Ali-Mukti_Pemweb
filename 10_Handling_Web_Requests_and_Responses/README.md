# 10: Handling Web Requests and Responses

## Analisis

- **Penanganan request dan response berdasarkan library WebOb**
- **Parameter request diakses melalui `request.params`**
- **Response headers dan body dapat dimodifikasi sebelum mengembalikan response**

## Jawaban Extra Credit

### Apa peran objek `request` dalam sebuah view?

**Objek request berfungsi sebagai representasi HTTP request yang masuk ke sistem. Selain itu, objek ini juga menyediakan berbagai akses ke parameter request, headers, serta atribut-atribut lainnya yang diperlukan.**

### Bagaimana cara mengakses query parameters dalam view?

**Query parameters dapat diakses melalui objek `request.params` yang berperilaku seperti dictionary. Sebagai contoh implementasinya: `name = request.params.get('name')`.**

### Apa tujuan dari class `Response`?

**Class Response bertugas merepresentasikan HTTP response yang nantinya akan dikirim kepada client. Melalui class ini, developer dapat mengatur berbagai aspek seperti status response, headers, maupun body content.**

### Bagaimana cara memodifikasi response headers?

**Modifikasi response headers dilakukan dengan cara menetapkan atribut pada objek `Response`. Implementasinya dapat dilakukan seperti: `response.headers['X-Custom-Header'] = 'Value'`.**

### Apa perbedaan antara `HTTPFound` dan `Response`?

**`HTTPFound` merupakan subclass khusus dari `Response` yang dirancang untuk menangani HTTP 302 redirects. Sementara itu, `HTTPFound` sebaiknya digunakan ketika kita perlu melakukan redirect ke URL yang berbeda.**
