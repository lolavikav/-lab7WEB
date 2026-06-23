# LAPORAN PRAKTIKUM MODUL 1-14

## NAMA: LOLA SEFTYLIANI
## KELAS: I241D
## NIM: 312410339
## MATKUL: PEMOGRAMAN WEB2

## Dokumentasi tentang Praktikum Website
Repositori ini digunakan sebagai dokumentasi berbagai tugas praktikum mata kuliah Pemrograman Website. Pengembangan aplikasi dilakukan dengan menerapkan CodeIgniter 4 pada sisi backend dan Vue.js pada sisi frontend guna membangun sistem web yang responsif, terorganisir, dan mudah dikelola

# PRAKTIKUM MODUL 1-14
# Penjelasan Praktikum 
# Progres Pengembangan Sistem
1. Fase Dasar (Modul 1–3)
Tahap awal difokuskan pada pemahaman dasar framework CodeIgniter 4, mulai dari proses instalasi dan konfigurasi lingkungan kerja, pembuatan Controller dan View, hingga pengelolaan data menggunakan Database dan Model. Fase ini menjadi landasan utama dalam pengembangan aplikasi web.
2. Fase Pengelolaan Data dan Antarmuka (Modul 4–6)
Pada tahap ini, aplikasi mulai dikembangkan dengan fitur pengelolaan data artikel menggunakan operasi CRUD (Create, Read, Update, Delete). Selain itu, diterapkan Form Handling dan validasi data untuk memastikan input pengguna sesuai dengan aturan yang ditentukan. Penggunaan View Layouts juga membantu menciptakan tampilan yang lebih terstruktur dan mudah dikelola.
3. Fase Interaktivitas (Modul 7–9)
Pengembangan selanjutnya berfokus pada peningkatan pengalaman pengguna melalui penerapan AJAX. Teknologi ini memungkinkan data diperbarui secara dinamis tanpa perlu memuat ulang seluruh halaman, sehingga aplikasi menjadi lebih responsif dan nyaman digunakan.
4.Fase Pengembangan Web API (Modul 10–12)
Pada fase ini, arsitektur aplikasi mulai dipisahkan antara backend dan frontend. CodeIgniter 4 berperan sebagai penyedia layanan data melalui REST API yang menghasilkan data dalam format JSON, sedangkan Vue.js digunakan untuk mengelola tampilan dan interaksi pada sisi klien.
5. Fase Keamanan dan Penyempurnaan (Modul 13–15)
Tahap akhir difokuskan pada penguatan keamanan aplikasi. Sistem autentikasi berbasis token diterapkan untuk mengontrol akses pengguna, sementara Middleware atau Filter digunakan untuk mengatur kebijakan CORS (Cross-Origin Resource Sharing). Dengan demikian, komunikasi antara frontend dan backend dapat berlangsung secara aman dan terkendali.

# Penjelasan dari setiap modul Praktikum
Perubahan yang terjadi dari Modul 1 hingga Modul 14 menunjukkan proses evolusi aplikasi web dari sistem tradisional menjadi aplikasi modern yang memanfaatkan arsitektur berbasis API. Setiap modul memberikan pengembangan dan penyempurnaan baru yang secara bertahap meningkatkan kemampuan, fleksibilitas, serta kualitas aplikasi. Berikut penjelasan dari setiap tahapan pengembangannya:

## Fase 1: Dasar Pengembangan Web (Modul 1–3)

Tahap awal pengembangan difokuskan pada pemahaman dasar framework CodeIgniter 4 serta alur kerja aplikasi web. Pada Modul 1 dan Modul 2, dilakukan instalasi lingkungan pengembangan sekaligus mempelajari konsep Controller dan View sebagai komponen utama dalam pola MVC (Model-View-Controller). Pada tahap ini, aplikasi masih bersifat sederhana dan menampilkan informasi secara statis.

Selanjutnya, pada Modul 3 diperkenalkan penggunaan Database dan Model. Dengan adanya integrasi MySQL, aplikasi tidak lagi hanya menampilkan data statis, tetapi sudah mampu menyimpan, mengelola, dan menampilkan data secara dinamis sesuai kebutuhan pengguna.

## Fase 2: Interaktivitas dan CRUD (Modul 4–6)

Pada fase ini, aplikasi mulai dikembangkan menjadi sistem yang mampu berinteraksi dengan pengguna. Modul 4 membahas Form Handling dan validasi data untuk memastikan setiap input yang diberikan pengguna dapat diproses dengan aman dan sesuai aturan yang ditentukan.

Kemudian pada Modul 5 diterapkan fitur CRUD (Create, Read, Update, Delete) sehingga aplikasi dapat digunakan untuk mengelola data secara lengkap, seperti menambah, menampilkan, mengubah, dan menghapus data artikel. Pada Modul 6, tampilan aplikasi disusun menggunakan sistem View Layouts agar struktur halaman menjadi lebih rapi, konsisten, dan mudah dipelihara.

## Fase 3: Manajemen Pengguna dan Pengalaman Pengguna (Modul 7–9)

Tahap ini berfokus pada peningkatan fungsi aplikasi dan kenyamanan pengguna. Modul 7 memperkenalkan sistem autentikasi berbasis Session yang memungkinkan pengguna melakukan login dan logout sehingga aplikasi dapat mengenali hak akses setiap pengguna.

Pada Modul 8 dan Modul 9 diterapkan teknologi AJAX yang memungkinkan pertukaran data dilakukan secara asynchronous. Dengan pendekatan ini, pengguna dapat melihat perubahan data tanpa harus melakukan refresh halaman secara penuh, sehingga aplikasi menjadi lebih cepat, responsif, dan interaktif.

### Fase 4: Transformasi ke Arsitektur Web API (Modul 10–12)

Fase ini menandai perubahan besar dalam arsitektur aplikasi. Pada Modul 10, CodeIgniter 4 mulai difungsikan sebagai penyedia layanan data melalui REST API yang menghasilkan data dalam format JSON. Perannya tidak lagi berfokus pada tampilan, melainkan sebagai backend yang melayani permintaan data.

Selanjutnya, Modul 11 memperkenalkan Vue.js sebagai framework frontend untuk membangun antarmuka pengguna yang lebih dinamis. Dengan demikian, frontend dan backend dipisahkan menjadi dua bagian yang saling terhubung. Pada Modul 12, komunikasi antara Vue.js dan REST API dilakukan menggunakan Axios, sekaligus memperkenalkan pengelolaan state untuk menyimpan data dan sesi pengguna pada sisi client.

## Fase 5: Keamanan dan Pengembangan SPA Lanjutan (Modul 13–14)

Tahap akhir difokuskan pada peningkatan keamanan aplikasi. Pada Modul 13 diterapkan sistem autentikasi yang dirancang khusus untuk Single Page Application (SPA). Proses login, pengelolaan token, dan pertukaran data dilakukan dengan mekanisme yang lebih aman. Selain itu, konfigurasi CORS (Cross-Origin Resource Sharing) diperlukan agar komunikasi antara frontend dan backend yang berjalan pada port berbeda dapat dilakukan tanpa kendala.

Kemudian pada Modul 14, keamanan diperkuat melalui penerapan Middleware atau Filters. Komponen ini berfungsi sebagai lapisan pemeriksaan yang memvalidasi setiap request sebelum diproses oleh Controller, sehingga akses yang tidak sah dapat dicegah dan keamanan aplikasi menjadi lebih terjamin.

## ### Arsitektur Komunikasi Data

Aplikasi ini menggunakan komunikasi asynchronous antara frontend (Vue.js) dan backend (CodeIgniter 4) melalui REST API. Data dikirim dan diterima dalam format JSON sehingga proses pertukaran data dapat dilakukan tanpa perlu me-refresh halaman. Karena frontend dan backend berjalan pada port yang berbeda, mekanisme CORS digunakan untuk mengatur dan mengamankan komunikasi antar keduanya.

## Cara Menjalankan Proyek
## 1. Menjalanan Backend ci4
Masuk ke direktori ci4, kemudian jalankan server lokal:
```
gunakan php spark serve port 8080
```
