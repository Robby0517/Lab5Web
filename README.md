# Lab5Web

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh `document.write` dan `console.log`</h3>
    <script>
        document.write("Hello World<br>");
        console.log("Hello World");
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pemasukan Data</title>
</head>
<body>
    <script language="javascript">
        var nama = prompt("Siapa nama Anda?", "Masukkan nama Anda");
        document.write("Hai, " + nama);
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Program JavaScript</title>
    <script language="javascript">
        function pesan() {
            alert("Memanggil JavaScript lewat body onload");
        }
    </script>
</head>
<body onload="pesan()">
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Program JavaScript</title>
    <script language="javascript">
        function test(val1, val2) {
            document.write("<br>Perkalian: " + (val1 * val2) + "<br>");
            document.write("Pembagian: " + (val1 / val2) + "<br>");
            document.write("Penjumlahan: " + (val1 + val2) + "<br>");
            document.write("Pengurangan: " + (val1 - val2) + "<br>");
            document.write("Modulus: " + (val1 % val2) + "<br>");
        }
    </script>
</head>
<body>
    <input type="button" value="Arithmetic" onclick="test(9, 4)">
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh If-Else</title>
</head>
<body>
    <script language="javascript">
        var nilai = prompt("Nilai (0-100):", 0);
        var hasil = "";
        if (nilai >= 60) {
            hasil = "Lulus";
        } else {
            hasil = "Tidak Lulus";
        }
        document.write("Hasil: " + hasil);
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Program JavaScript</title>
    <script language="javascript">
        function test() {
            var val1 = window.prompt("Input nilai (1-5):");
            switch (val1) {
                case "1":
                    document.write("Bilangan satu");
                    break;
                case "2":
                    document.write("Bilangan dua");
                    break;
                case "3":
                    document.write("Bilangan tiga");
                    break;
                case "4":
                    document.write("Bilangan empat");
                    break;
                case "5":
                    document.write("Bilangan lima");
                    break;
                default:
                    document.write("Bilangan lainnya");
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="Switch" onclick="test()">
</body>
</html>

<html>
<head>
    <script language="javascript">
        function test() {
            var val1 = document.kirim.T1.value;
            if (val1 % 2 == 0)
                document.kirim.T2.value = "bilangan genap";
            else
                document.kirim.T2.value = "bilangan ganjil";
        }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20"></p>
        <p>MERUPAKAN BIL <input type="text" name="T2" size="20" readonly></p>
        <p><input type="button" value="TEBAK" name="B1" onclick="test()"></p>
    </form>
</body>
</html>

<!DOCTYPE html>
<html>
<head>
    <title>objek document</title>
</head>
<body>

<script>
function ubahWarnaLB(warna) {
    document.bgColor = warna;
}

function ubahWarnaLD(warna) {
    document.fgColor = warna;
}
</script>

<h1>tes</h1>

<form>
    <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
    <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
    <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
    <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
</form>

<script>
document.write("Dimodifikasi terakhir pada " + document.lastModified);
</script>

</body>
</html>


<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language="javascript">
        <!--
        function ubahWarnaLB(warna) {
            document.bgColor = warna;
        }
        
        function ubahWarnaLD(warna) {
            document.fgColor = warna;
        }
        //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onClick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onClick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onClick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onClick="ubahWarnaLD('BLUE')">
    </form>

    <script language="javascript">
        <!--
        document.write("Dimodifikasi terakhir pada " + document.lastModified);
        //-->
    </script>
</body>
</html>


