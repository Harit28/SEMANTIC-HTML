# SEMANTIC-HTML
Latihan Praktikum Semantic HTML

## Latihan 1 : Semantic HTML

## Menganalisis Kode Index.html

1. **Deklarasi DOC TYPE**
   - Baris pertama menggunakan `<!DOCTYPE html>` ,yang menunjukkan bahwa dokumen ini adalah HTML5.

2. **Elemen `<html`**
   - Atribut `lang='en'` digunakan untuk mennetukan bahwa dokumen ini adalah bahasa inggris.

3. **Bagian `<head>`**
   - `<meta charset="UTF-8"` memastikan karakter yang digunakan adalah UTF-8, yang mendukung berbagai karakter dari berbagai bahasa
   - `<meta name="viewport" content='width=device-width, initial-scale=1.0">` memberikan responsivitas pada halaman, sehingga tampilannya dapat mneyesuaikan dengan ukuran layar perangkat.
   - `title>HTML5 Semantic</title>` memberikan judul pada halaman web, yang akan tampil di tab browser.
   - `<link rel="stylesheet" href="../assets/styles/styles.css">` untuk menyertakan stylesheet eksternal yang mengarah ke direktori `assets/styles/styles.cc`
4. **Bagian `<body>`:
   - Elemen `<header> :
     - Didalam `<header>`, terdapat `<h1>` dengan teks "HTML5 Semantic" ini merupakan judul utama dari halaman
   - Elemen `<nav>` :
     - `<nav>` digunakan untuk menampung menu navigasi,ini merupakan elemen semnatik yang menunjukkan bagian navigasi dari halaman
     - Didalam `<nav>` terdapat daftra tak berurutan `<ul>` dengan beberapa item `<li>`, masing- masing berisi tautan `<a>` yang mengarahkan ke berbagai bagian hal melalui `href` berisi id (#home,#pengertian,#kesimpulan). Ini adalah navigasi internal
   - Elemen `<section>` :
     - `<section>` berfungsi untuk menanmpung konten utama dari halaman. Disini berisi "KONTEN"
   - Elemen `<footer>` :
     - `<footer>` digunakan untuk menampilkan informasi penutup, dalam hal ini berisi teks "Copyright" yang berada dibawah halaman


## Menganalisis Kode style.css

1. **Elemen Global: `<body>`
   - `display: grid;` untuk menentukan bahwa elemen `<body>` menguunakan model tata letak grid
   - `grid-template-areas` membuat area tata letak grid dengan nama spesifik untuk setiap bagian :
     - Baris pertama : "header header header" (header mengambil seluruh baris pertama)
     - Baris kedua : "nav section section" (navigasi mengambil 20% lebar disebelah kiri, sedangkan konten utama mengambil 1fr dan sisanya 18%)
     - Baris ketiga: "footer footer footer" (footer mengambil seluruh baris terakhir)
   - `grid-template-columns:` Mengatur lebar kolom :
     - Kolom pertama (nav) : 20% dari lebar layar
     - Kolom kedua (konten utama) : 1fr (fleksibel,mengisi ruang sisa)
     - Kolom ketiga : 18%
   - `grid-gap: 5px;` Memeberikan jarak 5px diantar grid (baik horizaontal maupun vertikal)
   - `height: 100vh;` Mengatur tinggi total grid agar sama dengan tinggi layar browser (viewport height)
2. **Elemen Styling Khusus
   - Semua elemen (`header`, `nav`, `section`, `footer`) memiliki `padding: 5px;` untuk memeberi jarak dalam elemen
   - `header`
     - `background: #707070;` : warna latar belakan abu-abu gelap
     - `grid-area: header;` : ditetapkan sebagai area header dalam grid (sesuai `grid-template-areas`
     - `text-align: center;` : teks didalam header diatur rata tengah
   - `nav`
     - `background: #C9BFBF;` : warna latar belakang abu-abu muda
     - `grid-area: nav;` : ditetapkan sebagai area navigasi (sesaui `grid-template-areas`)
   - `section`
     - `background: #ABABAB;` : Warna latar belakang abu-abu sedang
     - `grid-area: section;` : ditetapkan sebgai area konten utama sesuai `grid-template-areas`
   - `footer`
     - `background: #707070;` : warna latar belakang abu_abu gelap, sama seperti header
     - `grid-area: footer;` : ditetapkan sebagai area footer sesuai `grid-template-areas`
     - `font-size: small` : ukuran font kecil untuk teks dalam footer
     - `text-align: center` : tekas didalam footer diatu rata tengah 


   
   
