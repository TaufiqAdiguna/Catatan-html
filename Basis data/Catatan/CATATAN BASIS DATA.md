
---
# PENGENALAN BASIS DATA

---
# Definisi basis data
## definisi basis
**Basis** diartikan sebagai tempat dimana data-data berkumpul. Contoh Basis adalah lemari arsip menjadi tempat dimana arsip data/dokumen dan objek data lainnya secara fisik disimpan. Contoh lain dari Basis adalah gudang menjadi tempat dimana sekumpulan barang secara fisik disimpan

---
## definisi data
**Data** adalah fakta dari sesuatu.data diperoleh dari hasil pencatatan sebuah kejadian,pengamatan,atau pengukuran.data dapat berupa karakter,teks,kata,angka, video,gambar,atau suara yang dapat kumpulkan dan diproses untuk menghasilkan informasi 
**Sekumpulan fakta dari sebuah objek**

---
## fungsi basis data
Peranan basis data dapat Memudahkan identifikasi data. Menghindari data ganda yang tersimpan. Memudahkan akses, simpan, pembaruan, dan penghapusan data. Menjadi penyimpanan data dari aplikasi atau situs web.

---
## kesimpulan basis data
Basis data adalah suatu tempat atau wadah untuk menyimpan data-data. yang di ibaratkan seperti rak yang dapat menyimpan buku dengan rapi dengan aturan dan perintah tertentu.

---
# peran basis data
Sit halba : pembayaran SPP,data siswa, absensi guru

**Pembayaran SPP**
Mempermudah bendahara dalam mengelola uang pembayaran Spp yang di terima dari siswa.

**Data siswa**
Membantu guru-guru dalam mengelola data siswanya

**Absensi guru**
Digunakan untuk menyimpan absen guru yang hadir,izin,sakit untuk mempermudah HRD dalam mengatur gaji yang harus di terima setiap bulannya

---
# struktur/hirarki database

Struktur atau hirarki database mengacu pada cara data disusun dan diorganisir di dalam database. Dalam konteks ini, struktur database mencakup tabel, kolom, dan hubungan antar tabel. Tabel menyimpan data, kolom mendefinisikan jenis data, dan hubungan antar tabel menggambarkan bagaimana data terkait satu sama lain. Struktur database biasanya dirancang untuk memudahkan penyimpanan, pengambilan, dan pembaruan data dengan efisien.

![Struktur database](Aset/1.1.jpg)

1. **Tabel (Table):** Merupakan entitas utama tempat data disimpan. Setiap tabel memiliki kolom-kolom yang mewakili atribut atau field, dan setiap barisnya mewakili satu entitas atau catatan.
    
2. **Field/kolom :** Merupakan bagian dari tabel yang menentukan jenis data yang dapat disimpan. Setiap kolom memiliki tipe data tertentu, seperti teks, angka, tanggal, dll. Sebagai contoh didalam tabel makmur jaya terdapat id,nama,jabatan adalah contoh field
    
3. **Baris/record :** Juga dikenal sebagai catatan atau tuple, merepresentasikan satu set lengkap data yang terkait dengan entitas tertentu.

4. **Item Data :** Merupakan nilai individu atau entri yang sesuai dengan suatu kolom atau field dalam sebuah tabel. Misalnya, dalam kolom "nama" setiap entri seperti "robin," "tari," atau "Wawan" adalah item data.
## contoh tabel 

==Data karyawan makmur jaya==

| Id    | Nama  | Posisi           | Usia  |
| ----- | ----- | ---------------- | ----- |
| 10010 | Robin | Direktur         | 45    |
| 10011 | Tari  | Bendahara        | 38    |
| 10012 | Wawan | Satpam           | 29    |
| 10013 | Aswar | Cleaning service | 25    |
| 10014 | Ira   | Hrd              | 40    |
 
==Penjelasan tabel ==
- id : Kunci primer yang mengidentifikasi secara unik setiap karyawan.
- nama : Kolom yang menyimpan nama karyawan.
- posisi/jabatan : Kolom yang menyimpan informasi departemen tempat karyawan bekerja.
- usia : kolom yang menyimpan umur karyawan 

---
# INSTALASI DAN QUERY AWAL DATABASE 

---
# ==Instalasi MySQL==
## menggunakan termux

1. Buka termux
2. Ketik termux-setup-storage lalu Berikan akses termux ke memori internal
3. Muncul pop-up untuk meminta izin akses ke memori internal klik izinkan/allow acces
4. Lakukan update dan sekaligus upgrade paket dengan mengetik **pkg update && upgrade** lalu klik y
5. Jika ada konfirmasi untuk melanjutkan instalasi. Silahkan **klik y dan enter**
6. Instal aplikasi mariadb dengan mengetik  **pkg install mariadb**
7. Memberikan akses aman ke MySQL dengan mengetik **mysql_safe**
8. Hentikan proses dengan **CTRL+Z**
9. Masuk kedalam admin dengan mengetik **MySQL -u root**
## referensi video YouTube

https://youtu.be/ez3nx3xH-y4?si=T4saycipqfBcqL1c

---
# ==Penggunaan awal MySQL==
## Query/struktur 

```MySQL
MySQL -u root
```

## Hasil
![MySQL -u root](2.1.jpg)

## Analisis 
==MySQL== adalah perintah untuk mengakses Shell MySQL, yaitu antarmuka command line untuk berinteraksi dengan server MySQL

=="-u root"== adalah opsi yang digunakan saat Anda mengakses MySQL dari baris perintah (command line). Di sini, "-u" adalah singkatan dari "user", dan "root" adalah nama pengguna. Dengan menggunakan "-u root", Anda masuk ke MySQL sebagai pengguna "root", yang biasanya memiliki hak akses penuh ke semua fungsi MySQL. Pengguna "root" sering digunakan untuk melakukan tugas administratif dan konfigurasi yang memerlukan tingkat akses tertinggi.

>[! summary ] Kesimpulan 
 ==MySQL -u root== adalah bahwa Anda mengakses server MySQL dengan menggunakan opsi "-u" untuk menentukan pengguna (dalam hal ini, "root" yang merupakan pengguna dengan hak akses tertinggi). Dengan menggunakan "root", Anda memiliki kemampuan untuk melakukan tugas administratif dan konfigurasi yang memerlukan tingkat akses penuh ke server MySQL. 


---
# ==Database==
## CREATE DATABASE 
### Struktur :
``` MySQL
CREATE DATABASE [nama_database];
```
### Contoh :
```MySQL
CREATE DATABASE Taufiq;
```
### Hasil 
![Create database](2.2.jpg)

### Analisis :
- `CREATE DATABASE` adalah sebuah query yang memerintahkan untuk membuat database.
- `taufiq` adalah nama dari suatu database yang kita buat

>[! summary ] Kesimpulan
>query atau kode tersebut memerintahkan untuk membuat suatu database yang bernama `taufiq`


---
## TAMPILKAN DATABASE
### Struktur :
```MySQL
SHOW DATABASES;
```

### Contoh :
```MySQL
SHOW DATABASES;
```

### Hasil :
![Show databases](2.3.jpg)
### Analisis :
- `SHOW DATABASE` merupakan query untuk menampilkan sebuah database dalam MySQL

>[! summary ] Kesimpulan
> `SHOW DATABASE` Suatu kode atau query yang berguna untuk menampilkan database yang sudah dibuat

---
## HAPUS DATABASE 
### Struktur
```MySQL
DROP DATABASE [nama_database];
```

### Contoh 
```MySQL
DROP DATABASE [xi_rpl_1];
```

### Hasil :
![Drop database](2.4.jpg)

### Analisis
- `DROP DATABASE` Merupakan perintah query untuk menghapus database
- `taufiq` nama dari database yang ingin kita hapus

>[! summary ] Kesimpulan 
>Untuk menghapus database kita bisa gunakan perintah `DROP DATABASE` 

---
## GUNAKAN DATABASE 

### Struktur
```MySQL
USE [nama_database];
```

### Contoh
```MySQL
USE xi_rpl_1;
```

### Hasil
![Use database](Aset/2.5.jpg)
### Analisis 
- `USE` adalah perintah untuk masuk kedalam database
- `xi_rpl_1` merupakan nama database yang ingin kita gunakan atau masuki

>[! summary ] Kesimpulan
Jika ingin masuk atau gunakan database, maka kita gunakan `USE` sebagai query 

---
# ==Tipe Data==
## ANGKA

-  ==INT:== Untuk menyimpan nilai bilangan bulat (integer). Misalnya, INT dapat digunakan untuk menyimpan angka seperti 1, 100, -10, dan sebagainya.

 - ==DECIMAL: ==Digunakan untuk menyimpan nilai desimal presisi tinggi, cocok untuk perhitungan finansial atau keuangan.
 
 - ==FLOAT dan DOUBLE: ==Digunakan untuk menyimpan nilai desimal dengan presisi floating-point. DOUBLE memiliki presisi lebih tinggi dibandingkan FLOAT.
 
 - ==TINYINT, SMALLINT,== ==MEDIUMINT==, dan ==BIGINT: ==Tipe data ini menyimpan bilangan bulat dengan ukuran yang berbeda-beda.
### Contoh 
```MySQL

CREATE TABLE contoh_tabel (
    id INT,
    harga DECIMAL(10, 2),
    jumlah_barang TINYINT
);
```

### Hasil
![Tipe data angka](Aset/2.6.jpg)

>[! summary ] Kesimpulan 
Dalam contoh tersebut, ==**id**== menggunakan tipe data ==**INT**==, ==**harga**== menggunakan tipe data ==**DECIMAL**== dengan presisi 10 digit dan 2 angka di belakang koma, dan ==**jumlah_barang**== menggunakan tipe data ==**TINYINT**==

---
## TEXT

- ==CHAR(N) ==Menyimpan string karakter tetap dengan panjang N. Contoh: ==CHAR(10) ==akan menyimpan string dengan panjang tepat 10 karakter.

- ==VARCHAR(N):== Menyimpan string karakter dengan panjang variabel maksimal N. Misalnya, ==VARCHAR(255) ==dapat menyimpan string hingga 255 karakter, tetapi sebenarnya hanya menyimpan panjang yang diperlukan plus beberapa overhead.

- ==TEXT: ==Digunakan untuk menyimpan teks dengan panjang variabel, tanpa batasan panjang tertentu. Cocok untuk data teks yang panjangnya tidak terduga.
### Contoh
```MySQL
CREATE TABLE adiguna_tabel (
    nama CHAR(50),
    alamat VARCHAR(100),
    catatan TEXT,
);
```

### Hasil
![Tipe data Text](Aset/2.7.jpg)

>[! summary ] Kesimpulan 
Dalam contoh tersebut, ==**nama**== menggunakan tipe data ==**char**== dengan panjang tetap, ==**alamat**== menggunakan tipe data ==**VARCHAR**== dengan panjang variabel, **catatan** menggunakan tipe data ==**TEXT**== untuk menyimpan teks yang mungkin panjangnya bervariasi, dan **status** menggunakan tipe data ==**ENUM**== untuk membatasi nilai yang mungkin.

---
## TANGGAL

- ==DATE== :  Menyimpan nilai tanggal dengan format YYYY-MM-DD.

- ==TIME==: Menyimpan nilai waktu dengan format HH:MM:SS.

- ==DATETIME: ==Menggabungkan nilai tanggal dan waktu dengan format YYYY-MM-DD HH:MM:SS

- ==TIMESTAMP: ==Sama seperti DATETIME, tetapi dengan kelebihan diatur secara otomatis saat data dimasukkan atau diubah.
### Contoh
```MySQL
CREATE TABLE Taufiq_tabel (
    tanggal DATE,
    waktu TIME,
    datetimekolom DATETIME,
    timestampkolom TIMESTAMP
);
```

### Hasil
![Tipe data tanggal](Aset/2.8.jpg)

>[! summary ] Kesimpulan 
Dalam contoh ini, kolom **==tanggal==** akan menyimpan nilai tanggal, **==waktu==** menyimpan nilai waktu, ==**datetimekolom**== menyimpan kombinasi tanggal dan waktu, dan **==timestampkolom==** akan secara otomatis diatur saat data dimasukkan atau diubah.

---
## BOOLEAN 

Boolean adalah tipe data yang hanya memiliki dua nilai: true atau false. Ini digunakan untuk menyatakan kebenaran suatu kondisi atau pernyataan. Dalam banyak bahasa pemrograman, termasuk SQL, boolean digunakan untuk pengambilan keputusan dan pengendalian alur program.

```MySQL
CREATE TABLE contohTabel (
    title VARCHAR(255),
    completed BOOLEAN
);```

 Dalam contoh diatas, kita mendefinisikan kolom **==completed==** sebagai tipe data ==**BOOLEAN**==. Ini merupakan cara yang sah dan umum digunakan di MySQL. Nilai yang dapat disimpan dalam kolom ini adalah **==TRUE==** atau ==**FALSE**==, atau dalam representasi angka, 1 atau 0.

---
# ==Tipe Data Pilihan ==
## ENUM
### Penjelasan 
Dalam MySQL, ENUM adalah tipe data khusus yang memungkinkan Anda mendefinisikan sebuah kolom yang dapat mengandung satu dari beberapa nilai konstan yang telah ditentukan. Ini memberikan cara yang efisien untuk menyimpan dan memvalidasi nilai dalam kolom.
### Contoh
```MySQL
CREATE TABLE ExampleTable (
    id INT PRIMARY KEY,
    status ENUM('Active', 'Inactive', 'Pending') NOT NULL
);

```

### Hasil
![Tipe data pilihan enum](Aset/2.9.jpg)

>[! summary ] Kesimpulan
status adalah kolom dengan tipe data ENUM yang dapat berisi nilai 'Active', 'Inactive', atau 'Pending'. Dengan menggunakan ENUM, Anda membatasi kolom tersebut hanya menerima nilai-nilai yang telah ditentukan, mengurangi kemungkinan kesalahan input dan meningkatkan kejelasan dalam struktur data tabel.

---
## SET
tipe data SET digunakan untuk mendefinisikan sebuah kolom yang dapat memiliki satu atau beberapa nilai dari sekumpulan nilai yang telah ditentukan. Nilai-nilai dalam tipe data SET disimpan sebagai himpunan tanpa urutan tertentu, dan setiap nilai hanya dapat muncul satu kali.
### Contoh
```MySQL
CREATE TABLE Set_tabel(
    id INT PRIMARY KEY,
    preferences SET('Email', 'SMS') NOT NULL
);
```

### Hasil
![Tipe data set](Aset/2.10.jpg)

>[! summary ] kesimpulan
>Preferences ada kolom dengan tipe data set yang terdapat 2 pilihan didalam nya yaitu Email dan SMS


---
# ==TABLE==
## BUAT TABLE
### Struktur
```MySQL
CREATE TABLE nama_tabel (
 Namakolom tipedata(lebar) cons,
 Namakolom tipedata(lebar) cons,
 Namakolom tipedata(lebar) cons,
);
```
### Contoh :
``` MySQL
Create table daftar_siswa;
Id int primary key,
Nama varchar(255),
Umur int,
Alamat text
);
```

### Hasil
![Create table](Aset/2.11.jpg)

### Analisis :
- `CREATE TABLE` Digunakan untuk membuat tabel
- `daftar_siswa` nama dari tabel yang ingin kita buat
- `id`: Kolom untuk menyimpan ID sebagai kunci utama (Primary Key).
- `Primary key`  merupakan kunci unik yg ada pada tabel dan hanya 1 setiap tabelnya
- `nama`: Kolom untuk menyimpan nama dengan tipe data VARCHAR (teks dengan panjang variabel).
- `umur`: Kolom untuk menyimpan umur dengan tipe data INT (bilangan bulat).
- `alamat`: Kolom untuk menyimpan alamat dengan tipe data TEXT (teks dengan panjang variabel).

>[!Summary] Kesimpulan 
> CREATE TABLE daftar_siswa; digunakan untuk membuat suatu tabel yg ingin digunakan untuk menampung daftar siswa sesuai dengan namanya yaitu daftar_siswa.

---
## TAMPILKAN STRUKTUR TABLE

### Struktur 
``` MySQL
DESC nama_tabel;
```

### Contoh Desc Tabel :
``` MySQL
Desc daftar_siswa;
```
### Contoh Hasil :
![Tampilkan Struktur tabel](Aset/2.12.jpg)
### Analisis Desc Tabel :
- `Desc` berfungsi memberikan informasi kolom-kolom dalam tabel yang di buat, termasuk nama kolom, tipe data,serta  penggunaan null dalam kolom itu bisa terlihat di Desc Tabel.
- `Daftar_siswa;` merupakan sebuah nama tabel  ingin di lihat strukturnya.

>[! summary ] kesimpulan 
>jika kita ingin melihat tipe data yang ada pada kolom-kolom tabel, kita dapat menampilkan nya dengan Desc [nama_tabel]

---
## MENAMPILKAN DAFTAR TABLE
### Struktur
``` MySQL
SHOW TABLES;
```

### Contoh Show tables :
``` MySQL
SHOW TABLES;
```

### Hasil Show tables :
![daftar table](Aset/2.13.jpg)

### Analisis 
- `SHOW TABLES` digunakan untuk memanggil tabel-tabel yang sudah dibuat dalam database rental_taufiq
- dalam database rental_taufiq terdapat 2 table yang bernama daftar_siswa dan pelanggan 


>[! summary ] kesimpulan 
>jika ingin mengetahui ada berapa tabel yang sudah dibuat dalam suatu database kita dapat menggunakan Query `SHOW TABLES`;

---
## QNA

>[!faq] 1
Mengapa hanya kolom id_pelanggan yang menggunakan constraint primary key?

>[!note] jawaban 
>Karna hanya kolom id_pelanggan yang memiliki id unik, yang tidak ada samanya dengan baris lain dalam tabel, sehingga kita pilih id_pelanggan sebagai primary key

>[!faq] 2
>mengapa pada kolom no_telp yang menggunakan tipe data char bukan varchar?

>[!note] Jawaban
> Karna tipe data char merupakan tipe data yang menetapkan panjang karakter, seperti yang di ketahui no_telp memiliki panjang yang tetap maka dari itu kita menggunakan tipe data char, karna jika tipe data varchar digunakan untuk text yang panjang

>[!faq] 3
>mengapa hanya kolom no_telp yang menggunakan constraint unique?

>[!note] Jawaban
>karna setiap pelanggan mempunyai no_telp masing" yang artinya nomornya pasti berbeda, maka dari itu kita pake unique agar setiap pelanggan memasukkan nomor telepon nya sendiri 

>[!faq] 4
>mengapa kolom no_telp tidak memakai constraint Not null, sementara kolom lainnya menggunakan constraint tersebut?

>[!note ] Jawaban 
>berarti dalam tabel tersebut no_telp hanya opsional saja dan tidak wajib di isi/bisa dikosongkan 

>[!faq] 5 
>perbedaan primary key dan unique

>[!Note] Jawaban 
>Dalam `primary key` hanya boleh 1 setiap tabelnya, sedangkan unique bisa lebih dari 1.
>`primary key `bertujuan mengidentifikasi secara unik setiap baris dalam tabel, sedangkan `unique` Berfungsi untuk memastikan bahwa tidak ada dua baris dalam tabel yang memiliki nilai yang sama pada kolom yang memiliki constraint `UNIQUE`.


---
# ==Insert==
## INSERT 1 DATA
### Struktur
```MySQL
INSERT INTO [nama_tabel]
VALUES (nilai1,nilai2, nilai3,....);
```
### Contoh 
```MySQl
INSERT INTO pelanggan
VALUES (123,"TAUFIQ","ADIGUNA","1234567890");
```

### Hasil :
![Insert 1 data](Aset/2.14.jpg)

### Analisis
- `INSERT INTO` Query awal untuk menambahkan data di dalam tabel
- `pelanggan` merupakan nama tabel yang ingin kita masukkan data kedalamnya
- `VALUES (123,"TAUFIQ","ADIGUNA","1234567890");` merupakan nilai yang ingin kita masukkan kedalam kolom-kolom yang sudah ada pada tabel pelanggan

>[! summary ] Kesimpulan
>Jika ingin menambahkan nilai dalam tabel, kita bisa menggunakan perintah `INSERT`

---
## INSERT >1 DATA
### Struktur 
```MySQL
INSERT INTO [nama_table]
VALUES (kolom1,kolom2,kolom3,kolom4),
	   (kolom1,kolom2,kolom3,kolom4),
	   (kolom1,kolom2,kolom3,kolom4),

```
### Contoh
``` MySQL
INSERT INTO pelanggan
VALUES  
	(124, "ALFAHREZI", "RAIHAN", "0812345678"),
    (125, "FARID", "WIBOWO", "9876543210"),
    (126, "SITI", "RAHMA", "5678901234");
```
### Hasil
![Insert >1 data](Aset/2.15.jpg)
### Analisis 
- `INSERT INTO` Query awal untuk menambahkan data di dalam tabel
- `pelanggan` merupakan nama tabel yang ingin kita masukkan data kedalamnya
- `VALUES`  
	`(124,"ALFAHREZI","RAIHAN","0812345678"`
    `(125, "FARID", "WIBOWO", "9876543210"),`
    `(126, "SITI", "RAHMA", "5678901234");`
    Nilai yang akan kita masukkan kedalam tabel lebih dari 1 data.

>[! summary ] Kesimpulan 
>jika ingin menambahkan data lebih dari 1 kita bisa menggunakan metode seperti ini

---
## MENYEBUT KOLOM
### Struktur 
```MySQL
INSERT INTO [nama_tabel]
(Kolom1,kolom2,kolom3,..)
VALUES (nilai1,nilai2,nilai3,...)
```
### Contoh
```MySQL
INSERT INTO pelanggan
       (id,nama_depan,nama_belakang)
VALUES (127,"ZHAFRAN","RIZKI");
```
### Hasil
![Menyebut kolom](Aset/2.16.jpg)

### Analisis
- `INSERT INTO` Query awal untuk menambahkan data di dalam tabel
- `pelanggan` merupakan nama tabel yang ingin kita masukkan data kedalamnya
- `(id,nama_depan,nama_belakang`) merupakan kolom pilihan yang ingin kita tambahkan data kedalamnya
- `VALUES (127,"ZHAFRAN","RIZKI");` data yang akan kita masukkan kedalam tabel sesuai dengan kolom yang sudah di tentukan 

>[! summary ] Kesimpulan 
>Untuk menambahkan data di kolom tertentu kita harus memanggil kolom yang ingin kita tambahkan data didalamnya terlebih dahulu Setelah itu data-data apa yang ingin kita masukkan 

---
# ==SELECT==
## SELURUH DATA
### Struktur 
```MySQL
SELECT * FROM [nama_tabel];
```
### Contoh
``` MySQL
SELECT * FROM pelanggan;
```
### Hasil
![Seluruh data](Aset/2.17.jpg)
### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan Data pada tabel database.
- `*` digunakan jika ingin mengambil/menampilkan semua kolom
- `FROM pelanggan` Merupakan nama tabel yang ingin di tampilkan 

>[! summary ] Kesimpulan 
>untuk mengambil semua data di tabel, kita bisa menggunakan `Query` dengan kata kunci `SELECT * FROM`

---
## DATA KOLOM TERTENTU 
### Struktur
``` MySQL
SELECT [nama_kolom1], [nama_kolom2], [nama_kolom3],... [nama_kolom_n],
FROM [nama_tabel];
```
### Contoh 
```MySQL

SELECT nama_depan,no_telp FROM pelanggan;
```
### Hasil
![kolom tertentu](Aset/2.18.jpg)

### Analisis
- `SELECT nama_depan,no_telp` query untuk menampilkan kolom nama depan dan no telp 
- `FROM pelanggan` merupakan nama tabel yang ingin kita tampilkan kolom nama depan dan no telp

>[! summary ] Kesimpulan
>Jika ingin menampilkan kolom-kolom tertentu atau yang di inginkan kita bisa gunakan perintah `SELECT nama_kolom FROM pelanggan`

---
## KLAUSA WHERE
### Struktur 
```MySQL
SELECT * FROM [nama_tabel] 
WHERE [nama_kolom] = [nilai];

```

>[!faq] Format kondisi
 `nama kolom` : seperti id,nama_depan,no_telp
 `operator` : seperti `=,>,>=,<,<=,!=<>,dst`
 `nilai` : seperti pada id 123 
### Contoh
``` MySQL
SELECT * FROM pelanggan
WHERE id=123;
```
### Hasil
![klausa where](Aset/2.19.jpg)
### Analisis
- `SELECT * FROM pelanggan` merupakan query untuk menampilkan tabel pelanggan 
- `WHERE id=123;` adalah perintah untuk menampilkan sebuah baris yang memiliki id 123 

>[! summary ] Kesimpulan
>Jika ingin mencari data tertentu yang ada pada tabel kita bisa gunakan `WHERE [nama_kolom] = [nilai]`


---
# ==Update==
## Struktur
```MySQL
UPDATE [nama_tabel]
SET [nama_kolom] = "nilai"
WHERE [nama_kolom] = "nilai";
```

## Contoh
```MySQL
UPDATE pelanggan
Set no_telp  = "085340305553"
WHERE id=123;

```

## Hasil
![Update](Aset/2.20.jpg)

## Analisis
- `Update`  merupakan query untuk mengupdate data dalam kolom
- `pelanggan` adalah nama dari database yang ingin di ubah
- `SET` digunakan untuk mengubah nilai kolom pada sebuah baris data.
- `no_telp = "085340305553"` no_telp nama Kolom yang ingin di ubah nilainya menjadi `085340305553` sebagai nilai yang baru

>[! Summary ] Kesimpulan 
>jika ingin mengganti atau update data pada kolom kita bisa gunakan query `UPDATE nama_table SET nama_kolom = value`

---
# ==DELETE BARIS==
## Struktur
```MySQL
DELETE FROM [nama_tabel]
WHERE [nama_kolom] = [nilai];
```
## Contoh
```MySQL
DELETE FROM pelanggan
WHERE id = "127";
```
## Hasil
![Delete baris](2.21.jpg)

## Analisis
- `DELETE` Merupakan perintah query untuk menghapus 
- `FROM PELANGGAN` Merupakan nama tabel yang ingin kita hapus datanya
- `WHERE id="127";` Query untuk menghapus baris pada tabel pelanggan yang memiliki `id=127`

>[! summary ] Kesimpulan
> Jika ingin menghapus suatu baris tertentu pada tabel kita dapat gunakan query `DELETE FROM [nama_tabel]
WHERE [nama_kolom] = [nilai];`

---
# ==DELETE TABEL==
## Struktur 
```MySQL
DROP TABLE [nama_tabel];
```

## Contoh 
``` MySQL
DROP TABLE penerima_pip;
```

## Hasil
![delete tabel](Aset/2.22.jpg)

## Analisis
- `DROP TABLE`Merupakan query untuk menghapus sebuah tabel.
- `penerima_pip` nama tabel yang ingin kita hapus.
 
>[! summary ] kesimpulan 
>ketika ingin menghapus sebuah tabel dalam database, kita dapat gunakan perintah query `DROP TABLE [nama_tabel];`



