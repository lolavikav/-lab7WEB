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

## Modul 2: CRUD & Interaksi Database
Di tahap ini, website dikembangkan menjadi lebih dinamis dengan menambahkan fitur pengelolaan data menggunakan MySQL.

Alurnya: dibuat `ArtikelModel`.php yang berfungsi sebagai penghubung antara aplikasi dengan tabel `artikel` di database.

Fitur pada Admin:

- Create: menyediakan form untuk menambahkan data berita baru.
- Read: menampilkan data dari database ke dalam bentuk tabel HTML.
- Update: mengambil data berdasarkan ID untuk kemudian bisa diedit kembali.
- Delete: menghapus data secara permanen dari database.

Konfigurasi: melakukan pengaturan koneksi database melalui file `.env.`

## Modul 3: Templating ( Viem Layout & View Cell)
Pada tahap ini, diterapkan prinsip DRY (Don't Repeat Yourself) supaya kode lebih rapi dan tidak berulang-ulang.

Untuk tampilan, digunakan konsep View Layout dengan satu file utama `layout/main.php`. Halaman lain cukup mengisi bagian tertentu saja menggunakan `$this->extend()`, jadi tidak perlu membuat struktur dari awal lagi.

Selain itu, dibuat View Cell berupa komponen modular seperti `ArtikelTerkini`. Komponen ini bisa dipanggil di berbagai halaman tanpa harus menulis ulang query database di setiap Controller.

Manfaatnya, kalau ada perubahan pada bagian seperti Header atau Footer, cukup ubah di satu file saja tanpa harus edit semua halaman.

## Modul 4: Autentikasi & Security Filter
Tahap ini berfokus pada pengamanan area penting seperti Dashboard Admin agar tidak bisa diakses sembarangan.

Alurnya: proses login dilakukan dengan memvalidasi username dan password menggunakan Session.

Pengamanan: diterapkan `AuthFilter.php.` Jika ada user yang mencoba mengakses halaman `/admin` tanpa login, sistem akan otomatis mengarahkan kembali ke halaman `/login.`

Database: dibuat tabel user untuk menyimpan data akun dan kredensial admin.

## Modul 5: Optimasi UX (Pagination & Searching)
Tahap ini berfokus pada peningkatan tampilan dan performa saat jumlah data sudah banyak.

- Pagination: penggunaan `findAll()` diganti dengan `paginate(10)` agar data ditampilkan per halaman, sehingga mencegah browser menjadi lambat ketika data sudah sangat banyak.
- Searching: memanfaatkan metode `like()` pada query SQL untuk mencari dan memfilter judul artikel sesuai kata kunci yang dimasukkan user.
- Persistence: menggunakan `pager->only(['q'])` supaya ketika user berpindah halaman (misalnya ke halaman 2), kata kunci pencarian tetap tersimpan dan hasilnya tidak hilang.

## Cara Instalasi Proyek
1. Clone & Setup:
   `

2. Database:
   - Buat Database Bernama `lab_ci4`
   - import file `.sql` yang bernama `database/`

3. Environment:
   - rename `env` menjadi `.env`
   - atur `database.deafult.username` dan `database.deafult.password` sesuai xampp masing masing.

4. Run:
   `php park serve`


## Bukti Hasil Praktikum
1. TAMPILAN HOME USER:
<img width="1076" height="950" alt="Screenshot 2026-04-07 224047" src="https://github.com/user-attachments/assets/30e057d1-1081-4792-9e91-bc3b9d304273" />

TAMPILAN ARTIKEL:
<img width="1412" height="898" alt="Screenshot 2026-04-07 224114" src="https://github.com/user-attachments/assets/70cd4e3b-8285-4013-a2f8-ae2bf22fb442" />

TAMPILAN ABOUT:
<img width="1496" height="916" alt="Screenshot 2026-04-07 224133" src="https://github.com/user-attachments/assets/6342fcef-6b03-42b3-a4d3-0c1c330390e5" />

TAMPILAN CONTACT:
<img width="1619" height="937" alt="Screenshot 2026-04-07 224155" src="https://github.com/user-attachments/assets/226ca46b-bd58-4a9a-aa09-26a775ed3119" />

2. DASHBOARD ADMIN:
<img width="1417" height="944" alt="Screenshot 2026-04-07 232052" src="https://github.com/user-attachments/assets/12899036-080b-41ca-8244-920c3695e8b3" />

TAMPILAN TAMBAH ARTIKEL:
<img width="1373" height="930" alt="Screenshot 2026-04-07 224302" src="https://github.com/user-attachments/assets/222f48f6-b12a-4a27-b0c4-1604e3675fdd" />

TAMPILAN UBAH ARTIKEL:
<img width="1369" height="890" alt="Screenshot 2026-04-07 224323" src="https://github.com/user-attachments/assets/c0c369a8-004e-4d86-a9b1-68214e318496" />

3.HALAMAN LOGIN:
<img width="1139" height="887" alt="Screenshot 2026-04-07 224358" src="https://github.com/user-attachments/assets/1e3dd078-d422-4923-8d80-fd2e346b4412" />







