# Tag Frame

Tag Frame mempunyai atribut

| ATRIBUT | KETERANGAN 
| :--- | :--- | 
| SRC | Membuat menentukan nama file HTML yang di gunakan sebagai frame
| MARGINHEIGHT | membuat penekanan pada teks 
| SCROLLING | membuat teks bercetak miring 
| NORESIZE | membuat teks bercetak kecil
| NAME | menyatakan bahwa teks tersebut penting
| BORDER | Membuat teks tercetak sebagai subscript

Contoh:
1. buka Notepad++, kemudian tulis kode berikut

```
    <html>
      <head>
          <title>Frame Kanan</title>
      </head>
   
      <body bgcolor = "white">
      <h1>Frame di sebelah Kanan</h1>
      </body>
   </html>
```
Simpan dengan nama: framekanan.html
Output:
![image](https://raw.githubusercontent.com/SansDev-Comunity/HTML/refs/heads/main/img/frame%20kanan.png)

   ```
    <html>
      <head>
          <title>Frame Kiri</title>
      </head>
   
      <body bgcolor = "white">
      <h1>Frame di sebelah Kiri</h1>
      </body>
   </html>
   ```

Simpan dengan nama: framekiri.html
Output:
![image](https://raw.githubusercontent.com/SansDev-Comunity/HTML/refs/heads/main/img/frame%20kiri.png)

   ```
    <html>
      <head>
          <title>Contoh Penggunaan Frame</title>
      </head>
   
      <frameset cols = "30%">
         <frame src="framekiri.html>
         <frame src="framekanan.html>
      </frameset>
   </html>
   ```
