<h1 align="center">LAPORAN PRAKTIKUM</h1>
<h1 align="center">APLIKASI BERBASIS PLATFORM</h1>

<br>

<h2 align="center">TUGAS 2</h2>
<h2 align="center">Modul 7 & 8</h2>

<br>

<p align="center">
  <img src="./Asset/LogoTelkom.png" width="250" alt="Logo Telkom University">
</p>
<br><br>

<h2 align="center">Disusun Oleh :</h2>

<p align="center" style="font-size:28px;">
  <b>Zefanya Brana Tertius Tarigan</b><br>
  <b>2311102028</b><br>
  <b>S1 Informatika</b>
</p>

<br>

<h2 align="center">PROGRAM STUDI S1 INFORMATIKA</h2>
<h2 align="center">FAKULTAS INFORMATIKA</h2>
<h2 align="center">TELKOM UNIVERSITY</h2>
<h2 align="center">TAHUN 2026</h2>

<hr>

## 1. Dasar Teori

### NodeJS (Express)
NodeJS merupakan runtime JavaScript yang digunakan untuk menjalankan kode JavaScript di sisi server. Pada project ini, NodeJS digunakan bersama framework Express untuk mengatur routing halaman, menangani request dan response, serta menjalankan proses CRUD.

### Bootstrap
Bootstrap adalah framework CSS yang digunakan untuk membangun tampilan website agar lebih rapi, responsif, dan modern. Pada project ini, Bootstrap digunakan untuk membuat navbar, card, button, form, dan tabel.

### jQuery dan jQuery Plugin
jQuery adalah library JavaScript yang mempermudah manipulasi elemen HTML, event handling, dan interaksi halaman. Pada project ini, jQuery digunakan bersama plugin:
- DataTables
- jQuery Validate
- jQuery Toast

### CRUD
CRUD adalah singkatan dari Create, Read, Update, Delete. Pada project ini:
- Create digunakan untuk menambah data mahasiswa
- Read digunakan untuk menampilkan data mahasiswa
- Update digunakan untuk mengubah data mahasiswa
- Delete digunakan untuk menghapus data mahasiswa

### JSON
JSON adalah format pertukaran data yang ringan dan mudah dibaca. Pada project ini, data mahasiswa disimpan dalam file `students.json` dan ditampilkan ke tabel menggunakan DataTables.

## 2. Struktur Halaman

Aplikasi ini memiliki halaman utama sebagai berikut:

### Halaman Home
Halaman home merupakan halaman awal aplikasi yang berisi judul aplikasi, deskripsi singkat, dan tombol navigasi ke halaman input data serta tabel data.

### Halaman Form (Input Data)
Halaman ini digunakan untuk memasukkan data mahasiswa, seperti NIM, nama, jurusan, dan email.

### Halaman Data (Tabel)
Halaman ini digunakan untuk menampilkan data mahasiswa dalam bentuk tabel interaktif menggunakan jQuery DataTables.

### Halaman Edit
Halaman ini digunakan untuk memperbarui data mahasiswa yang sudah tersimpan.

## 3. Struktur Folder

```text
web-crud-app
│
├── app.js
├── package.json
├── package-lock.json
│
├── Asset
│   ├── LogoTelkom.png
│   ├── Page 1.png
│   ├── Page 2.png
│   └── Page 3.png
│
├── data
│   └── students.json
│
├── public
│   ├── css
│   │   └── style.css
│   └── js
│       ├── form.js
│       └── table.js
│
└── views
    ├── index.ejs
    ├── students.ejs
    ├── create.ejs
    ├── edit.ejs
    └── partials
        ├── header.ejs
        └── footer.ejs

### Penjelasan Struktur Folder

| File / Folder | Keterangan |
|--------------|-----------|
| `app.js` | File utama NodeJS (Express) yang mengatur routing halaman, endpoint JSON, dan proses CRUD data mahasiswa. |
| `package.json` | File konfigurasi project yang berisi informasi project, script untuk menjalankan aplikasi, dan daftar dependency yang digunakan. |
| `package-lock.json` | File lock dependency hasil instalasi npm untuk memastikan versi package yang digunakan tetap konsisten. |
| `Asset/` | Folder yang berisi logo dan dokumentasi output aplikasi berupa screenshot halaman project. |
| `Asset/LogoTelkom.png` | File logo yang ditampilkan pada bagian atas laporan di `README.md`. |
| `Asset/Page 1.png` | Screenshot halaman Home aplikasi. |
| `Asset/Page 2.png` | Screenshot halaman Form Input Data. |
| `Asset/Page 3.png` | Screenshot halaman Tabel Data Mahasiswa. |
| `data/` | Folder penyimpanan data utama aplikasi dalam format JSON. |
| `data/students.json` | File JSON yang berisi data mahasiswa dan digunakan sebagai sumber data pada tabel DataTables. |
| `public/` | Folder untuk file statis yang dapat diakses langsung oleh browser. |
| `public/css/` | Folder untuk file CSS tambahan. |
| `public/css/style.css` | File CSS yang digunakan untuk menambahkan styling khusus pada tampilan aplikasi. |
| `public/js/` | Folder untuk file JavaScript frontend. |
| `public/js/form.js` | File JavaScript yang berisi validasi form menggunakan jQuery Validate dan notifikasi menggunakan jQuery Toast. |
| `public/js/table.js` | File JavaScript yang berisi implementasi DataTables untuk menampilkan data JSON ke dalam tabel. |
| `views/` | Folder template EJS yang digunakan untuk menampilkan halaman aplikasi. |
| `views/index.ejs` | File halaman Home atau halaman utama aplikasi. |
| `views/create.ejs` | File halaman Form Input untuk menambahkan data mahasiswa. |
| `views/students.ejs` | File halaman Tabel Data yang menampilkan data mahasiswa dengan DataTables. |
| `views/edit.ejs` | File halaman Edit Data untuk memperbarui data mahasiswa. |
| `views/partials/` | Folder untuk komponen halaman yang digunakan berulang. |
| `views/partials/header.ejs` | Bagian header yang berisi struktur awal HTML, import Bootstrap CSS, dan navbar aplikasi. |
| `views/partials/footer.ejs` | Bagian footer yang berisi import jQuery, DataTables, jQuery Validate, jQuery Toast, dan penutup HTML. |
