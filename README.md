# Laporan Praktikum 8: PHP dan Database MySQL

**Nama** : Kanaya Tabitha Sely Selovena
**NIM**  : 312510086
**Mata Kuliah** : Pemrograman Web OBE

## Tujuan
1. Memahami konsep dasar database.
2. Memahami konsep dasar CRUD menggunakan PHP.
3. Membuat program CRUD sederhana menggunakan PHP.

## 1. Persiapan
Menjalankan Apache dan MySQL melalui XAMPP Control Panel, lalu membuka phpMyAdmin di `http://localhost/phpmyadmin/`.

## 2. Membuat Database dan Tabel
Membuat database `latihan1` dan tabel `data_barang` dengan perintah SQL (lihat `database/latihan1.sql`), lalu mengisi 3 data awal.

![Struktur tabel](screenshots/01-struktur-tabel.png)
![Data awal](screenshots/02-data-awal.png)

## 3. File Koneksi (koneksi.php)
Berisi `mysqli_connect()` untuk menghubungkan PHP ke database `latihan1`. Jika koneksi gagal, tampil pesan "Koneksi ke server gagal."

![Tes koneksi](screenshots/03-koneksi.png)

## 4. Read (index.php)
Menjalankan `SELECT * FROM data_barang`, lalu menampilkan hasilnya dalam tabel HTML menggunakan perulangan `while`.

![Index](screenshots/04-index.png)

## 5. Create (tambah.php)
Form untuk menambah barang. Data dikirim dengan method POST, gambar diupload ke folder `gambar/`, lalu data disimpan dengan perintah `INSERT`.

![Form tambah](screenshots/05-tambah.png)
![Hasil tambah](screenshots/06-hasil-tambah.png)

## 6. Update (ubah.php)
Mengambil data berdasarkan `id_barang`, menampilkannya di form, lalu menyimpan perubahan dengan perintah `UPDATE`.

![Form ubah](screenshots/07-ubah.png)
![Hasil ubah](screenshots/08-hasil-ubah.png)

## 7. Delete (hapus.php)
Menghapus data berdasarkan `id_barang` dengan perintah `DELETE`, lalu kembali ke `index.php`.

![Hasil hapus](screenshots/09-hasil-hapus.png)

## Kesimpulan
Program CRUD sederhana dengan PHP dan MySQL berhasil dibuat dan dapat menambah, menampilkan, mengubah, dan menghapus data barang.
