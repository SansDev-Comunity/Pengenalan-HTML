# Form

Form adalah daftar isian. dalam isian ini untuk meminta informasi dari user untuk di olah.
form dilakukan pada server sengan menggunakan skrip yang bersifat server-side.

Untuk membuat form, tag yang di perlukan adalah:

| Tag | FORM
| :--- | :--- | 
| Tag | TEXAREA
| Tag | SELECT
| Tag | INPUT 
| Tag | FORM

# Tag Form

Tag FORM merupakan tag yang di gunakan untuk mendefinisikan sebuah form.
tag ini mempunyai dua METHOD yaitu:

| ATRIBUT | KETERANGAN
| :--- | :--- | 
| METHOD | Untuk menentukan metode pengolahan form. pilihan
|        | method adalah GET atau POST
| ACTION | Untuk menentukan URL atau lokasi dari file yang di gunakan untuk mengolah form tersebut

# Tag Texarea

Tag TEXAREA di gunakan untuk membuat sebuah kotak teks multibaris.

| ATRIBUT | KETERANGAN
| :--- | :--- | 
| NAME | Mendefinisikan nama texarea
| ROWS | Menentukan berapa jumlah baris area
| COLS | Menentukan lebar dari texarea

Contoh
Bukalah Notepad++, kemudian tulis kode berikut:

```
<HTML>
<HEAD>
	<TITLE>Text Area</TITLE>
</HEAD>
	<BODY>
		<FORM>
		<TEXTAREA NAME=textarea1 ROWS=4 COLS=80>
Setiap kejadian selalu ada hikmahnya. Jangan bertanya kenapa ini terjadi, tapi tanyakanlah dengan ini apa yang bisa kita lakukan
		</TEXTAREA>
	</FORM>
	</BODY>
</HTML>
```
