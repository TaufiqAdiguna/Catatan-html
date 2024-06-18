
# OPERATOR LOGIKA DAN PEMBANDING 

## AND

### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [Kondisi 1] AND [Kondisi 2];
```

### Contoh
```MySQL
SELECT * FROM mobil
WHERE warna = "Merah" AND Pemilik = "Taufiq";
```

### Hasil
![And](Aset/3.1.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` : nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `warna = "Merah" AND Pemilik ="Taufiq";` : terdapat 2 kondisi yang harus di penuhi untuk menampilkan sebuah data. Hanya baris dengan nilai kolom "warna" yang sama dengan "Merah" yang akan dipertimbangkan.di kondisi 2, baris tersebut juga harus memiliki nilai kolom "Pemilik"  sama dengan "Taufiq". Klausa AND memastikan bahwa kedua kondisi harus terpenuhi secara bersamaan agar bisa tampil.

### Kesimpulan
Perintah MySQL tersebut mengambil/manampilkan semua kolom dari tabel di mana warna adalah "Merah" dan pemilik adalah "Taufiq".

---
## OR
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [Kondisi 1] OR [Kondisi 2];
```

### Contoh
```MySQL
SELECT * FROM mobil
WHERE warna = "Merah" OR Pemilik ="adiguna";
```

### Hasil
![OR](Aset/3.2.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `WHERE warna = "Merah" OR Pemilik = "adiguna";`: Menetapkan kondisi untuk pengambilan data. dimana jika salah satu Baris yang memenuhi dari dua kondisi ini tersebut akan diambil/ditampilkan.

### Kesimpulan
digunakan untuk mengambil semua kolom dari tabel `mobil` di mana nilai kolom `warna` adalah `Merah` atau nilai kolom `Pemilik` adalah `adiguna`. Hasilnya akan mencakup data yang memenuhi salah satu dari dua kondisi tersebut.

---
## BETWEEN
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] BETWEEN [nilai] AND [nilai];

```

### Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental BETWEEN 100000 AND 150000;
```

### Hasil
![BETWEEN](Aset/3.3.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental BETWEEN 100000 AND 150000;`: dimana query tersebut memerintahkan untuk mengambil data Kolom `harga_rental` dari `100000` Sampai dengan `150000`.

### Kesimpulan 
Perintah MySQL tersebut akan  mengambil data dari tabel "mobil" dengan rentang harga sewa antara 100,000 dan 150,000.

---
## NOT BETWEEN
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] NOT BETWEEN [nilai_1] AND [nilai_2];
```

### Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental NOT BETWEEN 100000 AND 150000;
```
### Hasil
![NOT BETWEEN](Aset/3.4.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental NOT BETWEEN 100000 AND 150000;` :  data yang harga_rental nya diluar dari 100000 sampai dengan 150000 yang akan di ambil

### Kesimpulan
Perintah MySQL tersebut akan mengambil data dari tabel "mobil" di mana harga sewa tidak berada dalam rentang/diluar 100,000 hingga 150,000.

---
## <=
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] <= [nilai];
```

### Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental <= 100000;
```
### Hasil
![LEBIH KECIL SAMA DENGAN](Aset/3.5.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental <= 100000;` : akan menampilkan sebuah data yang hanya memiliki nilai harga_rental kurang dari `100000` atau sama dengan.

### Kesimpulan 
Perintah MySQL tersebut akan menampilkan sebuah data tabel mobil dimana harga_rentalnya berada di bawah dari `100000` atau sama dengan.

---
## >=

### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] >= [nilai];
```
### Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental >= 100000;
```
### Hasil
![LEBIH BESAR SAMA DENGAN](Aset/3.6.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental >= 100000;` : akan menampilkan sebuah data dari kolom harga_rental yang bernilai lebih besar dari `100000` atau sama dengan.

### Kesimpulan
Perintah MySQL tersebut akan menampilkan sebuah data tabel mobil dimana harga_rentalnya berada di atas `100000` atau sama dengan.

---
## <> atau =!
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
WHERE [nama_kolom] <> [nilai];
```

### Contoh
```MySQL
SELECT * FROM mobil
WHERE harga_rental <> 100000;
```

### Hasil
![TIDAK SAMA DENGAN](Aset/3.7.jpg)

### Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `harga_rental <> 100000;` : akan menampilkan sebuah data pada kolom `harga_rental` yang bukan `100000` nilainya

### Kesimpulan 
mengambil semua data dari tabel "mobil" kecuali  harga rental tidak sama dengan 100000. 


---
## TANTANGAN

### Struktur
```MySQL 
SELECT [nama_kolom] FROM [nama_tabel]
WHERE [nama_kolom] = [nilai];
```
### Contoh 
```MySQL
SELECT pemilik FROM mobil
WHERE id_mobil = 1;
```
### Hasil 
![TANTANGAN](Aset/3.8.jpg)

### Analisis 
- `SELECT` : digunakan untuk mengambil sebuah data pada tabel
- `pemilik` : nama dari kolom yang akan kita tampilkan
- `FROM mobil` :  merupakan nama tabel yang ingin kita ambil datanya
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `id_mobil = 1;` merupakan baris yang akan kita tampilkan yang memiliki id_mobil bernilai 1

### Kesimpulan
perintah SQL tersebut adalah mengambil/menampilkan pemilik mobil dengan ID 1 dari tabel "mobil".

---
## TANTANGAN LOGIN 
### Struktur 
```mysql
SELECT [nama_kolom] FROM [nama_tabel]
WHERE [nama_kolom] = [nilai];
```

### Contoh 
```mysql 
SELECT nama FROM akun 
WHERE id = 1;
```

### Hasil
![hasil](Aset/3.43.png)

### Analisis
- `SELECT` : digunakan untuk mengambil sebuah data pada tabel
- `nama` : nama dari kolom yang akan kita tampilkan
- `FROM akun` :  merupakan nama tabel yang ingin kita ambil datanya
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel
- `id = 1;` merupakan baris yang akan kita tampilkan yang memiliki id bernilai 1

### Kesimpulan
perintah SQL tersebut adalah mengambil/menampilkan nama yang memiliki  ID 1 dari tabel `akun`.

---
# IN

---
## IN
### Struktur Query
```MySQL

SELECT * FROM [nama_tabel] WHERE [nama_kolom] IN('nilai1','nilai2');

```

### Contoh 
```MySQL
SELECT * FROM mobil WHERE warna IN('Hitam','Merah');
```

### Hasil
![SELECT IN](Aset/3.9.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `warna IN('Hitam','Merah');` : Query tersebut menampilkan sebuah data pada tabel dimana kolom warna yang bernilai Hitam dan Merah akan di tampilkan.

### Kesimpulan 
Perintah MySQL tersebut Menyaring sebuah data pada tabel mobil dimana akan hanya menampilkan warna Hitam dan Merah.

---
## IN & AND
### Struktur Query
```MySQL

SELECT * FROM [nama_tabel]
 WHERE [nama_kolom] IN ('nilai')
 AND [nama_kolom] = nilai;

```

### Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     AND harga_rental = 50000;
```

### Hasil
![SELECT IN & AND](Aset/3.10.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- ` warna IN('Merah','silver') AND harga_rental = 50000;` : Query tersebut mencari dimana kolom warna yang hanya memiliki nilai Merah atau silver, dan kolom harga_rental bernilai 50000 yang akan tampil.
### Kesimpulan
Menggunakan operator AND, memastikan bahwa kedua kondisi/kolom harus benar untuk memilih baris yang akan diambil.

---
## IN & OR
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
    WHERE [nama_kolom] IN ('nilai')
    OR [nama_kolom] = nilai;
```

### Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     OR harga_rental = 150000;
```

### Hasil
![SELECT IN & OR](Aset/3.11.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- ` warna IN('Merah','silver') OR harga_rental = 150000;` : query tersebut mencari data pada kolom warna bernilai Merah dan silver atau kolom harga_rental yang bernilai 150000 yang akan ditampilkan.

### Kesimpulan
Menggunakan operator logika OR memastikan bahwa salah satu dari 2 kondisi/kolom tersebut memenuhi syarat akan diambil.

---
## IN + AND + OPERATOR 

---
### LEBIH BESAR 

#### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] IN ('nilai1','nilai2')
     AND [nama_kolom] > nilai;
```

#### Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     AND harga_rental > 50000;
```

#### Hasil
![SELECT OPERATOR LEBIH BESAR](Aset/3.12.jpg)

#### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `warna IN('Merah','silver') AND harga_rental > 50000;`: query tersebut mencari data pada kolom  warna yang bernilai Merah atau silver dengan kriteria harga_rental berada di atas 50000.

#### Kesimpulan
Query tersebut mencari data pada kolom warna yang bernilai Merah atau silver dan pada saat yang sama kolom harga_rental harus lebih besar dari 50000.

---
### LEBIH KECIL
#### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] IN ('nilai1','nilai2')
     AND [nama_kolom] > nilai;
```

#### Contoh
```MySQL
SELECT * FROM mobil
     WHERE warna IN('Merah','silver')
     AND harga_rental < 1000000;
```

#### Hasil
![SELECT OPERATOR LEBIH KECIL](Aset/3.13.jpg)

#### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `warna IN('Merah','silver') AND harga_rental < 50000;`: query tersebut mencari data pada kolom  warna yang bernilai Merah atau silver dengan kriteria harga_rental berada dibawah 100000.

#### Kesimpulan
Query tersebut mencari data pada kolom warna yang bernilai Merah atau silver dan pada saat yang sama kolom harga_rental berada dibawah 100000.

---
# LIKE

---
## MENCARI AWALAN
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] LIKE 'nilai%';
```

### Contoh
```MySQL
SELECT * FROM mobil
     WHERE pemilik LIKE 'T%';
```

### Hasil
![MENCARI AWALAN](Aset/3.14.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `pemilik LIKE 'T%';` : query tersebut mencari data pada kolom pemilik yang berawalan kata huruf T akan diambil.
### Kesimpulan
`SELECT * FROM mobil WHERE pemilik LIKE 'T%';`
: Query tersebut mencari data pada tabel mobil yang memiliki awalan kata huruf T pada kolom pemilik.

---
## MENCARI AKHIRAN
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
     WHERE [nama_kolom] LIKE 'nilai%';
```

### Contoh
```MySQL
SELECT * FROM mobil
     WHERE pemilik LIKE '%a';
```

### Hasil
![MENCARI AKHIRAN](Aset/3.15.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `pemilik LIKE '%a';` : Query tersebut mencari data pada kolom pemilik yang akhiran katanya adalah huruf a yang akan diambil 
### Kesimpulan
`SELECT * FROM mobil WHERE pemilik LIKE '%a';`
: Perintah query tersebut akan menampilkan sebuah data pada tabel mobil dimana kolom pemilik akhiran katanya huruf a.

---
## MENCARI AWALAN & AKHIRAN
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel]
   WHERE [nama_kolom] LIKE                            'nilai_awal%nilai_akhir';
```

### Contoh
```MySQL
SELECT * FROM mobil
   WHERE pemilik LIKE 'T%q';
```

### Hasil
![Mencari awalan & Akhiran](Aset/3.16.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `pemilik LIKE 'T%q';` : Perintah query tersebut akan menampilkan sebuah data pada kolom pemilik yang berawalan huruf T dan akhiran katanya q.
### Kesimpulan
`SELECT * FROM mobil WHERE pemilik LIKE 'T%q';`
: Perintah query tersebut mencari data pada tabel dimana kolom pemilik yang awalan katanya huruf T dan akhiran katanya q yang akan diambil.

---
## MENCARI BERDASARKAN TOTAL KARAKTER 

### Struktur Query 
``` MySQL
SELECT * FROM [nama_tabel]
   WHERE [nama_kolom] LIKE 'Nilai__';

SELECT * FROM [nama_tabel]
   WHERE [nama_kolom] LIKE 'underscore';
```

### Contoh
```MySQL
SELECT * FROM mobil
    WHERE pemilik LIKE 'T_____';

SELECT * FROM mobil
     WHERE warna LIKE '_____';
```

### Hasil
![HURUF AWALAN & total underscore](Aset/3.17.jpg)

![total underscore ](Aset/3.18.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `pemilik LIKE 'T_____';` : perintah query ini akan mencari data dimana kolom pemilik memiliki awalan kata huruf T serta panjang karakternya sebanyak 6.
- `warna LIKE '_____';` : perintah ini mencari data, dimana kolom warna yang memiliki jumlah karakter sebanyak 6 yang akan diambil.

### Kesimpulan
- `SELECT * FROM mobil WHERE pemilik LIKE 'T_____';` : perintah query tersebut akan mencari data pada tabel mobil, dimana kolom pemilik memiliki awalan kata T dan jumlah karakter sebanyak 6 yang akan diambil.
- `SELECT * FROM mobil WHERE warna LIKE '_____';` : dan kalau perintah query ini akan mencari data pada tabel mobil, dimana kolom warna memiliki jumlah karakter sebanyak 6 maka akan diambil.

---
## KOMBINASI
```MySQL
SELECT * FROM [nama_tabel]
    WHERE [nama_kolom] LIKE 'nilai%'

SELECT * FROM [nama_tabel]
    WHERE [nama_kolom] LIKE 'nilai%';

```

### Contoh
```MySQL
SELECT * FROM mobil
    WHERE pemilik LIKE '_d%';

SELECT * FROM mobil
    WHERE pemilik LIKE '__i%';
```
### Hasil
![kombinasi](Aset/3.19.jpg)

![kombinasi_2](Aset/3.20.jpg)
### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `pemilik LIKE '_d%';` : perintah ini akan mencari data pada kolom pemilik, dimana underscore nya sebagai pengganti karakter awal dan karakter keduanya bernilai d.
- `pemilik LIKE '__i%';` perintah ini akan mencari data pada kolom pemilik, yang dimana 2 underscore nya sebagai pengganti nilai asli dan karakter ketiganya bernilai i.
### Kesimpulan
- `SELECT * FROM mobil WHERE pemilik LIKE '_d%';` : Perintah query tersebut akan mencari data pada tabel mobil, dimana kolom pemilik yang bernilai d pada karakter keduanya akan diambil.
- `SELECT * FROM mobil WHERE pemilik LIKE '__i%';` : Perintah query tersebut akan mencari data pada tabel mobil, dimana kolom pemilik yang bernilai i pada karakter ketiga yang akan diambil.

---
## NOT LIKE
### Struktur Query 
```MySQL

SELECT * FROM [nama_tabel]
    WHERE [nama_kolom] NOT LIKE 'nilai%';
```

### Contoh
```MySQL
SELECT * FROM mobil
    WHERE pemilik NOT LIKE 'opi%';
```

### Hasil
![NOT LIKE](Aset/3.21.jpg)

### Analisis
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `pemilik NOT LIKE 'opi%';` : Perintah query ini tidak akan menampilkan yang bernilai Opi pada kolom pemilik
### Kesimpulan
`SELECT * FROM mobil WHERE pemilik NOT LIKE 'opi%';`: Jadi Perintah tersebut mengecualikan            sebuah data pada tabel mobil dimana kolom pemilik     yang bernilai Opi tidak akan ditampilkan.

---
# NULL & NOT NULL
## NULL
### Struktur Query 
```MySQL

SELECT * FROM [nama_tabel] WHERE [nama_kolom] IS NULL;
```

### Contoh 
```MySQL

SELECT * FROM mobil WHERE peminjam IS NULL;
```
### Hasil
![hasil](Aset/3.22.jpg)
### Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `peminjam IS NULL`pada kolom peminjam akan menampilkan data yang kosong.
### Kesimpulan 
Null digunakan ketika kita ingin menampilkan kolom yang kosong/belum ada isinya.

---
## NOT NULL
### Struktur Query 
```MySQL

SELECT * FROM [nama_tabel] WHERE [nama_kolom] IS NOT NULL;
```
### Contoh
```MySQL

SELECT * FROM mobil WHERE peminjam IS NOT NULL;
```
### Hasil
![hasil](Aset/3.23.jpg)
### Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE` :  digunakan untuk menyaring data yang ada pada tabel.
- `peminjam IS NOT NULL` pada kolom peminjam akan ditampilkan data yang terisi/tidak kosong.
### Kesimpulan 
Not null di gunakan ketika kita ingin menampilkan data yang terisi atau tidak kosong.

---
# ORDER BY & LIMIT
## Mengurutkan data dari data terkecil
### Struktur Query
```MySQL
SELECT * FROM [nama_tabel] ORDER BY [nama_kolom] ASC;
```

### Contoh 
```MySQL

SELECT * FROM mobil ORDER BY pemilik ASC;
```
### Hasil
![hasil](Aset/3.24.jpg)
### Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `ORDER BY` digunakan untuk mengurutkan hasil query berdasarkan hasil tertentu.
- `ASC`digunakan untuk mengurutkan hasil secara berurutan dari nilai terkecil ke nilai terbesar, seperti urutan alfabetis dari A ke Z.
### Kesimpulan 
`ORDER BY ASC` digunakan untuk mengurutkan nilai dari yang terkecil.

---
## Mengurutkan data dari data terbesar

### Struktur Query 
```MySQL
SELECT * FROM [nama_tabel] ORDER BY [nama_kolom] DESC;
```

### Contoh 
```MySQL

SELECT * FROM mobil ORDER BY peminjam DESC;
```
### Hasil
![hasil](Aset/3.25.jpg)
### Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `ORDER BY` digunakan untuk mengurutkan hasil query berdasarkan hasil tertentu.
- `DESC` digunakan untuk mengurutkan hasil secara berurutan dari nilai terbesar ke nilai terkecil, seperti urutan alfabetis dari Z ke A.
### Kesimpulan
`ORDER BY DESC` digunakan untuk mengurutkan nilai dari yang terbesar.

---
## Membatasi data yang tampil 
## Struktur Query 
```mysql
SELECT * FROM [nama_tabel]
    WHERE [nama_kolom] = [nilai] ORDER BY         [nama_kolom] ASC LIMIT [nilai];
```
## Contoh 
```mysql
SELECT * FROM mobil 
    WHERE warna = 'Hitam' ORDER BY                harga_rental ASC LIMIT 2;
```
## Hasil
![hasil](Aset/3.42.jpg)
## Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `mobil` nama dari tabel yang ingin kita tampilkan   data-data nya.
- `WHERE warna = 'Hitam'` Memilih hanya baris-baris di mana nilai kolom warna adalah `'Hitam'`.
- `ORDER BY harga_rental ASC` Mengurutkan baris-baris tersebut berdasarkan kolom harga_rental secara menaik (dari harga rental terendah ke tertinggi).
- `LIMIT 2` Membatasi hasil query untuk hanya menampilkan 2 baris pertama yang memenuhi kondisi warna hitam dan diurutkan berdasarkan harga rental.
## Kesimpulan 
Perintah SQL tersebut mengambil data `mobil` berwarna `hitam` dengan `harga_rental` terendah, hanya menampilkan 2 hasil teratas.

---
# DISTINCT
## Contoh Pertama 
### Struktur Query
```MySQL

SELECT DISTINCT(nama_kolom) FROM [nama_tabel];
```

### Contoh 
```MySQL

SELECT DISTINCT(warna) FROM mobil;
```
### Hasil
![Hasil](Aset/3.26.jpg)
### Analisis 
- `SELECT DISTINCT (warna)` digunakan untuk  mengambil nilai unik dari kolom warna dalam tabel, dan menghapus data duplikat sehingga hanya menampilkan data-data yang berbeda.
- `FROM mobil` Query tersebut memerintahkan untuk mengambil data pada tabel mobil.
### Kesimpulan 
Distinct digunakan untuk menampilkan data-data yang asli atau tidak duplikat 

---
## Kombinasi Distinct dan Order By

### Struktur Query 
```MySQL

SELECT DISTINCT(nama_kolom) FROM [nama_tabel] ORDER BY [nama_kolom] DESC;
```
### Contoh
 ```MySQL
 
SELECT DISTINCT(harga_rental) FROM mobil ORDER BY harga_rental DESC;
```

### Hasil
![Hasil](Aset/3.27.jpg)
### Analisis 
- `SELECT DISTINCT (harga_rental)` digunakan untuk mengambil nilai unik dari kolom harga_rental dalam tabel, dan menghapus data duplikat sehingga hanya menampilkan data-data yang berbeda.
- `FROM mobil` Query tersebut memerintahkan untuk mengambil data pada tabel mobil.
- `ORDER BY harga_rental DESC` Query tersebut Mengurutkan isi dalam kolom harga_rental dari yang tertinggi.
### Kesimpulan 
Kombinasi Distinct dan Order By digunakan ketika ingin mengetahui jumlah data asli yang ada pada kolom secara berurutan, baik dari yang tertinggi ataupun yang terendah.

---

# CONCAT, CONCAT_WS, AS

## Menggabungkan kolom tanpa pemisah
### Struktur Query 
```MySQL

SELECT CONCAT(kolom1,kolom2) FROM [nama_tabel];
```
### Contoh
```MySQL
SELECT CONCAT(pemilik,warna) FROM mobil;
```
### Hasil
![hasil](Aset/3.28.jpg)

### Analisis 
- `SELECT CONCAT` digunakan untuk mengambil dan menggabungkan 2 kolom atau lebih menjadi satu string tunggal.
- `(pemilik,warna)` Merupakan kolom yang akan di gabungkan menjadi satu.
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### kesimpulan 
`CONCAT` digunakan ketika kita ingin menggabungkan suatu kolom menjadi satu.

---
## Menggabungkan kolom dengan pemisah
### Struktur Query 
```MySQL

SELECT  CONCAT_WS(Separator,kolom1,kolom2,
kolom3) FROM [nama_tabel];
```
### Contoh
```MySQL
SELECT CONCAT_WS("-",no_plat,no_mesin,
id_mobil) FROM mobil;
```
### Hasil
![hasil](Aset/3.29.jpg)
### Analisis 
- `SELECT CONCAT_WS` digunakan untuk mengambil dan menggabungkan 2 kolom atau lebih menjadi satu string tunggal dengan pemisah.
- `("-",no_plat,no_mesin,id_mobil)` tanda "-"  adalah pemisah yang akan digunakan. `no_plat,no_mesin,id_mobil` nama kolom-kolom yang dipilih dari tabel untuk di gabungkan.
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### kesimpulan 
`CONCAT_WS` digunakan untuk menggabungkan nilai kolom-kolom dengan pemisah agar data-data yang di gabung terlihat rapi.

---
## Memberikan nama kolom alias

### Struktur Query 
```MySQL

SELECT CONCAT_WS(Separator,kolom1,kolom2) AS [nama_alias] FROM mobil;
```
### Contoh
```MySQL

SELECT CONCAT_WS("+",pemilik,peminjam) AS COLLAB FROM mobil;
```
### Hasil
![hasil](Aset/3.30.jpg)
### Analisis 
- `SELECT CONCAT_WS` digunakan untuk mengambil dan menggabungkan 2 kolom atau lebih menjadi satu string tunggal dengan pemisah.
- `("+",pemilik,peminjam)` tanda`"+"` sebagai pemisah `pemilik,peminjam` merupakan kolom yang akan digabungkan nilainya,setiap nilai dari kolom `pemilik` dan `peminjam` akan digabungkan menjadi satu string dengan tanda `"+"` di antara mereka.
- `AS COLLAB` AS merupakan alias sedangkan collab nama dari penggabungan 2 kolom yaitu pemilik dan peminjam.
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### kesimpulan 
Kita bisa menggunakan Query tersebut untuk menggabungkan sebuah kolom dengan memberi nama alias, agar lebih mudah di mengerti.

---
# VIEW

## Membuat tabel virtual
### Struktur Query 
```MySQL

CREATE VIEW [nama_tabel_virtual] AS SELECT id_mobil,no_plat,pemilik,peminjam FROM [nama_tabel] WHERE [nama_kolom] = "nilai";
```
### Contoh 
```MySQL

CREATE VIEW info_no_plat AS SELECT id_mobil, no_plat, pemilik, peminjam FROM mobil WHERE pemilik = "dani";
```
### Hasil
![hasil](Aset/3.31.jpg)
### Analisis 
- `CREATE VIEW info_no_plat AS` Perintah query tersebut membuat sebuah tabel virtual dengan nama info_no_plat.
- `SELECT id_mobil, no_plat, pemilik, peminjam FROM mobil` digunakan untuk memilih kolom-kolom dari tabel mobil untuk di masukkan ke dalam tabel virtual yang dibuat.
- `WHERE pemilik = "dani";` perintah tersebut akan menampilkan data-data yang pemiliknya Dani.
### kesimpulan 
Tabel virtual digunakan untuk mengelompokkan sebuah kolom tertentu dari tabel yang sudah ada.

---
## Menampilkan tabel virtual
### Struktur Query 
### Contoh 
```MySQL
SELECT * FROM info_no_plat;
```
### Hasil
![hasil](Aset/3.32.jpg)
### Analisis 
- `SELECT * FROM` : Merupakan query awal untuk menampilkan sebuah tabel virtual yang didalamnya berisikan kolom, di mana kolom tersebut menampung sebuah data.
- `info_no_plat` nama dari tabel virtual.
### kesimpulan 
Jika ingin menampilkan tabel virtual cukup dengan perintah SELECT * FROM.

---
## Menghapus tabel virtual
### Struktur Query 
### Contoh 
```MySQL
DROP VIEW info_no_plat;
```
### Hasil
![hasil](Aset/3.33.jpg)

### Analisis 
- `DROP VIEW` perintah query tersebut akan menghapus tabel virtual.
- `info_no_plat` nama tabel virtual yang akan di hapus.
### kesimpulan 
Jika ingin menghapus tabel virtual cukup dengan perintah DROP VIEW.

---
# Tantangan 
## 1
### Struktur Query 
```MySQL

CREATE VIEW [nama_tabel_virtual] AS SELECT [kolom_pilihan] FROM [nama_tabel] WHERE [kolom] = nilai;
```
### Contoh 
```MySQL
CREATE VIEW tantangan AS SELECT no_plat,warna,peminjam FROM mobil WHERE peminjam is null;
```
### Hasil
![hasil](Aset/3.34.jpg)

### Analisis 
- `CREATE VIEW` perintah MySQL yang digunakan untuk membuat tabel view yang akan tersimpan di dalam database.
- `tantangan AS` nama alias dari tabel virtual yang kita buat.
- `SELECT no_plat,warna,peminjam` Kolom yang kita pilih untuk di masukkan ke dalam sebuah tabel view yang dibuat.
- `FROM mobil` kolom yang kita pilih untuk tabel view merupakan dari tabel mobil yang sudah ada.
- `WHERE peminjam is null;` data yang akan tampil dimana peminjamnya null atau tidak ada.

### Kesimpulan 
Program MySQL tersebut membuat sebuah view yang disebut `tantangan` yang berisi daftar mobil yang belum dipinjam, dengan kolom-kolom `no_plat`, `warna`, dan `peminjam` dari tabel `mobil` di mana nilai `peminjam` belum diisi (NULL). View ini menyediakan informasi tentang mobil-mobil yang tersedia untuk dipinjam.

---
## 2
### Struktur Query 
```mysql

UPDATE [nama_tabel] SET [nama_kolom] = nilai WHERE [nama_kolom] = nilai;
```
### Contoh 
```mysql
UPDATE mobil SET peminjam = NULL WHERE id_mobil = 4;
```
### Hasil
![hasil](Aset/3.35.jpg)

### Analisis 
- `UPDATE mobil` Query tersebut akan mengupdate data pada tabel mobil.
- `SET peminjam = NULL` perintah tersebut akan mengosongkan kolom peminjam dengan `NULL`.
- `WHERE id_mobil = 4;` data yang akan di update yang memiliki `Id_mobil = 4`.

### Kesimpulan 
Perintah MySQL tersebut akan mengubah nilai kolom `peminjam` menjadi NULL untuk `mobil` yang memiliki `id_mobil = 4` dalam tabel `mobil`.

---
# AGREGASI
## Menghitung total nilai numerik suatu kolom (Sum)
### Struktur Query 
```mysql
SELECT SUM(nama_kolom) AS [nama_alias] FROM [nama_tabel]
```
### Contoh 
```mysql

SELECT SUM(harga_rental) AS total_harga FROM mobil;
```
### Hasil
![hasil](Aset/3.36.jpg)

### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan data 
- `SUM` digunakan untuk menjumlahkan nilai numerik dalam kolom.
- `harga_rental` nama kolom yang ingin di jumlahkan nilainya.
- `AS total_harga`sebagai nama alias kolom
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### Kesimpulan 
`SUM` digunakan untuk menjumlahkan nilai numerik dalam kolom 

---
## Menghitung jumlah baris/data, biasanya berdasarkan kriteria tertentu (Count)
### Struktur Query 
```mysql
SELECT COUNT(nama_kolom) AS [nama_alias] FROM 
[nama_tabel];
```
### Contoh 
```mysql
SELECT COUNT(pemilik) AS total_pemilik FROM mobil;
```
### Hasil
![hasil](Aset/3.37.jpg)

### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan data.
- `COUNT` digunakan untuk menghitung jumlah baris(nilai non-NULL).
- `pemilik` nama kolom yang ingin di hitung jumlah barisnya.
- `AS total_pemilik` sebagai nama alias kolom
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### Kesimpulan 
`COUNT` digunakan ketika ingin menghitung jumlah baris dalam suatu kolom(atau jumlah non-NULL).

---
### Struktur Query 
```mysql
SELECT COUNT(nama_kolom) AS [nama_alias] FROM 
[nama_tabel];
```
### Contoh 
```mysql

SELECT COUNT(peminjam) AS total_peminjam FROM mobil;
```
### Hasil
![hasil](Aset/3.38.jpg)

### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan data.
- `COUNT` digunakan untuk menghitung jumlah baris(nilai non-NULL).
- `peminjam` nama kolom yang ingin di hitung jumlah barisnya.
- `AS total_peminjam` sebagai nama alias kolom
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### Kesimpulan 
`COUNT` digunakan untuk menghitung jumlah baris dalam kolom yang hanya memiliki (bukan NULL)

---
## Menampilkan nilai terendah (Min)
### Struktur Query 
```mysql
SELECT MIN(nama_kolom) AS [nama_alias] FROM [nama_tabel];
```
### Contoh 
```mysql
SELECT MIN(harga_rental) AS minimum FROM mobil;
```
### Hasil
![hasil](Aset/3.39.jpg)

### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan data.
- `MIN` digunakan untuk menampilkan nilai numerik terendah dalam suatu kolom.
- `harga_rental` nama kolom yang ingin kita tampilkan nilai terendahnya.
- `AS minuman` sebagai nama alias kolom
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### Kesimpulan 
`MIN` digunakan untuk menampilkan nilai terendah dari suatu kolom.

---
## Menampilkan nilai tertinggi (Max)
### Struktur Query 
```mysql
SELECT MAX(nama_kolom) AS [nama_alias] FROM [nama_tabel];
```
### Contoh 
```mysql
SELECT MAX(harga_rental) AS maximum FROM mobil;
```
### Hasil
![hasil](Aset/3.40.jpg)

### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan data.
- `MAX` digunakan untuk menampilkan nilai numerik tertinggi dalam suatu kolom
- `harga_rental` nama kolom yang ingin kita tampilkan nilai tertinggi nya.
- `AS maximun` sebagai nama alias kolom
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### Kesimpulan 
`MAX` digunakan untuk menampilkan nilai numerik tertinggi dari suatu kolom.

---
## Menampilkan nilai rata-rata (Avg)
### Struktur Query 
```mysql
SELECT AVG(nama_kolom) AS [nama_alias] FROM [nama_tabel];
```
### Contoh 
```mysql
SELECT AVG(harga_rental) AS rerata FROM mobil;
```
### Hasil
![hasil](Aset/3.41.jpg)

### Analisis 
- `SELECT` digunakan untuk mengambil/menampilkan data.
- `AVG` digunakan untuk menghitung rata-rata dari nilai numerik yang ada pada kolom
- `harga_rental` nama kolom yang ingin kita tampilkan nilai tertinggi nya.
- `AS rerata` sebagai nama alias kolom
- `FROM mobil` query tersebut akan mengambil data dari tabel mobil.
### Kesimpulan
`AVG` digunakan untuk menghitung rata-rata dari nilai numerik pada suatu kolom.

---




