# Anatomi CSS
![anatomi css](Aset-CSS/1.1.jpg)
## Selector
Selector CSS di gunakan untuk memilih elemen HTML yang akan diberi gaya.Dengan menggunakan selector, Anda dapat menargetkan satu atau lebih elemen HTML untuk menerapkan properti CSS.

## Property
Property dalam CSS adalah karakteristik atau gaya yang diterapkan pada elemen HTML, seperti warna, ukuran font, atau margin. Properti bekerja dengan selector untuk mengatur tata letak dan penampilan elemen

## Property value
Dalam CSS property value (nilai sifat) merujuk pada nilai konkret yang diberikan kepada suatu properti.

---
# Percobaan I

.

# Percobaan II

## Kode css
```css
Button {
 Width: 150px;
 Height: 50px;
 Font-size: 20px;
 Margin-top: 50px;
 Color: white;
}
```

---
## Font-size

### Penjelasan
Font-size adalah Property yang menentukan ukuran text pada property html,yang terdapat pada dalam kotak, yang bertuliskan klik aku!

``` CSS
Button {
Font-size: 20px
}
```

### Hasil gambar 
#### Before 
![[1.1 before Font-size.jpg]]
#### After
![[1.2 after font-size.jpg]]


---
## Margin-Top
### Penjelasan 
margin top adalah sebuah Property untuk memberikan jarak pada suatu elemen terhadap elemen yang ada di atasnya.

```CSS
Button {
margin-top:50px;
}
```

### Hasil Gambar 
#### Before
![[1.3 before margin-top.jpg]]
#### After
![[1.4 after margin-top.jpg]]

---
## Color
### Penjelasan
Color adalah warna yang akan diberikan pada text yang di panggil dengan Selector

``` CSS
Button {
Color:green;
}
```

### Hasil Gambar 
#### Before 
![[1.5 Before color.jpg]]
#### After
![[1.6 After color.jpg]]


---
# Cara Pemanggilan CSS

---

**Terdapat 3 cara untuk pemanggilan CSS yaitu secara internal, eksternal dan inline**

---
## Internal
Internal adalah pemanggilan css secara satu file/ berada didalam file html yg ingin kita berikan style.
Adapun tempat penulisan CSS secara internal, kita dapat tuliskan di dalam `<head>`
### Contoh
```HTML

<!doctype html>
<html>
  <head>
    <title>web saya</title>
    
    <style>
      p {
      Color: bluesky;
      }
    </style>
    
  </head>
  <body>
    <p>Selamat datang</p>
  </body>
</html>
```

---
### Inline
Inline adalah pemanggilan css dengan cara didalam tag yang ingin kita berikan style.

### Contoh
```HTML

<!doctype html>
<html>
  <head>
    <title>web saya</title>
  </head>
  <body>
    <p style="color:red;">Hallo world</p>
  </body>
</html>

```

---
### External
External adalah pemanggilan dengan cara membuat file baru dengan format filenya ==nama_file.css== Berbeda dengan internal dan inline yang cukup dengan 1 file saja.

#### Contoh
##### File Html 
``` HTML

<!doctype html>
<html>
  <head>
    <title>web saya</title>
    <link rel="stylesheet" href="style.css"
  </head>
  <body>
    <p>Hallo RPL</p>
  </body>
</html>
```

##### File CSS
``` CSS
p {
Color: black;
}

```

---
# Selector Umum CSS

---
## Elemen Selector 
Elemen selector adalah jenis selector dengan cara pemanggilan langsung menyebut tag htmlnya. Contoh jika menggunakan tag `<p>` itu akan memilih semua elemen paragraf pada html.

## Class Selector
Digunakan untuk memberikan gaya pada elemen HTML yang memiliki kelas tertentu. Kelas ini didefinisikan di dalam tag HTML dengan atribut class. Satu elemen dapat memiliki banyak kelas, dan kelas dapat digunakan oleh beberapa elemen.

## Id Selector
ID dalam CSS merujuk pada identifikasi unik dari sebuah elemen HTML. Setiap elemen dapat diberi ID yang berbeda, dan ID tersebut harus unik di dalam satu halaman web. ID digunakan untuk memberikan gaya atau memanipulasi elemen secara spesifik.


---
# Text

---
## Text-align

### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 
---
## Text-decoration
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 
---
## Text-transfrom
### Penjelasan
- capitalize
- uppercase
- lowercase
- none
### Kode Program
### Hasil
### Kesimpulan 
---
## Text-indent
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 
---
## Letter-spacing
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---
## Line-height
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---
## Word-spacing
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---

---
# Background

---
## Background-image
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---
## Background-size
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---
## Background-repeat

### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---
## Background-attachment
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 

---
## Background-position
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 
Center
Left
Right

---

---

---
# Font

---
## Font-size
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 
---
## Font-style
### Penjelasan
### Kode Program
### Hasil
### Kesimpulan 
Normal
Italic
## Font-weight
Normal
Bold
Lighter
Bolder
## Font-family









---
# Box Model

---
# Border

---
### Border-width
### Border-style
#### solid
#### dashed
#### double
### Border-color

---
# Padding

---
## Padding-left
## Padding-bottom
## Padding-right
## Padding-top

---
# Margin

---
## Margin-left
## Margin-top
## Margin-right
## Margin-bottom

---

