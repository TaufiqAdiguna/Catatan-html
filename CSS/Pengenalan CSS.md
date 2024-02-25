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

>[! summary ] Penjelasan
>Font-size adalah ukuran text yang terdapat pada dalam kotak, yang bertuliskan klik aku!

``` CSS
Button {
Font-size: 20px
}
```

### Hasil gambar 
#### Before 
![[1.1 before font-size.jpg]]
#### After
![[1.2 after font-size.jpg]]


---
## Margin-Top

>[! summary ] Penjelasan
margin top adalah sebuah perintah untuk memberikan jarak, dengan text yang ada diatasnya sebanyak 50px

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

>[! summary ] Penjelasan
>Color adalah warna yang akan diberikan pada text yang dipanggil 

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
## Cara Pemanggilan CSS
Terdapat 3 cara untuk pemanggilan CSS yaitu secara internal, inline, dan external.

---
### Internal
Internal adalah pemanggilan css secara satu file/ berada didalam file html yg ingin kita berikan style.
Adapun tempat penulisan CSS secara internal, kita dapat tuliskan di dalam `<head>`

#### Contoh
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








