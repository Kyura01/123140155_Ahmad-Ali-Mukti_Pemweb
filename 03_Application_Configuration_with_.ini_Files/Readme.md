# Analisis

- **Konfigurasi dipisahkan dari kode**
- **Menggunakan file .ini untuk pengaturan**
- **Entry points mendefinisikan perilaku aplikasi**
- **Perintah pserve mem-bootstrap aplikasi**

## Jawaban Extra Credit

### Apa peran global_config dalam fungsi main?

- **global_config adalah placeholder untuk pengaturan global, jarang digunakan dalam praktik**
- **Memungkinkan penyampaian opsi konfigurasi dari file .ini**
- **Dapat diabaikan jika tidak diperlukan**

### Bagaimana pengaturan dikirim dari file .ini ke aplikasi?

- **Melalui **settings dalam signature fungsi main**
- **Dibongkar sebagai keyword arguments dalam Configurator**
- **Tersedia sebagai settings dalam aplikasi**

### Apa tujuan entry_points dalam setup.py?

- **Mendefinisikan entry points untuk aplikasi**
- **Memberitahu Pyramid di mana menemukan WSGI application factory**
- **Digunakan oleh perintah pserve untuk mem-bootstrap aplikasi**

### Bagaimana Pyramid menemukan WSGI application factory?

- **Mencari fungsi main dalam modul yang ditentukan**
- **Modul ditentukan oleh entry_points dalam setup.py**
- **Default adalah tutorial:main untuk package tutorial**

### Apa efek dari direktif use dalam file .ini?

- **Menentukan aplikasi dan server yang akan digunakan**
- **egg:tutorial mengacu pada entry point package yang terinstall**
- **egg:waitress#main menentukan Waitress sebagai WSGI server**