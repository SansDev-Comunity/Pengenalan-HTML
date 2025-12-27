# Memasukkan Gambar di Halaman Web

Gambar merupakan elemen penting yang membuat halaman web Anda terlihat lebih menarik. Untuk menambahkan gambar di HTML, Anda hanya perlu menggunakan tag 

```
img
```
Namun, perlu diingat bahwa Anda tidak bisa langsung memasukkan file gambar ke HTML. Anda perlu menyimpannya dulu di suatu lokasi, lalu merujuknya menggunakan atribut seperti src dan alt agar gambar bisa ditampilkan dengan benar.

```
<img src="gambar-pemandangan.jpg" alt="Pemandangan Indah di Pegunungan" width="300" height="200">
```

Pada contoh di atas, src menunjukkan lokasi file atau URL gambar. Anda bisa memasukkan link gambar dari internet atau alamat dari folder lokal di perangkat Anda.


Web Development
Feb 20, 2025

Faradilla A.

13menit Dibaca

23 Contoh Kode HTML yang Cocok Dipelajari oleh Pemula
Dapatkan ringkasan:
ChatGPT
Claude.ai
Google AI
Grok
Perplexity
Share:
HyperText Markup Language, atau yang lebih populer disebut HTML, adalah bahasa markup yang digunakan untuk menyusun struktur halaman web. Anda bisa mengatur teks, menambahkan gambar dan link, hingga membuat formulir.

Meskipun membutuhkan coding, HTML sebenarnya mudah dipelajari karena bukan merupakan bahasa pemrograman. Tag-tag HTML juga cukup jelas, karena memiliki struktur yang sederhana dan teratur.

Kalau Anda tertarik untuk belajar HTML, kami akan memandu Anda melalui artikel ini. Kami punya banyak contoh HTML untuk berbagai tujuan, mulai dari fungsi dasar hingga pembuatan halaman web. Sudah siap? Mari mulai!

Contoh Kode HTML untuk Pemula
1. Struktur Dasar HTML
2. Heading dan Paragraf
3. Memformat Teks dengan Bold, Italic, Underline
4. Memasukkan Gambar di Halaman Web
5. Menambahkan Link dalam Teks
6. Mencantumkan Daftar dengan Bullet Poin
7. Mebuat Daftar Berurutan
8. Membuat Tabel dengan Baris dan Kolom
9. Membuat Formulir Sederhana
10. Menambahkan Daftar Dropdown
11. Membuat Kotak Centang
12. Menambahkan Radio Button
13. Memasukkan Video dan Audio
14. Mengubah Warna Teks
15. Mengganti Font Teks
16. Menyorot Teks dengan Warna
17. Mengubah Ukuran Teks
18. Mengatur Perataan Teks
19. Mencoret Sebagian Teks
20. Membuat Kutipan
21. Menambahkan Tooltip
22. Menambahkan Kolom Tanggal
23. Menampilkan Teks Superscript dan Subscript
Tips Membuat Hasil Kode HTML Lebih Menarik
1. Tambahkan CSS untuk Memberikan Style
2. Berikan Animasi Interaktif dengan JavaScript
3. Gunakan Font Kustom
4. Tambahkan Hover dan Transisi
Contoh Kode HTML untuk Pemula
Untuk mempelajari HTML, Anda tidak perlu menguasai algoritma pemrograman atau logika seperti variabel dan syntax yang rumit. Hasil kode HTML juga akan langsung terlihat sehingga Anda bisa menyesuaikannya dengan lebih mudah.

Di tutorial ini, kami akan memberikan contoh coding HTML untuk membantu Anda mempelajarinya. Tenang, kami akan menunjukkan hasilnya sehingga Anda bisa mendapatkan gambaran yang lebih jelas.

Langsung saja, ini contoh kode HTML yang bisa Anda coba, dimulai dari yang paling mudah.

1. Struktur Dasar HTML
Dalam HTML, ada struktur dasar yang harus Anda gunakan agar halaman web yang dibuat bisa berfungsi. Struktur ini akan menjadi kerangka halaman sehingga web browser bisa menampilkannya dengan benar.

Beberapa tag utama yang menjadi struktur dasar HTML adalah <html>, <head>, dan <body>. Semua tag ini harus berpasangan untuk membuka dan menutup setiap bagiannya, yang ditandai dengan garis miring. Misalnya, tag <head> harus ditutup dengan tag </head>.

Berikut contoh penggunaannya:

<!DOCTYPE html>
<html>
  <head>
    <title>Contoh Struktur Dasar HTML</title>
  </head>
  <body>
    <p>Halo, dunia!</p>
  </body>
</html>
Pada contoh ini, kode dimulai dengan <!DOCTYPE html>. Tag ini memberi tahu web browser bahwa dokumen yang dimuat adalah HTML5.

Kemudian, tag <html> mencakup semua elemen yang ada di halaman. Setelah itu ada bagian <head> yang memuat informasi tambahan, seperti <title> untuk judul yang nantinya akan muncul di tab browser.

Nah, bagian <body> adalah tempat Anda memasukkan semua konten utama website, seperti teks, gambar, dan elemen lainnya. Perlu diingat bahwa hampir semua contoh kode berikutnya dalam tutorial ini perlu disertakan dalam tag <body> dan </body> agar bisa berfungsi.

Dari contoh pertama ini, berikut hasil coding HTML kami ketika dibuka di browser:

tampilan contoh html halo dunia di chrome
2. Heading dan Paragraf
Berikutnya, ada heading dan paragraf yang membentuk struktur teks di halaman web. Dengan dua elemen ini, Anda bisa membuat teks dengan format judul, subjudul, dan isi paragrafnya.

Heading dalam HTML memiliki 6 tingkat yang dimulai dari tag <h1> untuk judul utama, sampai <h6> untuk subjudul terkecil. Sementara itu, tag untuk paragraf adalaj <p>. Jangan lupa untuk menyertakan tag penutupnya juga.

Contoh penggunaan tag heading dan paragraf adalah sebagai berikut:

<h1>Judul Utama (H1) di Bagian Ini</h1>
<h2>Sub Judul (H2) Ada di Sini </h2>
<p>Bagian ini berisi teks paragraf yang bisa Anda isi dengan konten tulisan.</p>
Perlu diperhatikan bahwa tag <h1> biasanya hanya digunakan sekali sebagai judul utama. Heading lainnya boleh digunakan sesuai kebutuhan untuk subjudul. Anda akan melihat hasil seperti ini saat mencoba kode di atas:

tampilan hasil dari contoh coding html untuk heading dan paragraf
3. Memformat Teks dengan Bold, Italic, Underline
HTML memiliki tag <strong> untuk teks tebal atau bold, <em> untuk teks miring atau italic, serta <u> untuk garis bawah. Sebenarnya ada juga tag <b> untuk menebalkan teks dalam HTML, tapi tag ini hanya mengubah tampilan teks tanpa ada makna khusus.

Tag <strong> memiliki fungsi semantik yang menekankan bahwa teks dalam tag tersebut bersifat penting dan perlu ditekankan. Tag ini digunakan oleh crawler mesin pencari untuk SEO, dan oleh aplikasi pembaca layar untuk memberikan penekanan khusus.

Ini contohnya:

<p>Baris ini memiliki <strong>kata-kata yang diformat tebal dengan tag strong</strong>.</p>
<p>Sementara itu, kata-kata di baris ini <em>diformat dengan tag em</em> agar miring.</p>
<p>Di baris ini, <u>ada teks yang diformat underline</u> untuk menambahkan garis bawah.</p>
Berikut hasil percobaan kami:

tampilan contoh teks bold, italic, dan underline
4. Memasukkan Gambar di Halaman Web
Gambar merupakan elemen penting yang membuat halaman web Anda terlihat lebih menarik. Untuk menambahkan gambar di HTML, Anda hanya perlu menggunakan tag <img>.

Namun, perlu diingat bahwa Anda tidak bisa langsung memasukkan file gambar ke HTML. Anda perlu menyimpannya dulu di suatu lokasi, lalu merujuknya menggunakan atribut seperti src dan alt agar gambar bisa ditampilkan dengan benar.

Coba perhatikan contoh berikut:

<img src="gambar-pemandangan.jpg" alt="Pemandangan Indah di Pegunungan" width="300" height="200">
Pada contoh di atas, src menunjukkan lokasi file atau URL gambar. Anda bisa memasukkan link gambar dari internet atau alamat dari folder lokal di perangkat Anda.

Sementara itu, tag alt digunakan untuk menuliskan deskripsi gambar. Teks ini akan muncul kalau gambar gagal dimuat di web browser, serta membantu menjelaskan isi gambar kepada pengunjung yang memiliki gangguan penglihatan.

Di bagian akhir, kami menambahkan tag ukuran width dan height untuk mengatur lebar dan tinggi gambar sesuai kebutuhan. Hasilnya adalah
