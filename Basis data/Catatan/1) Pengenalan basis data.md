
# definisi basis data
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
#  peran basis data
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

 
