# Definisi HTML

HTML (Hypertext Markup Language) merupakan bahasa markup yang digunakan untuk menentukan konten dan
struktur halaman web.

Elemen dalam dokumen HTML ditunjukkan dengan menggunakan tag.

Penulisan tag HTML seperti di bawah ini:

```html
<tag>text</tag>
```

Beberapa tag memiliki teks tambahan di dalamnya yang memberikan informasi tambahan tentang tag; disebut dengan atribut.

```html
<tag atribut1="nilai1" atribut2="nilai2"> text </tag>
```

Nama tag boleh ditulis dengan huruf kecil, huruf kapital, ataupun kombinasi antara huruf kecil dan huruf kapital.

Teks editor untuk membuat file HTML diantaranya:
- ![Notepad++](https://img.shields.io/badge/Notepad++-90E59A.svg?style=for-the-badge&logo=notepad%2B%2B&logoColor=black)
- ![SublimeText](https://img.shields.io/badge/sublime_text-%23575757.svg?&style=for-the-badge&logo=sublime-text&logoColor=important)
- ![Visual Studio Code](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)

## Definisi HTML

## Apa itu HTML?

- HTML adalah *HyperText Markup Language*.
- HTML adalah bahasa markup standard untuk membuat halaman Web.
- HTML mendeskripsikan struktur halaman Web.
- HTML terdiri dari serangkaian elemen.
- Elemen HTML memberi tahu browser cara menampilkan konten.
- Elemen HTML memberi label potongan konten seperti "ini adalah judul", "ini adalah paragraf", "ini adalah tautan", dll.

### Dokumen Simple HTML

Contoh ke [HTMLIntroduction.html](HTMLIntroduction.html)

**Contoh Dijelaskan:**

- Deklarasi `<!DOCTYPE html>` mendefinisikan bahwa dokumen ini adalah dokumen HTML5
- Elemen `<html>` adalah elemen root dari halaman HTML
- Elemen `<head>` berisi informasi meta tentang halaman HTML
- Elemen `<title>` menentukan judul untuk halaman HTML (yang ditampilkan di bilah judul browser atau di tab halaman)
- Elemen `<body>` mendefinisikan isi dokumen, dan merupakan wadah untuk semua konten yang terlihat, seperti judul, paragraf, gambar, hyperlink, tabel, daftar, dll.
- Elemen `<h1>` mendefinisikan heading besar
- Elemen `<p>` mendefinisikan paragraf.

## Apa itu Elemen HTML?

Elemen HTML didefinisikan oleh tag awal, beberapa konten, dan tag akhir:
```html
<tagname>Konten ada di sini...</tagname>
```

Elemen HTML adalah segalanya mulai dari tag awal hingga tag akhir:
```html
<h1>Judul Pertama Saya</h1>
<p>Paragraf pertama saya.</p>
```

|     | Tag Awal |     Konten Elemen     | Tag terakhir |
| :-: | :------: | :-------------------: | ------------ |
| 01  |   `<h1>`   | Heading Pertama Saya  | `</h1>`        |
| 02  |   `<p>`    | Paragraf Pertama Saya | `</p>`         |
| 03  |   `<br>`   |         None          | None         |

> **Catatan:** Beberapa elemen HTML tidak memiliki konten (seperti elemen `<br>`). Elemen-elemen ini disebut elemen kosong. Elemen kosong tidak memiliki tag akhir!
## Web Browser

Tujuan browser web (Chrome, Edge, Firefox, Safari) adalah untuk membaca dokumen HTML dan menampilkannya dengan benar.

Browser tidak menampilkan tag HTML, tetapi menggunakannya untuk menentukan cara menampilkan dokumen:

### Struktur Halaman HTML

Di bawah ini adalah visualisasi struktur halaman HTML:

**Catatan:** Konten di dalam bagian `<body>` (area putih di atas) akan ditampilkan di browser. Konten di dalam elemen `<title>` akan ditampilkan di bilah judul browser atau di tab halaman.

## Sejarah HTML

Sejak awal World Wide Web, ada banyak versi HTML:

|     | Tahun |                  Versi                  |
| :-: | :---: | :-------------------------------------: |
| 01  | 1989  |      Tim Berners-Lee invented www       |
| 02  | 1991  |      Tim Berners-Lee invented HTML      |
| 03  | 1993  |       Dave Raggett drafted HTML+        |
| 04  | 1995  |   HTML Working Group defined HTML 2.0   |
| 05  | 1997  |      W3C Recommendation: HTML 3.2       |
| 06  | 1999  |      W3C Recommendation: HTML 4.01      |
| 07  | 2000  |      W3C Recommendation: XHTML 1.0      |
| 08  | 2008  |     WHATWG HTML5 First Public Draft     |
| 09  | 2012  |      WHATWG HTML5 Living Standard       |
| 10  | 2014  |        W3C Recommendation: HTML5        |
| 11  | 2016  | W3C Candidate Recommendation: HTML 5.1  |
| 12  | 2017  | W3C Recommendation: HTML5.1 2nd Edition |
| 13  | 2017  |       W3C Recommendation: HTML5.2       |

# HTML Basic

## Dokumen HTML

* Dokumen **HTML** harus dimulai dengan deklarasi tipe dokumen `<!DOCTYPE html>`
* Dokumen **HTML** harus mempunyai tag `html`. Dimulai dengan tag pembuka `<html>` dan diakhiri dengan tag penutup  `</html>`
* Dokumen **HTML** harus mempunyai tag `head`. Dimulai dengan tag pembuka `<head>` dan diakhiri dengan tag penutup `</head>`
* Dokumen **HTML** harus mempunyai tag `body`. Dimulai dengan tag pembuka  `<body` dan di akhiri dengan tag penutup `</body>`
* Element **HTML** harus terletak di dalam tag `body`

    Contoh Dokumen HTML:

    ```html
    <!DOCTYPE html>
    <html lang="en">
        <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Hello World</title>
        </head>
        <body>
        <!--Masukan Element HTML di dalam tag body -->
        <h1>Hello World</h1>
        <p>Halo Dunia</p>
        </body>
    </html>
    ```

    # Elemen HTML

## Apa itu Elemen dalam HTML ?

Elemen __HTML__  bisa dikatakan segalanya mulai dari tag awal hingga tag akhir. Elemen __HTML__ didefinisikan oleh tag awal. Jika elemen berisi konten lain, itu diakhiri dengan tag penutup, di mana nama elemen didahului oleh garis miring seperti yang ditunjukkan di bawah ini dengan beberapa tag.

## Contoh Elemen HTML

```html
<p>Elemen HTML</p>
<div>Ini adalah Elemen HTML</div>
```

Keterangan:
| Konten   | Tag Pembuka | Tag Penutup |
| -------- | :---------: | :---------: |
| Paragraf |    `<p>`    |   `</p>`    |
| Divisi   |   `<div>`   |  `</div>`   |

Jadi di sini ada dua elemen HTML yaitu, elemen `<p>...</p>` dan elemen `<div>...</div>`. Ada beberapa elemen yang tidak memerlukan tag __penutup__ seperti `<img>`, `<br>`, `<hr>`, `<input>`, dll.

## HTML Attribute

### Apa Itu HtML Attribute ?

HTML Attribute adalah suatu atribut untuk melengkapi informasi dari suatu elemen HTML

- Semua elemen HTML dapat memiliki Attribute.
- Attribute HtML memberikan informasi tambahan terhadap elemen HTML.
- Attribute selalu berada diawal tag, seperti:

  ```html
  <a href="google.com">Google</a>
  ```

- Attribute selalu berbapasangan dengan value/nilai, seperti: `href="google.com"`
- Value/Nilai dari attribute harus selalu dibungkus menggunakan double quote/petik dua (").

### Contoh Penerapan Attribute Pada HTML

#### `href` Attribute

`href` berfungsi untuk menentukan URL halaman yang ingin dituju.

```html
<html>
  <a href="Github.com">Github Website</a>
</html>
```

#### `src` Attribute

`src` berfungsi untuk menentukan lokasi gambar file yang ingin ditampilkan.

```html
<html>
  <img src="attribute.png" />
</html>
```

Ada dua cara untuk mendefinisikan URL di attribute `src`

1. Absolute URL - Memasukan gambar dari hosting eksternal/tidak dalam local, seperti:

    ```html
    <img src="https://avatars.githubusercontent.com/u/76999048?s=200&v=4" >
    ```

2. Relative URL

    ```html
    <img src="/src/images/avatar.png" >
    ```

#### `width` & `height` Attribute

`width` dan `height` berfungsi untuk menentukan lebar dan tinggi gambar dalam satuan piksel (px).

```html
<img src="/src/images/avatar.png" width="32" height="32" />
```

#### `alt` Attribute

`alt` berfungsi untuk menggantikan gambar dengan tulisan, jika gambar tidak bisa ditampilkan dengan alasan tertentu.

```html
<img src="/src/images/avatar.png" alt="avatar" />
```

#### `style` Attribute

`style` berfungsi untuk menambahkan gaya/style pada elemen seperti color, font, size, dan lainnya.

```html
<h1 style="color: green">Hello World</h1>
```

#### `lang` Attribute

`lang` berfungsi untuk mendeklarasikan bahasa yang digunakan dalam website, untuk membantu mesin pencari / browser.

```html
<!DOCTYPE html>
<html lang="en">
  <body>
    Hello World
  </body>
</html>
```

#### `title` Attribute

`title` berfungsi sebagai penambah informasi dalam suatu elemen, yang jika dihover akan memunculkan tooltip

```html
<span title="Komunitas untuk mengelola dan menulis kode">Bellshade</span>
```

#### `class` Attribute

`class` berfungsi untuk menunjuk nama class dalam style sheet, dapat digunakan untuk mengakses dan memanipulasi elemen di Javascript.

```html
<div class="kota">
  <p>Jakarta terletak di pulau Jawa, Indonesia.</p>
</div>
```

#### `id` Attribute

`id` berfungsi untuk menentukan id unik untuk elemen HTML, dapat digunakan untuk menunjuk deklarasi style tertentu dalam style sheet dan juga digunakan untuk mengakses dan memanipulasi elemen dengan id tertentu di Javascript.

```html
<html>
  <h1 id="judulSaya">Judul Saya</h1>
</html>
```

#### `method` Attribute

`method` berfungsi untuk menentukan cara mengirim data formulir (data formulir dikirim ke halaman yang ditentukan dalam atribut action).

Form-data dapat dikirim sebagai variabel URL (dengan `method="get"`) atau sebagai transaksi posting HTTP (dengan method="post").

Catatan tentang [GET](https://github.com/bellshade/PHP/tree/main/basics/9_form_handling):

- Menambahkan data formulir ke dalam URL dalam pasangan nama/nilai
- Panjang URL dibatasi (sekitar 3000 karakter)
- Jangan pernah menggunakan `GET` untuk mengirim data sensitif! (akan terlihat di URL)
- Berguna untuk pengiriman formulir di mana pengguna ingin menandai hasilnya
- `GET` lebih baik untuk data yang tidak aman, seperti string kueri di Google

```html
<form action="/action_page.php" method="get">
  Nama Depan: <input type="text" name="namaDepan" /><br />
  Nama Belakang: <input type="text" name="namaBelakang" /><br />
  <input type="submit" value="Submit" />
</form>
```

Catatan tentang [POST](https://github.com/bellshade/PHP/tree/main/basics/9_form_handling):

- Menambahkan formulir-data di dalam isi permintaan HTTP (data tidak ditampilkan dalam URL)
- Tidak memiliki batasan ukuran
- Pengiriman formulir dengan `POST` tidak dapat di-bookmark

```html
<form action="/action_page.php" method="post">
  Nama: <input type="text" name="nama" /><br />
  Password: <input type="text" name="password" /><br />
  <input type="submit" value="Submit" />
</form>
```
