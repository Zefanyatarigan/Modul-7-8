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
