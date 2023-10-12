<h1 <p align="center"><b>Praktikum 3</b></p></h1> 

<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Rini Ariza</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210337</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A3</td>
  </tr>
</table>

---

## Membuat dokumen HTML

Persiapan membuat dokumen HTML dengan nama file **lab3_list.html** seperti berikut.

```html
<!DOCTYPE html>
<html lang="en"
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="widht=device-width,initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>membuat list</h1>
    </header>
</body>
</html>

```

---

## Membuat Ordered List

Kemudian tambahkan kode untuk membuat *Ordered List* seperti berikut.

```html
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
    </ol>
</section>

```

![Screenshot (295)](https://github.com/rniarzz/Lab3web/assets/115542704/5a88f1fc-f8ba-4006-ad07-49e56442071b)

---

## Membuat Unorderd List

Kemudian tambakan kode untuk membuat *Unordered List*, setelah deklarasi ordered list pada
section unordered-list, seperti berikut.

```html
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

![Screenshot (296)](https://github.com/rniarzz/Lab3web/assets/115542704/1f70d1b9-7558-431e-9092-815f8737eb7e)

---

## Membuat Description List
Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.

```html
<section id="unorder-list">
    <h2>Description List</h2>
    <dl>
        <dt>Fakultas Teknik</dt>
        <dd>Teknik Industri</dd>
        <dd>Teknik Informatika</dd>
        <dd>Teknik Lingkungan</dd>
        <dt>Fakultas Ekonomi dan Bisnis</dt>
        <dd>Akuntansi</dd>
        <dd>Manajemen</dd>
        <dd>Bisnis Digital</dd>
    </dl>
</section>
```

![Screenshot (297)](https://github.com/rniarzz/Lab3web/assets/115542704/4a263429-65fd-40ca-ad79-c6dc0b791ffb)

---

## Membuat Tabel
Buat file baru dengan nama **lab3_tabel.html** seperti berikut.

```html
<!DOCTYPE html>
<html lang="en"
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="widht=device-width,initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>
</body>
</html>
```

Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:

```html
<table border="1" cellpadding="4" cellspacing="0">
    <thead>
        <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik</td>
            <td>Teknik Industri</td>
         </tr>
        <tr>
            <td>3.</td>
            <td>Teknik</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```

## Mengatur Margin dan Padding

Untuk mengatur margin dan padding pada cel data, tambahkan atribut `cellpadding` dan `cellspacing` pada tag table.

![Screenshot (298)](https://github.com/rniarzz/Lab3web/assets/115542704/f357e4f9-121c-4f5f-9a9e-3f2443aa7168)

---

## Menggabungkan Sel Data
Untuk menggabungkan sel data, gunakan atribut `rowspan` dan `colspan`. Atribut `rowspan` untuk
menggabungkan baris (secara vertikal) dan `colspan` untuk menggabungkan kolom (secara
horizontal).

```html
<body>
    <header>
        <h1>Menggabungkan Sel</h1>
    </header>
</body>

<table border="1" cellpadding="6" cellspacing="0">
    <thead>
        <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td rowspan="3">Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```

![Screenshot (299)](https://github.com/rniarzz/Lab3web/assets/115542704/5c682785-d0f8-4b2c-adfb-2d60d17ed824)

---

## Membuat Form
Buat file baru dengan nama **lab3_form.html** seperti berikut.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```

Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:

```html
<form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
        <p>
            <label for="nama">Nama</label>
            <input type="text" id="nama" name="nama">
        </p>
        <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </p>
        <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L" /><label
for="jk_l">Laki-laki</label>
        <input id="jk_p" type="radio" name="kelamin" value="P" /><label
for="jk_p">Perempuan</label>
    </p>
    <p><input type="submit" value="Login"></p>
    </fieldset>
</form>
```

![Screenshot (300)](https://github.com/rniarzz/Lab3web/assets/115542704/baba5366-11d5-46db-bed1-66759bd774f3)

---

## Menambahkan Style pada Form
Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.

```html
<style>
    form p > label {
        display: inline-block;
        width: 100px;
    }
    form input[type="text"], form textarea {
        border: 1px solid #197a43;
    }
    form input[type="submit"] {
        border: 1px solid #197a43;
        background-color: #197a43;
        color: #ffffff;
        font-weight: bold;
    padding: 5px 15px;
    }
    </style>
```

![Screenshot (302)](https://github.com/rniarzz/Lab3web/assets/115542704/2c62c116-30ae-4901-90c1-dbc0afd74cbd)

---

## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan ***dropdown*** menu dan ***listbox*** dengan *multiple selection*.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tugas 3</title>
    <style>
        /* CSS untuk styling */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 400px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }
        label {
            display: block;
            margin-bottom: 10px;
        }
        input[type="text"],
        input[type="email"],
        select,
        select[multiple] {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        select[multiple] {
            height: auto;
        }
        button {
            background-color: #007BFF;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Formulir Contoh</h2>
        <form action="#" method="post">
            <label for="nama">Nama:</label>
            <input type="text" id="nama" name="nama" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="pilihan">Jurusan:</label>
            <select id="pilihan" name="pilihan">
                <option value="opsi1">Teknik Informatika</option>
                <option value="opsi2">Manajemen</option>
                <option value="opsi3">Hukum</option>
            </select>

            <label for="multipleSelect">Pilih hobby anda:</label>
            <select id="multipleSelect" name="multipleSelect[]" multiple>
                <option value="opsi1">Bola</option>
                <option value="opsi2">Berenang</option>
                <option value="opsi3">Membaca</option>
                <option value="opsi4">Melukis</option>
                <option value="opsi5">Mendengarkan musik</option>
                <option value="opsi6">Shooping</option>
            </select>

            <button type="submit">Submit</button>
        </form>
```

---

## Hasil Run

![Screenshot (303)](https://github.com/rniarzz/Lab3web/assets/115542704/dc376689-73a3-4276-bbe5-aefd7c4191d9)

