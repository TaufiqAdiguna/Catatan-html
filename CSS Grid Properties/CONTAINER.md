# grid-template-colums
## Penjelasan
`grid-template-columns` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan lebar dari setiap kolom dalam grid. Properti ini memungkinkan Anda untuk secara fleksibel mendefinisikan lebar kolom dalam grid, baik secara absolut (dalam piksel, sentimeter, dll.) atau relatif (persentase dari lebar container atau fraksional).
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Template Columns</title>
    <style>
      .container {
        display: grid;
        grid-template-columns: 100px 200px 100px; /* Kolom pertama 100px, kolom kedua 200px, kolom ketiga 100px */
        gap: 10px; /* Jarak antara kolom */
      }
      .item {
        background-color: blue;
        padding: 20px;
        text-align: center;
      }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>
```
## Hasil Program
![hasil program grid template column](GTC.jpg)

# grid-template-row
## Penjelasan
`grid-template-rows` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan tinggi dari setiap baris dalam grid. Properti ini memungkinkan Anda untuk secara fleksibel mendefinisikan tinggi baris dalam grid, baik secara absolut (dalam piksel, sentimeter, dll.) atau relatif (persentase dari tinggi container atau fraksional).
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Template Rows</title>
    <style>
      .container {
        display: grid;
        grid-template-rows: 100px 200px 100px; /* Baris pertama 100px, baris kedua 200px, baris ketiga 100px */
        gap: 10px; /* Jarak antara baris */
        height: 500px; /* Tinggi container */
      }
      .item {
        background-color: aqua;
        padding: 20px;
        text-align: center;
      }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>
```
## Hasil Program
![hasil program grid template row](GTR.jpg)

# grid-auto-colums
## Penjelasan
`grid-auto-columns` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan lebar default kolom untuk elemen-elemen dalam grid yang tidak memiliki ukuran kolom yang ditentukan secara eksplisit.
## Kode Program
```HTML
<!DOCTYPE html>
<html>
<head>
    <title>Grid Auto Columns</title>
    <style>
      .container {
        display: grid;
        grid-template-columns: 100px; /* Kolom pertama 100px */
        grid-auto-columns: 200px; /* Lebar default kolom untuk elemen-elemen dalam grid */
        gap: 10px; /* Jarak antara kolom */
      }
      .item {
        background-color: #74f377;
        padding: 20px;
        text-align: center;
      }

    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>
```
## Hasil Program
![hasil program grid auto columns](GAC.jpg)

# grid-auto-rows
## Penjelasan
`grid-auto-rows` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan tinggi default baris untuk elemen-elemen dalam grid yang tidak memiliki ukuran baris yang ditentukan secara eksplisit. 
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Auto Rows</title>
    <style>
      .container {
        display: grid;
        grid-template-rows: 100px; /* Baris pertama 100px */
        grid-auto-rows: 200px; /* Tinggi default untuk baris-baris dalam grid */
        gap: 10px; /* Jarak antara baris */
      }
      .item {
        background-color: #f0f0f0;
        padding: 20px;
        text-align: center;
      }

    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>
```
## Hasil Program
![hasil program grid auto rows](GAR.jpg)
# grid-auto-flow
## Penjelasan
`grid-auto-flow` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan cara elemen-elemen baru ditempatkan dalam grid ketika elemen-elemen tersebut tidak memiliki area di grid yang didefinisikan secara eksplisit.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Auto Flow</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            grid-auto-flow: row; /* Elemen-elemen baru ditempatkan dalam baris baru */
            gap: 10px; /* Jarak antara elemen */
        }

        .item {
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
        <div class="item">5</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program grid auto flow](GAF.jpg)
# grid-template-areas
## Penjelasan
`grid-template-areas` adalah properti dalam CSS Grid Layout yang memungkinkan Anda untuk secara visual mendefinisikan tata letak grid dengan menggunakan nama area. Dengan grid-template-areas, Anda dapat dengan mudah membuat tata letak grid yang kompleks dengan menetapkan nama untuk setiap area dalam grid dan kemudian mendefinisikan tata letak menggunakan nama-nama tersebut.
## Kode Program
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Grid Template Areas</title>
    <style>
        .container {
            display: grid;
            grid-template-areas: 
                "header header header"
                "sidebar content content"
                "footer footer footer"; /* Definisi grid template areas */
            grid-template-rows: auto; /* Tinggi baris disesuaikan dengan konten */
            grid-template-columns: 200px 1fr 1fr; /* Lebar kolom pertama 200px, sisanya fr */
            gap: 10px; /* Jarak antara elemen */
        }

        .header {
            grid-area: header; /* Mengatur elemen dengan kelas .header di area header */
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }

        .sidebar {
            grid-area: sidebar; /* Mengatur elemen dengan kelas .sidebar di area sidebar */
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }

        .content {
            grid-area: content; /* Mengatur elemen dengan kelas .content di area content */
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }

        .footer {
            grid-area: footer; /* Mengatur elemen dengan kelas .footer di area footer */
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">Header</div>
        <div class="sidebar">Sidebar</div>
        <div class="content">Content</div>
        <div class="footer">Footer</div>
    </div>
</body>
</html>
```
## Hasil Program
![hasil program grid template areas](GTA.jpg)
# grid-template
## Penjelasan
`grid-template` adalah singkatan dari gabungan tiga properti dalam CSS Grid Layout: `grid-template-rows`, `grid-template-columns`, dan `grid-template-areas`. Properti ini digunakan untuk mendefinisikan tata letak grid secara lengkap dalam satu deklarasi.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Template</title>
    <style>
        .container {
            display: grid;
            grid-template:
                "header header header" 80px
                "sidebar content content" 200px
                "footer footer footer" 80px /
                1fr 2fr 1fr; /* Lebar kolom dalam fr */
            gap: 10px; /* Jarak antara sel */
        }

        .header, .sidebar, .content, .footer {
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">Header</div>
        <div class="sidebar">Sidebar</div>
        <div class="content">Content</div>
        <div class="footer">Footer</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program grid template](GT.jpg)
# grid-gap
## grid-column-gap
### Penjelasan
`grid-column-gap` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan jarak antara kolom-kolom dalam grid. Properti ini mengatur jarak horizontal antara kolom-kolom dalam grid container.
### Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Column Gap</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            grid-column-gap: 20px; /* Jarak antara kolom */
            gap: 10px; /* Jarak antara elemen */
        }

        .item {
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>

```
### Hasil Program
![hasil program grid column gap](GCG.jpg)

## grid-row-gap
### Penjelasan
`grid-row-gap` adalah properti dalam CSS Grid Layout yang digunakan untuk menentukan jarak antara baris-baris dalam grid. Properti ini mengatur jarak vertikal antara baris-baris dalam grid container.
### Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Grid Row Gap </title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            grid-template-rows: 100px 100px; /* Dua baris dengan tinggi 100px */
            grid-row-gap: 20px; /* Jarak antara baris 20px */
            gap: 10px; /* Jarak antara elemen */
        }

        .item {
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>
```
### Hasil Program
![hasil program grid row gap](GRG.jpg)
# justify-items
## Penjelasan
`justify-items` adalah properti dalam CSS Grid Layout yang digunakan untuk mengatur penempatan elemen-elemen di dalam sel grid secara horizontal. Properti ini mengontrol penempatan elemen-elemen di sepanjang sumbu baris dalam setiap sel grid.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Justify Items</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            justify-items: center; /* Elemen-elemen ditempatkan di tengah-tengah kolom */
            gap: 10px; /* Jarak antara elemen */
        }

        .item {
            background-color: #363b8f;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program justyfy items](JI.jpg)
# align-items
## Penjelasan
`align-items `adalah properti dalam CSS Grid Layout yang digunakan untuk mengatur penempatan elemen-elemen di dalam sel grid secara vertikal. Properti ini mengontrol penempatan elemen-elemen di sepanjang sumbu kolom dalam setiap sel grid.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Align Items</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            align-items: center; /* Elemen-elemen akan ditempatkan di tengah secara vertikal */
            height: 200px; /* Tinggi container */
        }

        .item {
            background-color: #755b5b;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program align items](AI.jpg)
# place-items
## Penjelasan
`place-items` adalah singkatan dari properti gabungan CSS Grid Layout yang digunakan untuk mengatur penempatan elemen-elemen di dalam sel grid secara horizontal dan vertikal secara bersamaan. Properti ini menggabungkan properti `justify-items` untuk mengatur penempatan horizontal dan `align-items` untuk mengatur penempatan vertikal.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Place Items </title>
    <style>
        .container {
            display: grid;
            place-items: center; /* Elemen-elemen ditempatkan di tengah container secara horizontal dan vertikal */
            width: 300px;
            height: 300px;
        }

        .item {
            background-color: #7bb78d;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program place items ](PI.jpg)
# justify-content
## Penjelasan
`justify-content` adalah properti dalam CSS Grid Layout yang digunakan untuk mengatur penempatan grid dalam container sepanjang sumbu baris. Properti ini mengontrol penempatan grid secara horizontal dalam container.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Justify Content</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: repeat(3, 100px); /* Tiga kolom dengan lebar 100px */
            justify-content: center; /* Grid ditempatkan di tengah-tengah container secara horizontal */
            gap: 10px; /* Jarak antara kolom */
        }

        .item {
            background-color: #471c54;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program justyfy content ](JC.jpg)
# align-content
## Penjelasan
`align-content` adalah properti dalam CSS Grid Layout yang digunakan untuk mengatur penempatan grid dalam container sepanjang sumbu kolom. Properti ini mengontrol penempatan grid secara vertikal dalam container.
## Kode Program
```html
<!DOCTYPE html>
<html>
<head>
    <title>Align Content</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            grid-template-rows: 100px 100px; /* Dua baris dengan tinggi 100px */
            align-content: center; /* Menengahkan grid secara vertikal dalam container */
            gap: 10px; /* Jarak antara elemen */
            height: 300px; /* Tinggi container */
        }

        .item {
            background-color: #931931;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program align content ](AC.jpg)
# place-content
## Penjelasan
`place-content `adalah singkatan dari properti gabungan CSS Grid Layout yang digunakan untuk mengatur penempatan grid dalam container secara horizontal dan vertikal secara bersamaan. Properti ini menggabungkan properti `justify-content` untuk mengatur penempatan horizontal dan `align-content` untuk mengatur penempatan vertikal.
## Kode Program
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Place Content</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 100px 100px; /* Dua kolom dengan lebar 100px */
            grid-template-rows: 100px 100px; /* Dua baris dengan tinggi 100px */
            place-content: center; /* Elemen-elemen ditempatkan di tengah container secara horizontal dan vertikal */
            gap: 10px; /* Jarak antara elemen */
            height: 300px; /* Tinggi container */
        }

        .item {
            background-color: #f0f0f0;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>

```
## Hasil Program
![hasil program place content ](PC.jpg)