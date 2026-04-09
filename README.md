# -lab7WEB
# Nama: Lola Seftyliani
# Kelas:I24ID
# NIM: 312410339
# Matkul: Pemrograman Web

# Praktikum Pemograman Web Sistem Informasi Portal Berita - Codelgniter 4

# Analisis Struktur Modul Praktikum

## Modul 1: Fondasi MVC & Routing
Di tahap awal, yang jadi fokus utama adalah mengubah cara kerja dari PHP Native ke penggunaan Framework.

Alurnya: saat user mengakses URL, permintaan tersebut akan diarahkan oleh `Routes.php` ke `Controller`, lalu Controller akan memanggil `View` untuk ditampilkan.

Penerapannya: membuat `Controller` bernama `Page.php` yang digunakan untuk mengatur halaman statis seperti Home, About, dan Contact.

Hal penting yang dipelajari: logika bisnis sebaiknya tidak ditempatkan di dalam View, tapi dipisahkan agar struktur kode lebih rapi dan mudah dikelola.

