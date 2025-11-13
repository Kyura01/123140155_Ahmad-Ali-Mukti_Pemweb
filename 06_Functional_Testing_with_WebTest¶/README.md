# Kajian: Pengujian Fungsional menggunakan WebTest

## Ringkasan Kajian

- **Pengujian fungsional mengevaluasi keseluruhan aplikasi, termasuk integrasi routing dan view**
- **WebTest digunakan untuk mensimulasikan HTTP requests dan memeriksa responses**
- **Organisasi dan struktur pengujian sangat krusial untuk kemudahan maintenance**

## Jawaban Pertanyaan Tambahan

### Apa perbedaan mendasar antara unit tests dan functional tests?

- **Unit tests mengevaluasi komponen secara individual dan terisolasi, sedangkan functional tests menguji aplikasi secara menyeluruh**
- **Functional tests memeriksa interaksi antar komponen dan kebenaran workflow sistem**

### Mengapa webtest perlu ditambahkan sebagai development dependency?

- **WebTest bukan bagian dari standard library Python, sehingga wajib ditambahkan sebagai dependency**
- **Menyediakan cara untuk mensimulasikan HTTP requests dan memeriksa responses dalam functional testing**

### Bagaimana prosedur menjalankan functional tests pada aplikasi?

- **Menggunakan perintah `pytest` di terminal, sama seperti unit tests**
- **Bisa menambahkan opsi seperti `--cov` untuk laporan coverage**
- **Dapat diintegrasikan dengan CI/CD pipelines untuk automated testing**

### Apa peran penting `DummyRequest` dalam pengujian?

- **`DummyRequest` adalah test double yang mensimulasikan HTTP request**
- **Memungkinkan pengujian views dan routes tanpa menjalankan server sesungguhnya**
- **Dapat dikustomisasi dengan parameters, headers, dan atribut request lainnya**

### Bagaimana cara menguji berbagai skenario untuk fungsi view dalam functional tests?

- **Menggunakan parameters request atau headers yang bervariasi dalam pengujian**
- **Melakukan mocking terhadap dependencies atau services yang digunakan view**
- **Melakukan assertion pada status response, headers, dan konten body**