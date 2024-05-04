# HTML, CSS dan JavaScript
### Bahasa pemrograman dasar yang digunakan dalam pembuatan website dan aplikasi lainnya
## 1. HTML (Hypertext Markup Language):
>HTML adalah bahasa markah standar yang digunakan untuk membuat dan merancang halaman web. 

 HTML memberikan struktur dasar dari suatu halaman web dengan menggunakan elemen-elemen seperti tag, atribut, dan konten untuk menampilkan informasi secara terstruktur. Ini adalah bahasa dasar untuk membuat konten web.
 
#### Berikut contoh tag-tag dasar HTML beserta penggunaanya:
 ```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Metadata dan karakter set -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Judul halaman -->
    <title>Contoh Halaman Web</title>
</head>
<body>
    <!-- Judul Utama -->
    <h1>Judul Utama</h1>
    <!-- Paragraf teks -->
    <p>Ini adalah paragraf teks yang terletak di dalam body.</p>
    
    <!-- Sub Judul -->
    <h2>Sub Judul</h2>
    <!-- Daftar tak terurut -->
    <ul>
        <!-- Item dalam daftar tak terurut -->
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ul>
    
    <!-- Sub Sub Judul -->
    <h3>Sub Sub Judul</h3>
    <!-- Daftar terurut -->
    <ol>
        <!-- Item dalam daftar terurut -->
        <li>Item A</li>
        <li>Item B</li>
        <li>Item C</li>
    </ol>
    
    <!-- Kontainer blok -->
    <div>
        <!-- Paragraf dan gambar di dalam div -->
        <p>Ini adalah paragraf di dalam div.</p>
        <img src="gambar.jpg" alt="Deskripsi gambar">
    </div>
    
    <!-- Paragraf lain di dalam body -->
    <p>Ini adalah paragraf lain di dalam body.</p>
    
    <!-- Tautan atau hyperlink -->
    <a href="https://www.contoh.com">Tautan</a>
</body>
</html>

```

Itu adalah struktur dasar dari sebuah halaman web HTML. Kita dapat melihat penggunaan tag-tag seperti 
``` <html>, <head>, <title>, <meta>, <body>, <h1> sampai <h3>, <p>, <ul> dan <li>, <ol> dan <li>, <div>, <img>, dan <a>.```

#### Contoh penggunaan HTML dalam pembuatan halaman web sederhana
```sh

<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Metadata dan karakter set -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Judul halaman -->
    <title>Contoh Halaman Web</title>
    <!-- Link CSS eksternal -->
    <link rel="stylesheet" href="style.css">
    <!-- Inline CSS -->
    <style>
        /* Gaya khusus untuk halaman ini */
        body {
            background-color: lightblue;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <!-- Logo -->
        <img src="logo.png" alt="Logo">
        <!-- Judul header -->
        <h1>Selamat Datang</h1>
        <!-- Navigasi -->
        <nav>
            <ul>
                <!-- Tautan navigasi -->
                <li><a href="#home">Beranda</a></li>
                <li><a href="#about">Tentang Kami</a></li>
                <li><a href="#services">Layanan</a></li>
                <li><a href="#contact">Kontak</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Main content -->
    <main>
        <!-- Section 1: Tentang Kami -->
        <section id="about">
            <!-- Sub judul -->
            <h2>Tentang Kami</h2>
            <!-- Paragraf -->
            <p>Kami adalah perusahaan yang bergerak di bidang teknologi informasi.</p>
            <!-- Gambar -->
            <img src="about.jpg" alt="Tentang Kami">
        </section>
        
        <!-- Section 2: Layanan -->
        <section id="services">
            <!-- Sub judul -->
            <h2>Layanan</h2>
            <!-- Daftar terurut -->
            <ol>
                <!-- Item dalam daftar -->
                <li>Pembuatan Website</li>
                <li>Pengembangan Aplikasi Mobile</li>
                <li>Konsultasi IT</li>
            </ol>
        </section>
        
        <!-- Section 3: Kontak -->
        <section id="contact">
            <!-- Sub judul -->
            <h2>Kontak</h2>
            <!-- Formulir kontak -->
            <form action="submit.php" method="post">
                <!-- Input nama -->
                <label for="name">Nama:</label>
                <input type="text" id="name" name="name" required>
                <!-- Input email -->
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                <!-- Tombol submit -->
                <button type="submit">Kirim</button>
            </form>
        </section>
    </main>
    
    <!-- Footer -->
    <footer>
        <!-- Copyright -->
        <p>&copy; 2024 Contoh Company. All rights reserved.</p>
    </footer>
</body>
</html>
```
#### Hasil
![Screenshot 2024-05-04 085617](https://github.com/rizqinrr/pemograman-web1/assets/152271198/b4afd71b-0a28-42aa-a801-af3520cf0062)



## 2. CSS (Cascading Style Sheets):
>CSS adalah bahasa gaya yang digunakan untuk mengatur tampilan dan penataan dari elemen-elemen HTML di dalam halaman web. 

Dengan CSS, kita dapat mengontrol warna, ukuran, font, tata letak, dan berbagai aspek visual lainnya dari suatu halaman web. Ini memungkinkan pemisahan antara struktur dan gaya dari halaman web, yang memungkinkan fleksibilitas dan konsistensi dalam desain.
[![N|Solid](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://www.w3schools.com/css/)

#### Contoh penggunaan CSS dalam halaman HTML sederhana
```sh
/* Selektor Universal */
* {
    margin: 0; /* Menghilangkan margin */
    padding: 0; /* Menghilangkan padding */
    box-sizing: border-box; /* Memastikan ukuran elemen termasuk border dan padding */
}

/* Selektor Elemen */
h1 {
    font-size: 24px; /* Ukuran font */
    color: #333; /* Warna teks */
}

/* Selektor ID */
#header {
    background-color: #f2f2f2; /* Warna latar belakang */
    padding: 20px; /* Padding */
}

/* Selektor Kelas */
.paragraf {
    font-style: italic; /* Gaya font */
    line-height: 1.5; /* Tinggi baris */
}

/* Pseudoselektor */
a:hover {
    text-decoration: underline; /* Garis bawah saat dihover */
    color: #FF0000; /* Warna teks saat dihover */
}

/* Komentar */
/* Ini adalah contoh komentar dalam CSS */

```
#### Penjelasan Fungsi Setiap Tag:

- Selektor Universal (*):
Mengatur properti CSS yang berlaku untuk semua elemen dalam halaman HTML, seperti menghilangkan margin dan padding, serta memastikan ukuran elemen termasuk border dan padding.
- Selektor Elemen (h1):
Mengatur gaya untuk elemen ```<h1>```, seperti ukuran font dan warna teks.
- Selektor ID (#header):
Mengatur gaya untuk elemen dengan ID "header", seperti warna latar belakang dan padding.
- Selektor Kelas (.paragraf):
Mengatur gaya untuk elemen dengan kelas "paragraf", seperti gaya font dan tinggi baris.
- Pseudoselektor (a:hover):
Mengatur gaya untuk tautan saat dihover, seperti menambahkan garis bawah dan mengubah warna teks.
- Komentar:
Menambahkan komentar dalam CSS untuk memberikan penjelasan atau dokumentasi pada kode. Komentar tidak memengaruhi tampilan halaman web dan hanya untuk referensi pengembang.

#### Selain selektor, terdapat juga properti-properti CSS yang digunakan untuk mengatur tampilan elemen, di antaranya:
| CSS | Fungsi |
| ------ | ------ |
| Color | Mengatur warna teks. |
| Background-color | Mengatur warna latar belakang. |
| Font-family | Mengatur jenis font.|
| Font-size | Mengatur ukuran font. |
| Font-weight | Mengatur ketebalan font. |
| Text-align | Mengatur penataan teks |
| Margin | Mengatur jarak antara elemen dengan elemen lain di luarnya. |
| Padding | Mengatur jarak antara isi elemen dan batasnya |
| Border | Mengatur border elemen. |
| Width dan Height | Mengatur lebar dan tinggi elemen. |
| Display| Mengatur tampilan elemen, seperti block, inline, atau inline-block. |

Ini hanya sebagian kecil dari tag-tag dan properti-properti CSS yang tersedia. CSS sangat luas dan fleksibel, memungkinkan pengembang web untuk mengontrol tampilan halaman web dengan sangat detail.

## 3. JavaScript:
>JavaScript adalah bahasa pemrograman yang digunakan untuk memberikan interaktivitas dan dinamika pada halaman web. 

Dengan JavaScript, Anda dapat menambahkan fungsionalitas seperti validasi formulir, animasi, manipulasi DOM (Document Object Model), dan responsif terhadap tindakan pengguna seperti klik dan geser. Ini memungkinkan pembuatan aplikasi web yang lebih interaktif dan dinamis. JavaScript adalah salah satu dari tiga teknologi inti dalam pengembangan web, bersama dengan HTML dan CSS.
[![Build Status](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://www.javascript.com/)

#### Contoh syntax JavaScript dan Funsinya
```sh
// Variabel
var nama = "John"; // Deklarasi variabel 'nama' dengan nilai string "John"
let umur = 30; // Deklarasi variabel 'umur' dengan nilai number 30
const PI = 3.14; // Deklarasi konstanta 'PI' dengan nilai number 3.14

// Penulisan Komentar
// Ini adalah contoh komentar satu baris
/* Ini adalah contoh komentar
   multi-baris */

// Tipe Data
let angka = 10; // Tipe data number
let teks = "Halo"; // Tipe data string
let benar = true; // Tipe data boolean
let array = [1, 2, 3]; // Tipe data array
let objek = { nama: "John", umur: 30 }; // Tipe data object
let kosong = null; // Tipe data null
let tidakDitentukan; // Tipe data undefined

// Operasi Aritmatika
let hasilPenjumlahan = 5 + 3; // Penjumlahan
let hasilPengurangan = 5 - 3; // Pengurangan
let hasilPerkalian = 5 * 3; // Perkalian
let hasilPembagian = 5 / 3; // Pembagian
let hasilModulus = 5 % 3; // Modulus (sisa pembagian)

// Pengkondisian (if-else)
let angka1 = 10;
let angka2 = 20;
if (angka1 > angka2) {
    console.log("Angka1 lebih besar dari Angka2"); // Jika angka1 lebih besar dari angka2
} else if (angka1 < angka2) {
    console.log("Angka1 lebih kecil dari Angka2"); // Jika angka1 lebih kecil dari angka2
} else {
    console.log("Angka1 sama dengan Angka2"); // Jika angka1 sama dengan angka2
}

// Perulangan (for)
for (let i = 0; i < 5; i++) {
    console.log("Perulangan ke-" + (i + 1)); // Menampilkan pesan perulangan
}

// Fungsi
function tambah(a, b) {
    return a + b; // Mengembalikan hasil penjumlahan dari dua parameter
}
let hasil = tambah(3, 4); // Memanggil fungsi tambah dengan argumen 3 dan 4
console.log("Hasil penjumlahan: " + hasil); // Menampilkan hasil penjumlahan

```
Di atas ini hanya beberapa dari banyak fitur dan sintaksis dalam JavaScript. JS sangat fleksibel dan kuat, memungkinkan untuk membuat berbagai aplikasi web yang interaktif dan dinamis.

##### Berikut adalah beberapa hal yang dapat dilakukan menggunakan JavaScript pada sebuah website:
- Manipulasi DOM (Document Object Model):
JavaScript dapat digunakan untuk menambah, menghapus, atau mengubah elemen-elemen HTML, CSS, dan konten halaman secara dinamis.
Ini memungkinkan pembuatan efek animasi, perubahan tampilan, dan penyesuaian layout halaman secara real-time.
- Interaksi Pengguna:
JavaScript memungkinkan interaksi dengan pengguna melalui berbagai elemen seperti formulir, tombol, dan tautan.
Hal ini memungkinkan validasi formulir, respon terhadap input pengguna, dan navigasi halaman yang lebih dinamis.
- Manipulasi Data:
JavaScript dapat digunakan untuk mengambil, mengubah, dan menyimpan data secara dinamis pada website.
Data dapat dimuat secara asinkron melalui teknik seperti AJAX untuk meningkatkan kinerja dan responsivitas website.
- Animasi dan Efek Visual:
JavaScript memungkinkan pembuatan animasi dan efek visual yang menarik untuk meningkatkan pengalaman pengguna.
Ini termasuk animasi transisi, efek hover, parallax scrolling, dan banyak lagi.
- Validasi Formulir:
JavaScript dapat digunakan untuk melakukan validasi formulir pada sisi klien sebelum data dikirim ke server.
Ini memungkinkan deteksi kesalahan input sebelum pengguna mengirimkan data, meningkatkan pengalaman pengguna.
- Manipulasi Cookie dan Local Storage:
JavaScript dapat digunakan untuk menyimpan data pada browser pengguna, baik menggunakan cookie atau local storage.
Hal ini memungkinkan penyimpanan preferensi pengguna, data sesi, dan informasi lainnya untuk penggunaan berikutnya.
- Komunikasi dengan Server:
JavaScript dapat digunakan untuk berkomunikasi dengan server secara asinkron melalui teknik seperti AJAX (Asynchronous JavaScript and XML).
Ini memungkinkan pembaruan halaman tanpa harus me-refresh seluruh halaman, meningkatkan responsivitas dan pengalaman pengguna.
- Pembuatan Aplikasi Web Interaktif:
Dengan semua kemampuan di atas, JavaScript memungkinkan pembuatan aplikasi web yang interaktif dan responsif.
Hal ini termasuk game online, aplikasi produktivitas, layanan web real-time, dan banyak lagi.

# Contoh Penggunaannya Dalam Landing Page Sederhana 
![Screenshot 2024-05-04 092546](https://github.com/rizqinrr/pemograman-web1/assets/152271198/8d0859be-18af-404b-8182-bc5c24fadc4c)

>Muhammad Rizqi Nurahman
