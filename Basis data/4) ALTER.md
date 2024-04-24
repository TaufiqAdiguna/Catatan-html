# Struktur Awal Tabel
![Hasil](Aset/4.1.jpg)

---
# Menambahkan Kolom
## Struktur Query 
```mysql

ALTER TABLE [nama_tabel] ADD [nama_kolom_baru]
[type_data] [posisi_dalam_tabel] [nama_kolom]
```
## Contoh 
```MySQL
ALTER TABLE mobil ADD batas_peminjaman varchar(10) AFTER peminjam;
```
## Hasil
![hasil](Aset/4.2.jpg)
## Analisis 
## Kesimpulan 

## Tambahan 
### Struktur Query

![hasil ](Aset/4.3.jpg)
### Penjelasan 

---
# Mengubah Nama Kolom
## Struktur Query 
```mysql
ALTER TABLE [nama_tabel]
  RENAME COLUMN [nama_kolom_sebelumnya] TO       [nama_kolom_baru];
```
## Contoh
```mysql
ALTER TABLE mobil
 RENAME COLUMN batas_peminjaman TO deadline;
```
## Hasil
![hasil](Aset/4.4.jpg)
## Analisis 
## Kesimpulan 

---
# Mengubah Tipe data kolom
## Struktur Query 
```mysql

ALTER TABLE [nama_tabel] MODIFY [nama_kolom] [tipe_data];
```

## Contoh
```mysql
ALTER TABLE mobil MODIFY deadline DATE;
```
## Hasil
![hasil](Aset/4.5.jpg)
## Analisis 
## Kesimpulan 

---
# Menambahkan Constraint
## Struktur Query 
## Contoh
```mysql
ALTER TABLE mobil
  ALTER deadline
```
## Hasil
![hasil](Aset/4.6.jpg)
## Analisis 
## Kesimpulan 

## Tambahan 
### Struktur Query 
```mysql
INSERT INTO mobil
(id_mobil,no_plat,no_mesin,warna,pemilik,
 peminjam,harga_rental)
VALUES (7,"DD 5678 GH","GFD8906","Hitam",
"zhafran",NULL,150000);
```
### Hasil
![hasil](Aset/4.7.jpg)
## Referensi 
https://revou.co/panduan-teknis/sql-constraint

---
# Menghapus Constraint 
## Struktur Query 
## Contoh 
## Hasil
## Analisis 
## Kesimpulan 

## Referensi 
https://www.geeksforgeeks.org/sql-drop-constraint/


---

## Struktur Query 
## Contoh 
## Hasil
## Analisis 
## Kesimpulan 

---

## Struktur Query 
## Contoh 
## Hasil
## Analisis 
## Kesimpulan 