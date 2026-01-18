# HTML 5 Canvas

Canvas adalah komponen utama yang membedakan HTML 5 dengan HTML versi sebelum nya

### Membuat Segi Empat

Contoh:
Buka Notepad++ simpan ke dalam file canvasSegiEmpat.html

```
<HTML>
	<HEAD>
		<TITLE> Belajar Canvas </TITLE>
	</HEAD>
	<BODY>
		<canvas id="myCanvas" width="200" height="100"
			style="border:1px solid #000000;">
		</canvas>
		<script>
			var c=document.getElementById("myCanvas");
			var ctx=c.getContext("2d");
			ctx.fillStyle="#FF0000";
			ctx.fillRect(0,0,150,75);
		</script>
	</BODY>
</HTML>

```

![image](https://raw.githubusercontent.com/SansDev-Comunity/Pengenalan-HTML/refs/heads/main/img/canvas%20segi%20empat.png)

Penjelasan
1. mencari elemen canvas pada kode:

```
var c=document.getElementByID ("myCanvas");
```

2. Memanggil method getContext() dengan parameter "2d) sehingga nantinya bisa menggunakan banyak properti dan method untuk menggambar kotak, garis, lingkaran, dsb

```
var ctx=c.getContext("2d");
```

3 Selanjutnya adalah perintah menggambar segi enmpat, Kode di bawah ini memilih warna pengambaran #FF0000 (merah).
setelah itu memnggambar segi empat (FillReact) mulai dari koordinat (0,0) dengan lebar 150 px dan tinggi 75px. Perlu di perhatikan bahwa koordinat (0,0) HTML 5 di mulai dari pojok kiri atas.

```
ctx.fillStyle="#FF0000";
ctx.fillRect(0,0,150,75);
```
