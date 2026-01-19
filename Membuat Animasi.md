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
        var plane = new Image();
        plane.src = "https://raw.githubusercontent.com/FebrianyRenata02/San-Digital-Academy/refs/heads/main/img/Agency%20Logo%20Transparant.png";

        var i = 0,
            i_obs = 0,
            left = 0,
            right = 1;

        plane.onload = function() {
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

            // 🔥 PLANE (DIPERKECIL)
            ctx.drawImage(
                plane,
                70,
                240,
                plane.width / 8,
                plane.height / 8
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
