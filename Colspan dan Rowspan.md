# Colspan dan Rowspan

Anda mungkin sudah familiar dengan istilah merge cell pada Microsoft Excel atau Microsoft Word.
dalam pemrograman web juga terdapat fasilitas untuk menggabungkan beberapa cell secara horizontal (ke samping) dan vertikal (ke bawah) jadi satu,
Colspan artinya menggabungkan beberapa kolom cell jadi satu sedangkan rowspan menggabungkan beberapa baris cell jadi satu.

Colspan atau column span merupakan atribute HTML yang berfungsi untuk
menggabungkan beberapa kolom, sederhananya menggabungkan kolom ke samping. 
Rowspan merupakan atribut HTML yang fungsi utamanya adalah menggabungkan 
beberapa baris, sederhananya menggabungkan baris ke bawah.

Buka Notepad++ tulis kode berikut

```
<html>
	<head>
		<title> Latihan Colspan dan Rowspan</title>
	</head>

	<body>
		<table border="8">
		<tr>
			<td colspan="2" align="center">Satu</td>
		</tr>
		<tr>
			<td align="center">Dua</td>
			<td align="center">Tiga</td>
		</tr>
		<tr>
			<td colspan="2" align="center">Empat</td>
		</tr>
		</table>
	</body>
</html>

```

Simpan dalam table_span.html

## Output

![image](https://raw.githubusercontent.com/SansDev-Comunity/HTML/refs/heads/main/img/table%20span.png)
