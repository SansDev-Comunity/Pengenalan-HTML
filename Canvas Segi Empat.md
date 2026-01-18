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
