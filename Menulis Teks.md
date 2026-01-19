# Menulis Teks

Untuk menulis pada canvas, berikut adalah method-method yang penting

- font mendefinisikan property font untuk teks yang akan di tulis
- fillText(text,x,y) - menggambar teks dengan fill pada canvas
- strokeText (text,x,y) - menggambar teks tanpa fill pada canvas

Berikut contoh pembuatan teks dengan mengganti bagian kode JavaScript, Contoh:
simpan fike canvasTeks.html

```
<HTML>

<HEAD>
    <TITLE> Canvas Teks </TITLE>
</HEAD>

<BODY>
    <canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;">
		</canvas>
    <script>
        var c = document.getElementById("myCanvas");
        var ctx = c.getContext("2d");
        ctx.font = "30px Arial";
        ctx.fillText("Hai Indonesia", 10, 50);
    </script>
</BODY>

</HTML>
```

## Output

![image](https://raw.githubusercontent.com/SansDev-Comunity/Pengenalan-HTML/refs/heads/main/img/Canvas%20Teks.png)
