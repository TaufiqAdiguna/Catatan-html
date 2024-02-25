
---
# PENGENALAN WEB

---
# SEJARAH
Website pertama kali di ciptakan pada tahun 1990-an ketika Tim Berners-Lee menciptakan world wide web (WWW) yang memungkinkan dokumen bisa terhubung satu sama lain di internet. dan HTTP (Hypertext Transfer Protocol) menjadi dasar untuk jdi jembatan antara server dan client dalam mengakses halaman web. 
# HTML
Tim berners-lee menciptakan Hyper text market language atau yang biasa disebut (html) untuk merapikan sebuah teks dan lebih terstruktur, html merupakan bahasa pemrograman yang di ibaratkan seperti tulang manusia yang mengatur setiap bagian website, seluruh website yang di buat pasti menggunakan yang namanya html dalam html kita harus biasain yang namanya tag agar lonjong browser tau kalau itu sebuah html dan bukan teks biasa, dalam html juga terdapat yang namanya head dan body
Dimana head berfungsi sebagai penyimpanan informasi dan body sebagai tempat komponen-komponen website seperti teks, gambar, tabel, link, dll
# CSS
Pada tahun 1994 di ciptakan cascading styling sheet atau CSS oleh hakon weyung Lee yang berfungsi sebagai style dalam sebuah website. untuk membuat website terlihat lebih rapi dan elegan, cara menggunakan nya adalah kita harus kasih identitas setiap komponen html yang ingin kita hias 

# Word Wide Web atau www
Browser yang sering kali kita temui di website 

# Kesimpulan 
Pada tahun 1990-an Tim berners-lee  menciptakan html (Hyper text market language) untuk merapikan atau lebih terstruktur teks yang ada di dalamnya, html di ibaratkan seperti tulang manusia yang mengatur seluruh dokumen yang ada didalamnya, tim berners-lee juga menciptakan http (hypertext transfer protocol) sebagai jembatan antara client-server, tim berners-lee juga menciptakan worldwide website atau www untuk bisa membuka suatu website yang dibuat di html sehingga client lebih mudah mendapatkan informasi.Pada tahun 1994 di ciptakan cascading styling sheet atau CSS oleh hakon weyung Lee yang berfungsi sebagai style dalam sebuah website. Agar website yang kita buat terlihat lebih rapi dan elegan.

---
# DESKRIPSI HTML,CSS, DAN JAVASCRIPT DALAM PEMBUATAN WEBSITE 

---
# deskripsi bahasa pemrograman 

![[HTML/Aset/3.1.jpg]]

## **HTML**
Html adalah suatu kerangka yang membangun sebuah website dimana html membentuk website/rumah sesuai dengan keinginan konsumen atau yang buat
## **CSS**
Peran CSS dalam pembuatan website adalah merapikan dan melengkapi sebuah website yang sudah di buat dengan html contoh yang ada seperti cat,atap, jendela, corong Agar terlihat lebih rapi dan lengkap 
## **JAVASCRIPT**
Javascript adalah interaksi yang dilakukan didalam suatu website dimana tanpa javascript hanya website saja yang tidak bakalan ada interaksi yang dilakukan didalamnya seperti asap yang ada pada corong rumah, lampu yang menyala dikarenakan ada saklar yang dinyalakan 
## **Kesimpulan**
Yang dapat disimpulkan dari 3 bahasa pemrograman ini ialah tanpa html tidak akan terbentuk sebuah website, tanpa CSS website yang kita buat tidak akan terlihat rapi dan bagus serta peran javascript untuk menghidupkan website dengan interaksi yg ada didalam nya

---
# STRUKTUR DASAR HTML

---
# Struktur dasar html

## Penjelasan
tag <`doctype html>`memberitahukan web browser bahwa dokumen HTML adalah versi 5
- tag pembuka `<html>` menandai awal sebuah dokumen HTML sampai dengan tag penutup `<html>`
- tag pembuka `<head>` berisi informasi tentang halaman html sampai dengan tag penutup `</head>`, biasanya dalam tag head terdapat tag `<title>` untuk memberikan informasi  judul halaman html 
- adapun tag yang berada di antara tag pembuka `<body>` Sampai dengan tag penutup `</body>` akan tampil di web browser.
## Kode Program :
```html
<!doctype html>
<html>
  <head>
    <title>web saya</title>
  </head>
  <body
    <p>ketika kamu lelah, jangan berhenti tetapi istirahatlah sejenak </p>
    <p>kesuksesan itu seperti banyaknya tempe</p>
    <p>tidak ada yang tahu</p>
    <a href="https://www.google.com"> klik Google </a>
    
  </body>
</html>
```

## Hasil Program :
![struktur dasar](Aset/4.1.jpg)


> [!info] `<tag html>`
- tag <`doctype html>`memberitahukan web browser bahwa dokumen HTML adalah versi 5
- tag pembuka `<html>` menandai awal sebuah dokumen HTML sampai dengan tag penutup `<html>`
- tag pembuka `<head>` berisi informasi tentang halaman html sampai dengan tag penutup `</head>`, biasanya dalam tag head terdapat tag `<title>` untuk memberikan informasi  judul halaman html 
- adapun tag yang berada di antara tag pembuka `<body>` Sampai dengan tag penutup `</body>` akan tampil di web browser.

---
# Anatomi elemen html
## Penjelasan 
**Elemen** adalah suatu kesatuan dan sebuah Tag yang dimulai dari ==Tag pembuka== hingga ke ==Tag penutup==. **ELEMEN** HTML secara garis besar terdiri atas tiga bagian yaitu **Tag pembuka**, **konten/Isi tag**, dan **tag penutup.

![anatomi](Aset/4.2.jpg)

## Kode Program :
``` html

<a href="https://www.google.com"> klik Google </a>
```

## Hasil Program :
![Hasil program](Aset/4.3.jpg)

## Tag Atribut 

- tag pembuka `<a>` berisi nama atribut seperti href serta nilai atribut yang ingin di simpan 
- sebelum tag penutup terdapat konten atau isi tag yang berfungsi sebagai tempat pembuka link yg di simpan di nilai atribut
- tag penutup `</a>` sebagai tanda bahwa suatu elemen berakhir 
### nama atribut 

 Href adalah nama atribut berfungsi untuk menentukan url atau alamat tujuan. dan dapat mengarahkan client ke halaman google jika url yang kita pilih google https://www.google.com

### nilai atribut 

 Https://www.google.com adalah nilai atribut. Sebagai url atau alamat web yang ingin ditujukan. Dengan memilih url ini dalam atribut tag `<a>` kita bisa masuk ke halaman google. 

### isi konten/tag

 **Klik google** adalah berfungsi sebagai petunjuk bagi client bahwa deskripsi tersebut  akan mengarahkan ke halaman go
 
 ---
  </body>
</html>
```

### Hasil Program Tag Italic :
![tag Italic](Aset/4.8.jpg)

---
## ==Tag Br==
### Penjelasan
- `<br>`: Tag ini digunakan untuk membuat jeda baris, sehingga teks akan ditampilkan di baris berikutnya, jika ingin membuat jeda baris lebih jauh kita harus mengulang penggunaan tag `<br>`.

### Kode Program Tag Br :
```html
<!doctype html>
<html>
  <head>
    <title>tag atribut</title>
  </head>
  <body>
   <p>baris pertama <br> baris kedua <br> baris ketiga</p>
  </body>
</html>
```

### Hasil Program Tag Br :
![tag br](Aset/4.9.jpg)


---

### Kode Program Tag Align :
```html

<h3>Belajar Menggunakan Elemen Tag HTML p</h3>
<p align="left">
Sebuah rumah yang berisikan satu keluarga yaitu,ayah,ibu,dan 3 anaknya.<\p>
<p align="right">
Sebuah rumah yang berisikan satu keluarga yaitu,ayah,ibu,dan 3 anaknya.</p>
<p align="center">
Sebuah rumah yang berisikan satu keluarga yaitu,ayah,ibu,dan 3 anaknya.</p>
<p align="justify">
Sebuah rumah yang berisikan satu keluarga yaitu,ayah,ibu,dan 3 anaknya.</n>

```

### Hasil Program Tag Align :
![tag Align](Aset/4.10.jpg)


___
## ==Komentar==
### Penjelasan 
Html juga mempunyai Tag khusus untuk komentar.Untuk membuat komentar di HTML kita menggunakan awalan `<!--` dan penutup `-->`.

> [!faq]  info!
>  Komentar tidak akan di tampilkan pada halaman website namun programmer biasanya menggunakan komentar untuk memperjelas kode program

### Kode Program Komentar :
```html

<!--ini komentar tidak akan tampil di browser -->
<p>ini bukan komentar dan akan tampil di browser</p>
```

### Hasil Program Komentar :
![komentar](Aset/4.11.jpg)


---
## ==List==
### Penjelasan 
List adalah fungsi dalam HTML yang digunakan untuk menampilkan daftar dari sesuatu.Tag HTML terdiri dari 2 jenis ,`<ol>` ordered list (berurutan),dan `<ul> `urdered list (tidak berurutan). oredered list `<ol>` akan ditampilkan dengan angka atau huruf sedangkan undered list `<ul>`dengan bulatan atau kotak ataupun simbol lainnya.

>[!faq] !! Untuk menampilkan list dalam HTML dapat menggunakan tag `<ol>`...`<\ol>` atau` <ul>`...`</ul>`namun perlu dengan menyisipkan elemen `<li>` untuk membuat daftar list


---
### ==Tag ul==
### Kode Program urdered list :
```html
urdered list

<h1>list peralatan kelas</h1>
<ul>
<li>Sapu</Li>
<li>pel</Li>
<li>dispenser</Li>
<li>kipas</Li>
<li>gelas</Li>
</ul>


```

### Hasil Program urdered list :
![ul list](Aset/4.12.jpg)

---
### ==Tag ol==
#### Beberapa type list ol/ordered list
- type = "1" artinya daftar isi akan menggunakan angka (ini adalah default nya)
- type = "A" artinya daftar isi akan menggunakan huruf kapital
- type = "a" artinya daftar isi akan menggunakan huruf kecil 
- type ="I" artinya daftar isi akan menggunakan angka Romawi kapital
- type ="i" artinya daftar isi akan menggunakan angka Romawi kecil
### Kode Program ordered list :
``` html
Ordered list

<h1>list Kalimat</h1>
<ol>
<li>Ini kalimat pertama</Li>
<li>ini kalimat kedua</Li>
<li>ini kalimat ketiga</Li>
<li>ini kalimat ke empat</Li>
<li>ini kalimat ke lima</Li>
</ol>
```

### Hasil Program ordered list :
![ol list](Aset/4.13.jpg)

---
## ==Link==
### Penjelasan 
Link dapat ditemukan di hampir semua halaman web. Link/Tautan memungkinkan sebuah teks yang ketika di-klik akan pindah ke halaman lainnya. HTML Menggunakan tag `<a>` untuk keperluan ini. Link ditulis dengan `<a>` yang merupakan singkatan dari anchor (jangkar). 

Setiap tag `<a>` setidaknya memiliki sebuah atribut `href` Dimana `href` berisi alamat yang dituju. `href` adalah singkatan dari hypertext reference. 

Atribut Penting Lainnya dari tag `<a>` adalah `target` . Atribut target menentukan tempat untuk membuka dokumen yang ditautkan. Atribut `target` memiliki beberapa nilai salah satunya `_blank` yang berfungi untuk membuka tautan di tab baru. 

### Kode Program Tag Anchor :
```html
<h3>Menggunakan Tag Anchor</h3>
<a href ="https://www.google.com" target="_blank">klik disini untuk ke google</a><br>
<a href ="halaman_lain.html">klik disini untuk ke halaman lain yang saya buat!</a>
```

### Hasil Program Tag Anchor :
![link](Aset/4.14.jpg)


---
## ==Multimedia==

### Gambar
#### Penjelasan 
Dalam HTML gambar didefinisikan dengan tag <img> Tag <img> adalah tag kosong hanya berisi atribut saja, dan tidak memiliki tag penutup. 

Atribut ==src== setidaknya mesti ada dalam tag ini untuk menentukan URL (alamat web) dari gambar yang ingin ditampilkan. 

Atribut ==alt== menyediakan teks alternatif untuk gambar, jika pengguna karena beberapa pengguna alasan tidak dapat melihatnya (karena koneksi lambat, kesalahan pada atribut ==src== ,atau jika web browser telah disetting untuk tidak menampilkan gambar). Jika browser tidak dapat menentukan gambar, maka akan muncul nilai pada atribut ==alt==  

Dalam tag `<img>` terdapat juga atribut `<width>` dan `<height>` untuk mengatur ukuran gambar, pada versi HTML5 standar satuan ukuran gambar adalah pixel. 

- Misalnya dalam folder root terdapat file gambar bernama logo.png. untuk menampilkan gambar tersebut kita hanya perlu mengisi nama gambar beserta jenis ekstensi file gambar ke dalam atribut `src` , Contohnya `src = "logo.png"` 
- untuk menampilkan dari internet carilah link gambar yang akan ditampilkan lalu masukkan dalam nilai atribut `src` , contohnya **`https://namasitus.com/gambar.png`**

#### Kode Program Tag img :
```html
<img src="pulau-padar.jpg" width="400" height="200">
```

#### Hasil Program Gambar :
![hasil gambar](Aset/4.15.jpg)

#### Folder Program Gambar :
![folder gambar](Aset/4.16.jpg)


---
### Video
#### Penjelasan 
Fitur HTML 5 mencakup dukungan audio dan video asli tanpa memerlukan flash. tag `<audio>` dan `<vidio>` pada HTML 5 mempermudah penambahan media ke dalam halaman web. Yang penting untuk diatur pada tag ini adalah atribut `src` yang berfungsi untuk mengidentifikasi sumber media. Selain itu, terdapat pula atribut `controls`agar pengguna dapat memutar dan menjeda media.

#### Kode Program Tag Video :
```html
    <video src="videotiktok.mp4" controls width="100%" height="500" ></video>
```

#### Hasil Program Video :
![hasil video](Aset/4.17.jpg)

#### Folder Program Video :
![folder video](Aset/4.18.jpg)

---
### Audio
#### Penjelasan 
Seperti yang telah dibahas sebelumnya bahwasanya tag `<audio>` merupakan bagian fitur HTML5 untuk menampilkan audio asli dihalaman web tanpa memerlukan flash sebagaimana pada HTML versi 4. Yang penting untuk diatur pada tag ini adalah atribut `src` yang berfungi untuk mengidentifikasi sumber media. Selain itu, terdapat pula atribut `controls` agar pengguna dapat memutar dan menjeda media. 

#### Kode Program  Tag Audio :
```html 
  <audio src="musiktiktok.mp3" controls >
  Browser anda tidak mendukung elemen 
  <audio>.</audio>
```

#### Hasil Program Audio :
![hasil audio](Aset/4.19.jpg)


> [!INFO]
> Konten berupa teks "Browser anda tidak mendukung elemen `<audio>`." Pada tag `<audio>` akan ditampilkan jika browser tidak mendukung elemen tersebut. Sehingga sebenarnya bagian ini dapat dihilangkan.

#### Folder Program Audio :
![folder audio](Aset/4.20.jpg)

---
### Iframe 
#### Penjelasan 
 Elemen <`iframe>` dapat digunakan untuk menampilkan halaman website lain dalam suatu website. Atau menampilkan dokumen html lain dalam sebuah website. Mudahnya, bisa dibilang website dalam website

 Contoh penggunaannya seperti ini. Jika kita mempunyai website sekolah, lalu di website tersebut ingin menampilkan alamat dalam google maps sekolah. Agar memudahkan pengunjung website,kita bisa langsung tampilkan saja halaman sekolah yang ada digoogle maps

 Dalam tag inframe ada beberapa atribut yang penting seperti : 
- src,untuk mencari sumber halaman html atau web yang akan ditampilkan didalam frame
- width dan height, untuk mengatur ukuran panjang dan lebar dari frame.

#### Kode Program Tag Iframe :
```html

<iframe src="https://smkn7makassar.sch.id/" 
width="400"></iframe>
```

#### Hasil Program Iframe :
![hasil iframe](Aset/4.21.jpg)

---
## ==Table==
### Penjelasan 
Tabel dalam HTML didefinisikan dengan tag `<table>`.
- Setiap baris tabel didefinisikan dengan tag `<tr>`.
- Header/judul tabel didefinisikan dengan tag `<th>`.Secara default, header tabel memiliki teks tebal dan berada di tengah.
- Data tabel/sel didefinisikan dengan tag `<td>`karena sel merupakan bagian terkecil dari tabel maka dari itu tag ini selalu berada di dalam tag `<tr>`.

Perhatikan bahwa pada tag `<table>` terdapat sebuah atribut `<border>`. Atribut digunakan untuk memberikan nilai garis tepi dari tabel. Nilai ini dalam ukuran pixel. `border="1"`, berarti kita menginstruksikan kepada web browser bahwa tabel tersebut akan memiliki garis tepi sebesar 1 pixel. Jika tidak ditambahkan, secara default tabel tidak memiliki garis tepi.
#### Atribut Table
Selain itu, terdapat pula beberapa atribut tabel yang penting untuk diketahui yaitu:
- ==rowspan== merupakan atribut HTML yang berfungsi untuk menggabungkan beberapa baris (ke bawah).
- ==colspan== atau colomn span merupakan atribut html yang berfungsi untuk menggabungkan beberapa kolom (ke samping).
- ==width== berfungsi untuk mengatur lebar kabel yang nilainya didefinisikan dalam satuan pixel secara default.
- ==height== berfungsi untuk mengatur tinggi tabel yang nilainya didefinisikan dalam satuan pixel secara default.
- ==Align== berfungsi untuk mengatur perataan teks pada tabel.nilai atribut yang dapat diberikan yaitu left untuk perataan teks kekiri,right untuk teks ke kanan dan,center untuk perataan teks ke tengah.

---

### Kode Program Tabel 1 :
```html
<table Border="1">
<tr>
<th>nama</th>
<th>Asal institusi</th>
</tr>
<tr>
<td>adiguna</td>
<td>halba</td>
</tr>
<tr>
  <td>Zhafran</td>
  <td>fajar tv</td>
</tr>
```

### Hasil Program Tabel 1 :
![tabel 1](Aset/4.22.jpg)

---
### Kode Program Tabel 2 :
``` html
<table Border="1">
<tr>
<th rowspan="2">nama</th>
<th colspan="2">Asal institusi</th>
</tr>
<tr>
<th width="100">sekolah</th>
<th width="100">kampus</th>
</tr>
<tr>
<td>uga</td>
<td>SMKN 7 MAKASSAR</td>
<td>universitas negeri Makassar</td>
</tr>
<tr>
  <td>fatur</td>
  <td rowspan="2"> SMKN 7 Makassar</td>
  <td align="center" rowspan="2<">-</td>
</tr>
<tr>
  <td>rezeky awalya</td>
</tr>
  <td>rizal</td>
  <td>SMKN 7 MAKASSAR</td>
  <td>unhas</td>
</tr>
</table>
```

### Hasil Program Tabel 2 :
![tabel 2](Aset/4.23.jpg)


> [! info ] perhatikan para konten elemen `<td` yang berisi `Rezeky Awalya`, hanya terdapat satu elemen `<td>` disana. Hal ini dikarenakan konten elemen `<td>` sebelumnya yaitu `SMKN 7 Makassar` dan `-` pada data `fatur` mengandung atribut `rowspan` dengan bernilai `2` yang secara otomatis mengisi data di bawahnya yakni data `Rezeky awalya`. Nilai `2` menunjukkan bahwa ada dua baris yang digabungkan menjadi satu.
>  Konsep ini juga sama dengan apa yang terjadi pada `<th rowspan="2">nama</th>` dan `<th colspan="2">Asal institusi</th>`

---
### Penjelasan Tabel latihan
`<table Border="2" width="100%">:` Mendefinisikan sebuah tabel dengan batas (border) sebesar 2 piksel dan lebar 100% dari lebar elemen induknya.

`<tr align="center" bgcolor="green">:` Membuat baris pertama tabel dengan teks berada di tengah (align="center") dan latar belakang (bgcolor) berwarna hijau.

`<td colspan="2">nama hari</td>` dan `<td colspan="2">nama bulan</td>:` Menggunakan sel data dengan teks "nama hari" dan "nama bulan" yang mengambil dua kolom secara horizontal (colspan="2").

`<tr align="center">: `Membuat baris kedua tabel dengan teks berada di tengah 

`<td>Senin</td>`, `<td>Selasa</td>`,`<td>april</td>`:
Mengisi sel data pada baris kedua dengan teks "senin", "selasa", dan "april".

`<td> rowspan="2">Juni</td>` : Mengisi sel data pada baris kedua, kolom keempat dengan teks "juni" dan menggabungkan sel tersebut ke dua baris (rowspan="2").

`<tr align="center">`: Membuat baris ketiga tabel dengan teks berada di tengah.

`<td>rabu</td>,`` <td>kamis</td>, ``<td>mei</td>:` Mengisi sel data pada baris ketiga dengan teks "rabu", "kamis", dan "mei".

### Kode Program Tabel Latihan :
```Html
  <table Border="2" width="100%" >
    <tr align="center" bgcolor="green">
      <td colspan="2">nama hari</td>
      <td colspan="2">nama bulan</td>
    </tr>
    
    <tr align="center">
      <td>senin</td>
      <td>selasa</td>
      <td>april</td>
      <td rowspan="2">juni</td>
    </tr>
    
    <tr align="center">
      <td>rabu</td>
      <td>kamis</td>
      <td>mei</td>
    </tr>
  </table>
```

### Hasil Program Tabel Latihan :
![tabel latihan](Aset/4.26.jpg)


---
## ==Form==
### Penjelasan 
Elemen `<form>` HTML digunakan untuk mendefinisikan form yang digunakan untuk mengumpulkan inputan dari pengguna website. Tag ini digunakan untuk mengkoleksi inputan dari user, konsep ini sama seperti konsep formulir di dunia nyata.

>[!info]
Dengan kata lain tag `<form>` merepresentasikan sebuah "formulir" di mana satu formulir bisa memiliki banyak kolom isian.

Form HTML berisikan elemen-elemen `<form> ` lainnya. Elemen `<form>` digunakan untuk menampung macam-macam elemen yang berkaitan dengan sebuah `form`, seperti `text` `fields`, `checkbox`, `radio button`, `tombol subalt`, dan banyak lagi yang dapat diedit kemudian ditulis untuk dikirim pada sebuah server untuk selanjutnya diproses guna mendapatkan informasi tertentu dari atau untuk user.

Umumnya, sebuah website selalu memiliki fitur form, contoh paling umum yang sering kita temui adalah seperti form login, form sign up, form komentar di suatu blog/media. 

---
#### Input
Elemen `<input>` adalah elemen `form` yang paling penting. Elemen `<input>` dapat ditampilkan dalam beberapa cara, tergantung pada nilai atribut `type` yang digunakan. Request Berikut adalah beberapa contoh nilai dari atribut `type`:

 - ==Text== digunakan untuk mengambil isian berupa teks. Contohnya seperti nama.
 
- ==Password== digunakan untuk mengambil isian berupa kata sandi atau sesuatu yang bersifat rahasia. Tipe ini akan mengubah semua karakter yang diketikkan ke dalam karakter bulat.

- ==Radio== digunakan sebagai kolom isian bertipe pilihan yang menawarkan beberapa opsi kepada user namun tetapi hanya satu opsi saja yang boleh dipilih. Contohnya seperti jenis kelamin atau agama.

>[!note]
Perlu diperhatikan bahwa untuk penggunaan tipe radio yang berkategori set pilihan yang sama mengharuskan nilai-nya juga sama.

  Opsi default dapat dilakukan dengan menambahkan atribut checked pada elemen opsi yang dijadikan sebagai opsi default.

- ==Checkbox== digunakan untuk memberikan **daftar pilihan dalam satu set opsi**. User dapat memilih satu atau bahkan lebih dari satu pilihan pada tipe ini. Hal ini berbeda dengan tipe sebelumnya yaitu `radio` yang hanya memungkinkan user untuk memilih satu  pilihan saja. Contoh penggunaan `checkbox` seperti daftar makanan kesukaan, daftar olahraga yang tidak disukai, dan yang semisalnya.

>[!note]
Perlu diperhatikan bahwa untuk penggunaan tipe checkbox yang berkategori set pilihan yang sama mengharuskan nilai name -nya juga sama.

- ==Number== digunakan untuk membatasi isian user hanya pada karakter numerik saja. Browser akan menambahkan dua buah tombol atas dan bawah untuk mengubah angka isian.
  Beberapa atribut untuk tipe `number`:
  - `min`-menentukan angka minimal
  - `max`-menentukan angka maksimal
  - `step`-smenentukan kelipatan (nilai yang tidak sesuai kelipatan tidak bisa di-input, dan default dari atribut ini adalah 1)

- ==Date== digunakan untuk memberikan isian berupa tanggal. Atribut `min` dan `max` dapat pula difungsikan pada tipe ini untuk mengatur tanggal minimal dan tanggal maksimal yang diinginkan. Nilai `min` dan `max` tersebut ditulis dengan format: `YYYY-em-dd`.

- ==File== digunakan untuk memungkinkan pengguna memuat file. Atribut `accept` juga dapat disisipkan pada tipe ini dengan maksud untuk mengatur file apa saja yang boleh di-upload. Beberapa contoh value dari atribut `accept` yaitu:
   - `accept="image/png,inage/jpg.Image/jpeg` - untuk file gambar seperti `png`. `jpg`. atau `jpeg`
   - `accept="pdf"` - untuk file pdf
   - `accept="pdf"` - untuk file pdf
   - `accept-".doc, docx"` - untuk file `doc` atau `docx`
   - `accept-".ppt, pptx"` untuk file `ppt` atau `pptx`

- ==submit== ditampilkan dalam bentuk tombol untuk mengirim data pada `<form>` yang menjadi pembungkusnya. Atribut `value` digunakan untuk mengisi teks yang ingin ditampilkan pada tombol.

- ==reset== berguna untuk **mengembalikan state (keadaan) atau data dari suatu form ke nilai awalnya**. Jika nilai awal sebuah input adalah kosong, maka ketika direset ia akan kembali kosong. Tapi jika nilai awalnya sudah terisi sesuatu, maka ketika direset datanya akan kembali seperti yang sudah diset sebelumnya.

- ==button== berguna untuk membuat inputan berupa sebuah tombol. Tombol ini nantinya bisa difungsikan sesuai dengan keinginan dari pengembang web

---
#### Label
Elemen `<label>` memiliki fungsi khusus untuk melabeli sebuah kolom inputan. Ketika screen reader membaca konten halaman HTML, lalu menemukan sebuah inputan, ia akan membaca label yang  bersangkutan. Fungsi lain dari tag `<label>` adalah ketika kita mengklik label, maka browser akan meletakkan fokus pada kolom isian yang terhubung dengannya. Syarat yang perlu diperhatikan yaitu dengan menghubungkan sebuah `<label>`dan `<input> `dengan atribut for untuk label, dan atribut id pada `<input>` dengan nilai untuk kedua atribut tersebut mesti sama persis.

---
#### Select
Elemen `<select>` berguna dalam mendefinisikan sebuah tombol dropdown yang dimana user dapat memilih salah satu dari banyak pilihan.

>[!note] 
> Elemen `<select>` nantinya berperan sebagai kontainer atau pembungkus dari elemen `<option>` yang berperan sebagai daftar pilihan atau opsi. 

 Elemen `<select>` hampir mirip fungsinya dengan `<input type ="radio">` akan tetapi baiknya elemen `<select>` digunakan untuk memilih satu pilihan yang terdapat banyak opsi di dalamnya, sedangkan `<input type ="radio">` lebih baiknya untuk digunakan jika user diarahkan memilih hanya satu pilihan yang opsi pilihannya tidak terlalu banyak. Contoh penggunaan elemen ini seperti memasukkan pilihan berupa asal daerah atau yang semisalnya.
 Penting untuk diketahui bahwasanya opsi yang aktif secara default adalah  opsi yang pertama. Akan tetapi, kita bisa mengatur opsi mana yang aktif secara default dengan menambahkan atribut select pada suatu `<option>` yang ingin dijadikan sebagai opsi default.

---
#### Text Area
Elemen `<textarea>` berguna untuk mengambil inputan user berupa teks yang dapat memuat lebih dari satu baris. Jika dibandingkan dengan elemen `<input>` teks biasa, elemen `<textarea>` memiliki ukuran tinggi yang lebih besar. Element `<textarea>` bisa diisi lebih dari satu baris dengan menekan enter.

Atribut yang dapat digunakan untuk mengatur kuran dari textarea yaitu rows untuk jumlah baris, sedangkan atribut cols untuk lebarnya.

---
#### Button
Elemen `<button>` yang berada di dalam sebuah `form` akan otomatis dianggap sama fungsinya seperti `<input type="submit">`. Jika ingin membuat tombol biasa yang tidak men-submit `<form>` dapat dilakukan dengan menambahkan atribut `type="button"`.

---
### Kode Program Form 
```html
<h1>Formulir Pendaftaran</h1>
<form action="">
  <div>
    <label for="nama-lengkap"><b>Nama Lengkap:</b></label
    ><br />
    <input
      type="text"
      id="nama-lengkap"
      name="nama_lengkap"
      placeholder="Masukkan nama lengkap"
      required
    />
  </div>
  
  <div>
    <label for="password"><b>Password:</b></label
    ><br />
    <input
      type="password"
      id="password"
      name="password"
      placeholder="Masukkan password"
      required
    />
  </div>
  
  <div>
    <b>Jenis Kelamin:</b><br />
    <input id="lk" type="radio" name="jenis_kelamin" checked />
    <label for="lk">Laki-Laki</label>
    <input id="pr" type="radio" name="jenis_kelamin" />
    <label for="pr">Perempuan</label>
  </div>
  
  <div>
    <label for="isian-usia"><b>Usia:</b></label
    ><br />
    <input
      type="number"
      id="isian-usia"
      name="usia"
      min="17"
      max="25"
      value="19"
      required
    />
    Tahun
  </div>

  <div>
    <label for="tgl-ijazah"><b>Tanggal Ijazah:</b></label> <br />
    <input
      type="date"
      id="tgl-ijazah"
      name="tgl_ijazah"
      min="2021-01-01"
      value="2023-06-20"
      required
    />
  </div>

  <div>
    <label for="opsi-agama"><b>Agama:</b></label
    ><br />
    <select id="opsi-agama" name="agama" required>
      <option disabled>---Pilih Agama----</option>
      <option value="islam">Islam</option>
      <option value="kristen">Kristen</option>
      <option value="katolik">Katolik</option>
      <option value="hindu">Hindu</option>
      <option value="buddha">Buddha</option>
      <option value="atheis" disabled>Atheis</option>
    </select>
  </div>

  <div>
    <label for="alamat"><b>Alamat:</b></label> <br />
    <textarea
      id="alamat"
      name="alamat"
      cols="25"
      rows="5"
      placeholder="Harap masukkan alamat secara lengkap"
      required
    ></textarea>
  </div>

  <div>
    <b>Kemampuan Berbahasa Asing:*</b><br />
    <input type="checkbox" id="inggris" name="bahasa_asing" />
    <label for="inggris">Inggris</label>
    <input type="checkbox" id="arab" name="bahasa_asing" />
    <label for="arab">Arab</label>
    <input type="checkbox" id="jepang" name="bahasa_asing" />
    <label for="jepang">Jepang</label>
  </div>

  <div>
    <label for="isian-foto"><b>Foto 4x6:*</b></label
    ><br />
    <input
      type="file"
      id="isian-foto"
      name="foto"
      accept="image/png,image/jpg,image/jpeg"
    />
  </div>

  <br />
  <input type="submit" value="Kirim" />
  <input type="reset" value="Batal" />
  <i>*opsional (tidak wajib diisi)</i>
</form>
```

### Hasil Program Form
![form](Aset/4.24.jpg)

- ==name== - digunakan sebagai nama variabel yang akan diproses oleh web server (contoh menggunakan PHP).
- ==required== - digunakan untuk memastikan bahwa pengguna harus memasukkan nilai pada input tersebut sebelum dapat melakukan proses submit formulir.
- ==placeholder== - menuliskan teks pada elemen input. Placeholder sangat bermanfaat untuk memberikan teks bantuan kepada user untuk inputan form yang kompleks.
- ==value== - menentukan nilai awal dari sebuah elemen input.
- ==disabled== - digunakan untuk menonaktifkan inputan pada elemen yang diberi atribut ini.


---
### Penjelasan Form latihan

1. `<form>:` Membuat formulir untuk mengumpulkan data dari pengguna.
2. `<label>`: Memberi label kepada elemen formulir agar lebih jelas.
3. `<input>`: Elemen input untuk menerima data dari pengguna.
   - `type="text`": Input teks untuk nama lengkap.
   - `type="password":` Input sandi (diberi ID "sandi").
   - `type="radio`": Pilihan jenis kelamin (diberi ID "jk").
   - `type="checkbox"`: Pilihan bahasa pemrograman (WEB, MOBILE, DESKTOP).
   - `type="submit"`: Tombol kirim.
   - `type="reset"`: Tombol reset untuk mengulangi formulir.
4. `<select>`: Elemen dropdown untuk memilih kota asal.
5. `<option>`: Opsi dropdown (Surabaya, Makassar).
6. `checked`: Menandai opsi default untuk radio button jenis kelamin.

### Kode Program Form Latihan :
``` html
<!doctype html>
<html>
  <head>
    <title>heading</title>
  </head>
  <body>

    <form>
    <label for="nama-lengkap">nama :</label>
      <input type="text" id="password"               required> 
      <br>
      <br>
      <label for="sandi">password :</label>
      <input type="password" id="sandi">
      <br>
      <br>
      <label>jenis kelamin :</label>
      <br>
      <input type="radio" name="jk" id="jk"          checked>
      <label for="jenis kelamin">Laki-laki           </label>
      <input type="radio" name="jk" id="jk">
      <label for="jenis kelamin">                     perempuan</label>
      <br>
      <br>
      <label>bahasa pemrograman yang dikuasai:       </label>
      <br>
      <input type="checkbox" name="web" id="">
      <label>WEB</label>
      <input type="checkbox" name="mobile"           id="">
      <label>MOBILE</label>
      <input type="checkbox" name="desk" id=""
      <label>DESKTOP</label>
      <br>
      <br>
      <label>kota asal</label>
      <br>
      <select name="kota asal" id="">
       <br>
        <option>Surabaya</option>
        <option>Makassar</option>
        </select>
       <br>
       <br>
        <input type="submit" value="kirim">
        <input type="reset" value="ulangi">
      </form>
  </body>
</html>
```

### Hasil Program Form Latihan :
![form latihan](Aset/4.25.jpg)


---
### **Bagaimana Cara Memproses Form?**

Ketika sebuah `<form>` disubmit, baik menggunakan elemen `<button>` mau pun `<input type="submit">`, browser akan mengirimkan data tersebut kepada URL yang didefinisikan pada atribut `action` di dalam tag `form`.

Ada pun jika atribut `action` tidak didefinisikan, maka *browser* akan menggunakan URL sekarang sebagai tujuan pengiriman data.

==Contoh:==

```html

<form action="/proses-pendaftaran">
</form>
```

Pada contoh di atas, ketika form di-*submit*, *browser* akan mengirimkan data yang ada  menuju URL `/proses-pendaftaran`.

**Apa yang terjadi pada URL `/proses-pendaftaran`?**

Pada URL tersebut terdapat sebuah aplikasi/program yang berjalan di *server* (bukan di *browser*). Tugas dari program tersebut adalah mengelola data yang dikirim seperti misalnya menyimpan data tersebut ke dalam sebuah *database*.

Bahasa yang umum digunakan di dalam server adalah python, nodejs, PHP, dan lain sebagainya.

Untuk mendapatkan gambaran lebih jelas, sebenarnya akan dijelaskan pada modul selanjutnya yang berkaitan dengan materi PHP atau juga bisa dengan membaca tutorial berikut:
https://jagongoding.com/web/php/web-dinamis/membuat-dan-menangani-form/

---
## ==Div dan Span==
### Div 
#### Penjelasan 
Div digunakan untuk mengelompokkan Elemen html menjadi blok atau bagian yang lebih besar atau lebih singkatnya di gunakan sebagai tempat atau wadah
#### Kode Program 
```HTML
<!doctype html>
<html>
  <head>
    <title>DIV</title>
  </head>
  <body>
    <div class="navbar">
      <ul>
        <li>beranda</li>
        <li>artikel</li>
        <li>media sosial</li>
      </ul>
    </div>
```

#### Hasil
![Div](Aset/4.27.jpg)

---
### Span
#### Penjelasan
Span digunakan untuk menandai atau mengelompokkan sebagian teks atau elemen inline tanpa memengaruhi struktur blok.
#### Kode Program
```HTML
<html>
  <head>
    <title>SPAN</title>
  </head>
  <body>
<p><span style="color:aqua; font-size:25px;">Selamat datang</span><br><span style="color:red; font-size:35px"> di Perpustakaan Online</span></p>
```

#### Hasil
![span](Aset/4.28.jpg)

