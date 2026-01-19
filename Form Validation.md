# Form Validation

Form valodation adalah proses di mana browser dan web server akan memeriksa data yang di input dalam format yang di tetapkan.
validasi yang di lakukan di server di sebut server-side validation.

HTML 5 mempunyai beberapa fitur validasi tepat nya pada TAG

| Atribut | Keterangan
| :--- | :--- | 
| required | Menentukan apakah bidang formulir perlu di isi sebelum formulir dapat di kirim
| minlength | Menentukan panjang minimum dari data tekstual (string)
| min | Menentukan panjang maksimum dari tipe input numerik (angka)
| max | Menentukan nilai maksimum dari tipe input numerik (angka)
| type | Menentukan tipe data, contohnya bertipe angka dan alamat email
| pattern | Menentukan regular expression (regex) yang mendefinisikan pola yang harus di ikuti data yang dimasukan

Berikut contoh untuk validasi form, Simpan kode ke dalam validasiForm.html

```
<!DOCTYPE HTML>
	<HEAD>
		<TITLE>Form Validation</TITLE>		
	</HEAD>
	<BODY>
		<p>Isilah Form di Bawah Ini</p>
		<hr>
		<form>
			Nama *<br>
			<input id="nama" type="text" required><br>
			Alamat *<br>
			<textarea id="alamat" type="text" required rows="5" cols="30"></textarea><br>
			No Telepon *<br>
			<input id="telepon" type="text" minlength="8" pattern="\+62?(\d+)+|\(\d+\)"><br>	
			Alamat Email<br>
			<input id="email" type="email"><br>
			Umur<br>
			<input id="umur" type="number" min=1><br><br>

  			<button>Kirim</button>
		</form>	
	</BODY>
</HTML>
```

## Output

![image](https://raw.githubusercontent.com/SansDev-Comunity/Pengenalan-HTML/refs/heads/main/img/Validasi%20Form.png)
