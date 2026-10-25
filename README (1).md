# Catatan HTML Kuroneko - Bagian 1: Home dan Syntax

Mulai belajar: 14 Maret 2019
Catatan ditulis: 16 Maret 2019

Lihat langsung: https://kronix-k.github.io/belajar-html-01-home/

Catatan belajar HTML waktu masih pemula, mengikuti urutan W3Schools.

## Deskripsi

Bagian ini membahas tentang syntax HTML: apa itu syntax, bagian-bagiannya, aturan penulisannya, dan fungsi tiap syntax yang bisa dipakai. Syntax adalah aturan penulisan yang harus diikuti supaya browser mengerti kode yang kita tulis. Di HTML, syntax berupa tag yang ditulis di dalam tanda `< >`.

## Apa itu syntax

Syntax adalah aturan penulisan sebuah bahasa: urutan, tanda baca, dan bentuk yang harus diikuti supaya komputer bisa membaca kodenya.

HTML singkatan dari HyperText Markup Language. Markup language artinya bahasa penanda: tugasnya memberi tanda pada teks, misalnya "ini judul", "ini paragraf", atau "ini tautan". HTML bukan bahasa pemrograman karena tidak punya logika seperti perhitungan atau percabangan.

## Bagian-bagian syntax HTML

- Tag: nama di dalam `< >`. Tag pembuka `<p>`, tag penutup `</p>`.
- Elemen: tag pembuka, isi, dan tag penutup digabung. Contoh `<p>Halo</p>`.
- Isi: teks atau elemen lain di antara tag pembuka dan tag penutup.
- Atribut: pengaturan tambahan di tag pembuka, ditulis `nama="nilai"`. Contoh `<a href="https://contoh.com">`.
- Deklarasi: `<!DOCTYPE html>` adalah instruksi agar browser memakai standar HTML5.
- Komentar: `<!-- catatan -->`. Tidak tampil di halaman dan tidak boleh bersarang.
- Entitas karakter: kode untuk karakter khusus, yaitu `&lt;` untuk <, `&gt;` untuk >, `&amp;` untuk &, `&quot;` untuk tanda kutip, `&nbsp;` untuk spasi yang tidak terputus, dan `&copy;` untuk ©.

## Aturan syntax HTML

1. Tag diawali `<` dan diakhiri `>`.
2. Tag penutup memakai garis miring: `</p>`.
3. Nama tag dan nama atribut tidak membedakan huruf besar kecil, tetapi tulis dengan huruf kecil. Nilai atribut seperti nama file bisa membedakan huruf besar kecil.
4. Beri tanda kutip pada nilai atribut: `href="halaman.html"`.
5. Atribut hanya ditulis di tag pembuka, dipisah spasi: `<img src="foto.jpg" alt="Foto">`.
6. Satu atribut tidak boleh ditulis dua kali dalam satu tag.
7. Sebagian atribut boleh tanpa nilai, misalnya `<input disabled>`.
8. Elemen bersarang harus rapi dan tidak boleh bertumpang: `<b><i>teks</i></b>`.
9. Spasi dan enter di kode tidak berpengaruh: beberapa spasi atau baris baru ditampilkan sebagai satu spasi.
10. Karakter `<` dan `&` yang mau ditampilkan sebagai teks ditulis sebagai entitas.

## Syntax error di HTML

Di bahasa pemrograman, syntax yang salah biasanya membuat program berhenti dan menampilkan pesan error. HTML tidak begitu: browser mencoba memperbaikinya sendiri dan tetap menampilkan halaman. Akibatnya tidak ada pesan, tetapi hasilnya bisa berbeda dari maksud kita.

## Struktur dokumen minimal

```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Judul halaman</title>
</head>
<body>
  <h1>Judul</h1>
  <p>Paragraf.</p>
</body>
</html>
```

## Syntax yang bisa dipakai dan fungsinya

### Struktur halaman

- `<html>` : pembungkus seluruh halaman.
- `<head>` : informasi halaman, tidak tampil di layar.
- `<title>` : judul di tab browser.
- `<body>` : isi halaman yang terlihat.
- `<meta>` : informasi tambahan, misalnya set karakter. Tidak punya tag penutup.
- `<link>` : menghubungkan file luar, misalnya CSS. Tidak punya tag penutup.
- `<style>` : menulis CSS di dalam halaman.
- `<script>` : menulis atau memuat JavaScript.
- `<base>` : alamat dasar untuk semua tautan. Tidak punya tag penutup.

### Judul dan teks

- `<h1>` sampai `<h6>` : judul; h1 paling besar sampai h6 paling kecil.
- `<p>` : paragraf.
- `<br>` : pindah baris. Tidak punya tag penutup.
- `<hr>` : garis pemisah. Tidak punya tag penutup.
- `<pre>` : teks apa adanya, spasi dan enter dipertahankan.
- `<blockquote>` : kutipan panjang.
- `<q>` : kutipan pendek.
- `<address>` : informasi kontak.

### Format teks

- `<b>` : teks tebal.
- `<strong>` : teks penting, tampil tebal.
- `<i>` : teks miring.
- `<em>` : teks ditekankan, tampil miring.
- `<u>` : teks bergaris bawah.
- `<s>` : teks dicoret.
- `<small>` : teks lebih kecil.
- `<mark>` : teks disorot seperti stabilo.
- `<sub>` : teks turun (subscript).
- `<sup>` : teks naik (superscript).
- `<del>` : teks yang dihapus.
- `<ins>` : teks yang ditambahkan.
- `<code>` : potongan kode.
- `<kbd>` : tombol keyboard.
- `<abbr>` : singkatan.
- `<cite>` : judul sebuah karya.

### Tautan dan media

- `<a>` : tautan ke halaman lain.
- `<img>` : gambar. Tidak punya tag penutup.
- `<audio>` : pemutar suara.
- `<video>` : pemutar video.
- `<source>` : sumber file untuk audio atau video. Tidak punya tag penutup.
- `<iframe>` : halaman di dalam halaman.
- `<canvas>` : area gambar untuk JavaScript.
- `<svg>` : gambar vektor.

### Daftar

- `<ul>` : daftar berpoin.
- `<ol>` : daftar bernomor.
- `<li>` : satu butir dalam daftar.
- `<dl>` : daftar istilah.
- `<dt>` : istilah.
- `<dd>` : penjelasan istilah.

### Tabel

- `<table>` : tabel.
- `<caption>` : judul tabel.
- `<thead>` : bagian kepala tabel.
- `<tbody>` : bagian isi tabel.
- `<tfoot>` : bagian kaki tabel.
- `<tr>` : satu baris tabel.
- `<th>` : sel judul kolom.
- `<td>` : sel isi.

### Formulir

- `<form>` : formulir.
- `<input>` : kolom isian. Tidak punya tag penutup.
- `<label>` : label untuk isian.
- `<textarea>` : isian banyak baris.
- `<select>` : menu pilihan.
- `<option>` : satu pilihan di menu.
- `<button>` : tombol.
- `<fieldset>` : kelompok isian.
- `<legend>` : judul kelompok isian.

### Pengelompok dan semantik

- `<div>` : kotak pengelompok.
- `<span>` : pembungkus sebagian teks.
- `<header>` : kepala halaman atau bagian.
- `<nav>` : menu navigasi.
- `<main>` : isi utama halaman.
- `<section>` : satu bagian isi.
- `<article>` : tulisan yang berdiri sendiri.
- `<aside>` : isi sampingan.
- `<footer>` : kaki halaman atau bagian.
- `<figure>` : gambar beserta keterangannya.
- `<figcaption>` : keterangan gambar.

### Atribut yang sering dipakai

- `href` : alamat tujuan tautan, dipakai di a.
- `src` : alamat file gambar, audio, atau video.
- `alt` : teks pengganti kalau gambar gagal tampil.
- `id` : nama unik untuk satu elemen.
- `class` : nama kelompok yang bisa dipakai banyak elemen.
- `style` : mengatur tampilan langsung di elemen.
- `title` : teks bantuan saat kursor diarahkan.
- `lang` : bahasa isi halaman atau elemen.
- `width` : lebar elemen, misalnya gambar.
- `height` : tinggi elemen.
- `target` : tempat membuka tautan, misalnya _blank untuk tab baru.
- `type` : jenis isian pada input atau jenis tombol.
- `name` : nama isian pada formulir.
- `value` : nilai awal atau nilai kiriman.
- `placeholder` : teks petunjuk di dalam kolom isian.
- `disabled` : menonaktifkan elemen.
- `required` : isian wajib diisi.
- `charset` : set karakter, dipakai di meta.

## Kenapa tag harus ditutup

- Tanpa tag penutup, browser harus menebak di mana elemen berhenti.
- `</p>` boleh dihilangkan dalam kondisi tertentu, tetapi lebih aman selalu ditulis.
- `</h6>` wajib ditulis. Kalau lupa, elemen sesudahnya ikut masuk ke dalam h6.
- Elemen kosong seperti `<br>`, `<hr>`, dan `<img>` tidak perlu ditutup.
- Browser tidak menampilkan error, jadi kesalahan baru ketahuan setelah tampilan rusak.
- Cara mengecek: validator W3C di https://validator.w3.org/

## Fitur halaman

- Arahkan kursor ke bagian kode untuk melihat artinya.
- Edit kode langsung, hasilnya tampil di Website.
- Daftar "Perubahan yang dibuat" menjelaskan pengaruh tiap perubahan.
- Tag yang lupa ditutup ditandai dengan peringatan.

## Cara membuka di komputer

Download file index.html lalu buka di browser.

## Sumber

Mengikuti urutan W3Schools HTML Tutorial.
https://www.w3schools.com/html/
