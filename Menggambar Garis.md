# Menggambar Garis

penggambaran garis di lakukan menggunakan dua fungsi dasar yaitu MoveTo() dan LineTo()
kita bisa membuat garis dari titik (0,0) ke (200,100). Kemudian simpan kodenya dalam file canvasGaris.html

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
			ctx.moveTo(0,0);
			ctx.lineTo(200,100);
			ctx.stroke();
		</script>
	</BODY>
</HTML>
```

## Output
![image](https://raw.githubusercontent.com/SansDev-Comunity/Pengenalan-HTML/refs/heads/main/img/Canvas%20Garis.png)

Penjelasan

1. Kursor di posisikan dulu pada titik (0,0) dengan kode berikut
   
```
ctx.moveTo(0,0);
```

2. Setelah itu panggil method untuk menarik garis dari posisi kursor sekarang (0,0) ke tujuan (200,100). namun sampai tahap ini
garis belum tergambaar

```
ctx.lineTo(200,100);
```

3. Setelah itu panggil method Stroke() yang berfungsi untuk betul-betul menggambar garis yang sudah dispesifikkan di atas

```
ctx.stroke();
```
