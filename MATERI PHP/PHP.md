# Apa itu Web dinamis & PHP
## Web dinamis 
Web dinamis adalah jenis situs web yang dapat menghasilkan konten yang berbeda berdasarkan interaksi pengguna, data terbaru, atau variabel lainnya. Web dinamis dapat memberikan pengalaman yang lebih interaktif dan personal bagi pengguna karena kontennya dapat berubah secara dinamis tanpa harus memuat ulang halaman secara penuh.

## PHP
`PHP (Hypertext Preprocessor)` adalah bahasa pemrograman yang sering digunakan untuk mengembangkan aplikasi web dinamis. PHP memungkinkan Anda untuk membuat halaman web yang dapat berinteraksi dengan basis data, menghasilkan konten dinamis, mengelola formulir, mengakses file, dan melakukan banyak tugas lainnya yang diperlukan untuk membangun aplikasi web yang dinamis dan interaktif.

Dengan PHP, Anda dapat:

- Menghubungkan situs web Anda ke basis data seperti MySQL untuk menyimpan dan mengambil informasi.
- Menghasilkan halaman web yang berubah berdasarkan input pengguna.
- Membuat formulir web untuk mengumpulkan informasi dari pengguna.
- Mengelola file pada server.
- Melakukan banyak tugas pemrograman lainnya yang mendukung pengembangan web dinamis.

# Echo & commentar
## Echo
### Penjelasan 
`echo` adalah sebuah perintah yang digunakan untuk menampilkan output ke dalam halaman web. Dengan menggunakan `echo`, Anda dapat menampilkan teks, variabel, atau hasil operasi lainnya di dalam kode PHP, dan hasilnya akan ditampilkan pada halaman web ketika halaman tersebut dimuat oleh browser.
### Kode Program 
```php
<?php
    $nama = "Adiguna";
    echo "Halo, " . $nama . "! Selamat            datang.";
?>
```


---
## Commentar
### Penjelasan 
 `comment` atau komentar adalah bagian dari kode yang tidak dieksekusi oleh PHP. Komentar digunakan untuk memberikan penjelasan atau dokumentasi di dalam kode, dan komentar ini tidak akan ditampilkan pada halaman web saat dijalankan. Ada dua jenis komentar dalam PHP.
### Kode Program 
**komentar 1 baris :**
```php
// Ini adalah komentar satu baris
```

**Komentar multi-baris :**
```php
/*
 Ini adalah komentar
 multi-baris
*/
```


# Variabel,Const, Operator 
## Variabel 
### Penjelasan 
Variabel adalah sebuah wadah atau tempat untuk menyimpan data di dalam program. Di dalam PHP, variabel memiliki tipe dinamis, yang berarti Anda tidak perlu mendeklarasikan tipe data saat membuat variabel. Cukup beri nama variabel dan langsung gunakan untuk menyimpan nilai.


---
## Const
Konstanta adalah nilai yang tetap dan tidak berubah selama eksekusi program. Di PHP, Anda bisa mendefinisikan konstanta menggunakan fungsi `define()` atau keyword `const`.



---
## Operator 
Operator adalah simbol atau kata kunci yang digunakan untuk melakukan operasi tertentu pada variabel atau nilai. Ada berbagai jenis operator dalam PHP:

### Operator Aritmatika 
Digunakan untuk operasi matematika seperti penambahan (+), pengurangan (-), perkalian (*), pembagian (/), modulus (%), dll.

```php
$a = 10;
$b = 5;
$hasil_penambahan = $a + $b; // Hasilnya 15
$hasil_pengurangan = $a - $b; // Hasilnya 5
```

### Operator Penugasan 
Digunakan untuk memberikan nilai ke variabel dengan menggunakan tanda sama dengan (=) atau operator lain seperti (+=, -=, *=, /=, dll).

```php
$x = 10;
$x += 5; // Setara dengan $x = $x + 5; (Hasilnya 15)
```

### Operator Perbandingan
Digunakan untuk membandingkan dua nilai dan menghasilkan nilai boolean (true/false).

```php
$a = 10;
$b = 5;
$c = 10;
var_dump($a > $b); // Output: true
var_dump($a == $c); // Output: true

```

### Operator Logika 
Digunakan untuk menggabungkan beberapa kondisi logika dan menghasilkan nilai boolean (true/false).

```php
$x = true;
$y = false;
var_dump($x && $y); // Output: false (AND logika)
var_dump($x || $y); // Output: true (OR logika)
```