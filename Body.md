# Body

Element ini untuk menampilkan isi dokumen HTML
terletak di bawah tag <Head>

```
<body test="v" bgcolor = "w" background="url" link="x" alink="y">
..........
</body>
```

Keterangan:
● Bentuk dari tag HTML adalah <Element Atribute = Value>

○ Element - nama tag <br>
○ Atribute - atribute dari tag <br>
○ Value - nilai dari atribute <br>

● text memberikan warna pada teks <br>
● bgcolor: memberikan warna pada latar belakang dokumen HTML dan bentuk gambar <br>
● background: memberikan latar belakang dokumen HTML dalam bentuk gambar <br>
● link: memberikan warna untuk link <br>
● alink: memberikan warna untuk link yang sedang aktif <br>
● vlink: memberi warna untuk link yang telah di kunjungi <br>

Contoh <br>
1. Bukalah Notepad++, Kemudian tuliskan kode berikut

```
<HTML>
  <Body>
  Tuliskan ini akan tampak di dalam browser
  </Body>
</HTML>
```

Smpan di dalam body.html kemuadian buka body.html menggunakan browser

![image](https://raw.githubusercontent.com/SansDev-Comunity/HTML/refs/heads/main/img/body_html.png)

2. Buka Notepad++, tuliskan kode berikut

```
<HTML>
  <BODY BGCOLOR = "yelow' TEXT = "red">
    Tulisan ini akan tampak dalam browser.
  </BODY>
</HTML>
```

Simpan ke dalam background.html

![image](https://raw.githubusercontent.com/SansDev-Comunity/HTML/refs/heads/main/img/background.png)

3. Bukalah Notepad++, kemudian tulis kode berikut

```
<HTML>
  <BODY BGCOLOR = "#FFFF000' TEXT = "#FF0000">
    Tulisan ini akan tampak dalam browser.
  </BODY>
</HTML>
```

Simpan ke dalam warna.html kemudian buka warna.html menggunakan browser,
Ganti-ganti gambar warna nya dengan warna lain sesuai tabel berikut.

| black | #000000 | blue | #0000ff | olive | #8080000
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[01. Konvensi Kode](chapters/01-konvensi-dan-standar-kode.md)** | Standardisasi | Penamaan, Sintaks Modern, DRY. |
| **[02. Arsitektur](chapters/02-arsitektur-dan-logika-bisnis.md)** | Struktur | Service Layer, SRP, Skinny Controller. |
| **[03. Validasi & Keamanan](chapters/03-validasi-dan-keamanan.md)** | Integritas | Form Requests, Policies, Config Safety. |
| **[04. Manajemen Data](chapters/04-eloquent-dan-manajemen-data.md)** | Eloquent | Mass Assignment, Accessors, Transactions. |
| **[05. Optimasi Performa](chapters/05-optimasi-query-dan-performa.md)** | Skalabilitas | N+1 Problem, Queues, Database Indexing. |
| **[06. Presentasi](chapters/06-presentasi-dan-frontend.md)** | Output | API Resources, Blade Clean Code, Assets. |
| **[07. Pengujian](chapters/07-pengujian-dan-kualitas.md)** | Reliabilitas | Feature Testing, Model Factories, Pint. |
