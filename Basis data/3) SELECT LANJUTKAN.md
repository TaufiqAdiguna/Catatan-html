
# AND

## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [Kondisi 1] AND [Kondisi 2];
```

## Contoh
```MySQL
SELECT * FROM mobil
WHERE warna = "Merah" AND Pemilik ="Taufiq";
```
``
## Hasil
![[Basis data/Aset/3.1.jpg]]

## Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` : nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `warna = "Merah" AND Pemilik ="Taufiq";` : terdapat 2 kondisi yang harus di penuhi untuk menampilkan sebuah data. Hanya baris dengan nilai kolom "warna" yang sama dengan "Merah" yang akan dipertimbangkan.di kondisi 2, baris tersebut juga harus memiliki nilai kolom "Pemilik"  sama dengan "Taufiq". Klausa AND memastikan bahwa kedua kondisi harus terpenuhi secara bersamaan agar bisa tampil.

## Kesimpulan
Perintah MySQL tersebut mengambil/manampilkan semua kolom dari tabel di mana warna adalah "Merah" dan pemilik adalah "Taufiq".

---
# OR
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [Kondisi 1] OR [Kondisi 2];
```

## Contoh
```MySQL
SELECT * FROM mobil
WHERE warna = "Merah" OR Pemilik ="adiguna";
```

## Hasil
![[3.2.jpg]]

## Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `WHERE warna = "Merah" OR Pemilik = "adiguna";`: Menetapkan kondisi untuk pengambilan data. dimana jika salah satu Baris yang memenuhi dari dua kondisi ini tersebut akan diambil/ditampilkan.

## Kesimpulan
digunakan untuk mengambil semua kolom dari tabel `mobil` di mana nilai kolom `warna` adalah `Merah` atau nilai kolom `Pemilik` adalah `adiguna`. Hasilnya akan mencakup data yang memenuhi salah satu dari dua kondisi tersebut.

---
# BETWEEN
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] BETWEEN [nilai] AND [nilai];

```

## Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental BETWEEN 100000 AND 150000;
```

## Hasil
![[3.3.jpg]]

## Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental BETWEEN 100000 AND 150000;`: dimana query tersebut memerintahkan untuk mengambil data Kolom `harga_rental` dari `100000` Sampai dengan `150000`.

## Kesimpulan 
Perintah MySQL tersebut akan  mengambil data dari tabel "mobil" dengan rentang harga sewa antara 100,000 dan 150,000.

---
# NOT BETWEEN
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] NOT BETWEEN [nilai_1] AND [nilai_2];
```

## Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental NOT BETWEEN 100000 AND 150000;
```
## Hasil
![[3.4.jpg]]

## Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental NOT BETWEEN 100000 AND 150000;` :  data yang harga_rental nya diluar dari 100000 sampai dengan 150000 yang akan di ambil

## Kesimpulan
Perintah MySQL tersebut akan mengambil data dari tabel "mobil" di mana harga sewa tidak berada dalam rentang/diluar 100,000 hingga 150,000.

---
# <=
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] <= [nilai];
```

## Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental <= 100000;
```
## Hasil
![[3.5.jpg]]

## Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental <= 100000;` : akan menampilkan sebuah data yang hanya memiliki nilai harga_rental kurang dari `100000` atau sama dengan.

## Kesimpulan 
Perintah MySQL tersebut akan menampilkan sebuah data tabel mobil dimana harga_rentalnya berada di bawah dari `100000` atau sama dengan.

---
# >=

## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] >= [nilai];
```
## Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental >= 100000;
```
## Hasil
![[3.6.jpg]]

## Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental >= 100000;` : akan menampilkan sebuah data dari kolom harga_rental yang bernilai lebih besar dari `100000` atau sama dengan.

## Kesimpulan
Perintah MySQL tersebut akan menampilkan sebuah data tabel mobil dimana harga_rentalnya berada di atas `100000` atau sama dengan.

---
# <> atau =!
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] <> [nilai];
```

## Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental <> 100000;
```

### Hasil
![[3.7.jpg]]

## Analisis 

## Kesimpulan 

---
# Tantangan
## Struktur
## Contoh 
## Hasil 
![[3.8.jpg]]

## Analisis 

## Kesimpulan

---
# IN
## Struktur Query
```MySQL

SELECT * FROM [nama_tabel] WHERE [nama_kolom] IN('nilai');

```

## Contoh 
```MySQL
SELECT * FROM mobil WHERE warna IN('Hitam','Merah');
```

## Hasil
![SELECT IN](Aset/3.9.jpg)

## Analisis

## Kesimpulan 

---
# IN & AND
## Struktur Query
```MySQL

SELECT * FROM [nama_tabel]
 WHERE [nama_kolom] IN ('nilai')
 AND [nama_kolom] = nilai;

```

## Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     AND harga_rental = 50000;
```

## Hasil
![SELECT IN & AND](Aset/3.10.jpg)

## Analisis
## Kesimpulan

---
# IN & OR
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
    WHERE [nama_kolom] IN ('nilai')
    OR [nama_kolom] = nilai;
```

## Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     OR harga_rental = 150000;
```

## Hasil
![SELECT IN & OR](Aset/3.11.jpg)

## Analisis
## Kesimpulan

---
# IN + AND + OPERATOR 

---
# OPERATOR LEBIH BESAR 

## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] IN ('nilai')
     AND [nama_kolom] > nilai;
```

## Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     AND harga_rental > 50000;
```

## Hasil
![SELECT OPERATOR LEBIH BESAR](Aset/3.12.jpg)

## Analisis
## Kesimpulan

---
# OPERATOR LEBIH KECIL
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] IN ('nilai')
     AND [nama_kolom] > nilai;
```

## Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     AND harga_rental < 1000000;
```

## Hasil
![SELECT OPERATOR LEBIH KECIL](Aset/3.13.jpg)

## Analisis
## Kesimpulan

---
# LIKE

---
## MENCARI AWALAN
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] LIKE 'nilai%';
```

## Contoh
```MySQL
SELECT * FROM mobil
     WHERE pemilik LIKE 'T%';
```

## Hasil
![MENCARI AWALAN](Aset/3.14.jpg)

## Analisis
## Kesimpulan

---
## MENCARI AKHIRAN
## Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] LIKE 'nilai%';
```

## Contoh
```MySQL
SELECT * FROM mobil
     WHERE pemilik LIKE '%a';
```

## Hasil
![MENCARI AKHIRAN](Aset/3.15.jpg)

## Analisis
## Kesimpulan

---
