# rangkuman-materi
Bab 1 membahas bagaimana melakukan konversi dari Entity Relationship Diagram (ERD) ke skema relasi dan kemudian menjadi tabel fisik dalam basis data.

Tujuan Pembelajaran
Memahami cara mengubah ERD menjadi skema relasi.
Memudahkan proses transformasi dari level konseptual ke level fisik database.

Isi Utama Bab 1
1. Konsep Dasar
Entitas → menjadi tabel.
Atribut → menjadi kolom.
Primary Key (PK) → kolom kunci utama.
Foreign Key (FK) → kolom yang mengacu ke tabel lain.
Relasi dan kardinalitas menentukan penempatan FK.

2. Aturan Konversi ER ke Skema Relasi
Beberapa aturan penting:
Entitas kuat → tabel mandiri.
Atribut komposit → dipecah menjadi kolom kolom sederhana.
Atribut multivalue → menjadi tabel baru.
Entitas lemah → tabel dengan FK ke entitas kuat.
Relasi 1–1, 1–N, N–N → menentukan peletakan FK dan tabel relasi.
Unary, ternary, generalisasi/spesialisasi, agregasi memiliki aturan khusus.

3. Studi Kasus: Skema Pembayaran Apotik
Dibahas ERD apotik lengkap dengan:
Pasien, resep, obat, pegawai, pembayaran, retur, kategori obat, dsb.
Hasil konversi berupa 13 tabel, misalnya:
PASIEN
RESEP
OBAT
DETAIL_OBAT
PEMBAYARAN
PEGAWAI
RETUR
KATEGORI_OBAT
dll.

Bab 1 juga berisi contoh diagram relationship akhir dan daftar tabel hasil relasi.

Ringkasan Bab 2 – Pengantar Basis Data & DDL
Bab ini membahas pengenalan database dan dasar penggunaan MySQL, terutama perintah DDL (Data Definition Language).

Tujuan Pembelajaran
Memahami dasar database dan DBMS.
Menjalankan MySQL server & client.
Mengenal tipe data pada MySQL.
Mampu membuat database menggunakan perintah DDL.

Isi Utama Bab 2
1. Pengenalan DBMS MySQL
MySQL adalah DBMS berbasis SQL, bersifat open-source.

Keunggulan:

cepat dan stabil
reliable
mendukung banyak OS
multithreaded
enkripsi bagus
open source

2. Instalasi
Umumnya menggunakan XAMPP (MariaDB menggantikan MySQL).
Server MySQL dapat dijalankan via Control Panel XAMPP.

3. Mengakses MySQL
Melalui Command Prompt:
cd c:\xampp\mysql\bin
mysql -u root -p
-u → username
-p → password
-h → host

4. Client MySQL
Program mysql.exe digunakan sebagai client (CLI).
Semua perintah SQL harus diakhiri titik koma (;).

5. Tipe Data MySQL
Beberapa tipe data yang sering digunakan:
INT
FLOAT
CHAR / VARCHAR
DATE, DATETIME
BLOB, LONGBLOB

6. Database Relasional
Database = kumpulan tabel.
Tabel = kumpulan kolom dan baris.

7. Perintah DDL Dasar
Membuat Database
CREATE DATABASE nama_db;
Melihat Semua Database
SHOW DATABASES;
Menggunakan Database
USE nama_db;
Menghapus Database
DROP DATABASE nama_db;

Bab 2 juga menyertakan Test Akhir untuk latihan pembuatan database dan pengoperasian perintah SQL dasar.
