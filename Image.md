# Image

Tampilan halaman web akan lebih menarik jika di tambah media gambar seperti GIF, JPEG, PCX, PNG, WMF, dll.
psling cocok untuk menambahkan di gunakan tag 
```
img
```
| Atribut | Keterangan
| :--- | :--- | 
| SRC | Menunjukan url atau direktori tempat file gambar berada
| WIDTH | lebar gambar (dalam pixel)
| HEIGHT | Tinggi gambar (dalam pixel)
| ALIGN | posisis teks di sekitar gambar. Alternatif misalnya
|       | Adalah TOP, MIDDLE, BoTTOM, LEFT, RIGHT.
|       | Atribut ini tidak dikenali di HTML5 dan mulai
|       | di tinggalkan di HTML4.01
| ALT | menampilkan teks pengganti gambar jika gambar tidak dapat di tampilkan

Contoh:
Bukalah Notepad++, kemudian tulis kode berikut

```
<HTML>

<HEAD>
    <TITLE> Menambah Gambar </TITLE>
</HEAD>

<BODY>
    <IMG SRC="https://raw.githubusercontent.com/FebrianyRenata02/San-Digital-Academy/refs/heads/main/img/Agency%20Logo.png" ALT="San Digital Agency" ALIGN=Middle width="300px"> Gambar ini terdapat pada CD. Anda boleh menggantinya.
</BODY>

</HTML>
```

## Output

![image]()
