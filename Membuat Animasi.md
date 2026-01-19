# Membuat Animasi

Animasi yang akan di buat menggunakan gambar berikut yang akan di gerakan, untuk menggerakan gambar.
berikut method yang penting.

- setInterval (nama-method, waktu) - memanggil suatu method setiap beberapa milisecond
- save() - untuk menyimpan kondisi defauld
- restore() - untuk restrore kondisi
- translate(x, y) unruk menggeser sebuah object pada canvas bertambah akan bergeser secara vertikal

Berikut contoh kode untuk membuat animasi canvas, simpan kode ke dalam file animasi.html

```
<!DOCTYPE html>
<html>

<head>
    <title>Animation</title>
</head>

<body>
    <canvas id="canvas" width="300" height="300"></canvas>

    <script>
        var logo = new Image();
        logo.src = "https://raw.githubusercontent.com/FebrianyRenata02/San-Digital-Academy/refs/heads/main/img/Agency%20Logo%20Transparant.png";

        var i = 0,
            i_obs = 0,
            left = 0,
            right = 1;

        logo.onload = function() {
            setInterval(showAnimation, 30);
        };

        function showAnimation() {

            var canvas = document.getElementById('canvas');
            var ctx = canvas.getContext('2d');

            ctx.clearRect(0, 0, 300, 300);

            // BACKGROUND
            ctx.fillStyle = 'black';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            ctx.save();

            // MOVE RIGHT
            if ((i < 70) && (right == 1)) {
                i++;
            } else {
                right = 0;
                left = 1;
            }

            // MOVE LEFT
            if ((i > 0) && (left == 1)) {
                i--;
            } else {
                left = 0;
                right = 1;
            }

            ctx.translate(i, 0);

            // 🔥 LOGO (DIPERKECIL)
            ctx.drawImage(
                logo,
                70,
                240,
                logo.width / 8,
                logo.height / 8
            );

            ctx.restore();

            // OBSTACLES
            i_obs++;
            ctx.save();
            ctx.fillStyle = 'white';
            ctx.translate(0, i_obs);

            ctx.fillRect(100, -70, 30, 8);
            ctx.fillRect(150, 0, 30, 8);
            ctx.fillRect(100, 70, 30, 8);
            ctx.fillRect(150, 140, 30, 8);
            ctx.fillRect(100, 210, 30, 8);

            if (i_obs >= 423) {
                i_obs = 0;
            }

            ctx.restore();
        }
    </script>
</body>

</html>
```

## Output

![image](https://raw.githubusercontent.com/SansDev-Comunity/Pengenalan-HTML/refs/heads/main/img/canvas%20animation.png)

Penjelasan:
1. Load image

```
        var logo = new Image();
        logo.src = "https://raw.githubusercontent.com/FebrianyRenata02/San-Digital-Academy/refs/heads/main/img/Agency%20Logo%20Transparant.png";
```

2. Tentukan variable untuk pergerakan. Var i untuk pergerakan plane dan i_obs untuk pergerakan obstacle. Var left dan right di gunakan untuk menentukan apakah plane bergerak ke kiri atau ke kanan

```
  var i = 0,
            i_obs = 0,
            left = 0,
            right = 1;

        logo.onload = function() {
            setInterval(showAnimation, 30);
        };
```

3. Tentukan waktu untuk memanggil method yang menampilkan animasi, waktu yang di tentukan adalah 30 milisecond

```
  setInterval(showAnimation, 30);
```

4. Menyiapkan canvas dan penyimpanan state awal yaitu sebagai pergerakan.

```
    var canvas = document.getElementById('canvas');
            var ctx = canvas.getContext('2d');

            ctx.clearRect(0, 0, 300, 300);

            ctx.fillStyle = 'black';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            ctx.save();
```

5. Tentukan pergerakan logo.. logo akan bergerak secara horizontal yang di tentukan oleh variable i. variable i akan bertambah saat bergerak ke kanan dan akan berhenti pada saat i = 70. Saat i = 70 logo bergerak ke kiri sampai i = 0

```
 // MOVE RIGHT
            if ((i < 70) && (right == 1)) {
                i++;
            } else {
                right = 0;
                left = 1;
            }

            // MOVE LEFT
            if ((i > 0) && (left == 1)) {
                i--;
            } else {
                left = 0;
                right = 1;
            }

            ctx.translate(i, 0);

            // 🔥 LOGO (DIPERKECIL)
            ctx.drawImage(
                logo,
                70,
                240,
                logo.width / 8,
                logo.height / 8
            );

            ctx.restore();
```
