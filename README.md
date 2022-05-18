# Lab7Web

                              Nama = Angga Thifal Ananda
                              NIM = 312010419
                              Kelas = TI 20 B2


# Praktikum 7

# A. Install Xampp
Jika sudah install, taruh file tersebut di direktori (d:\xampp)
![Screenshot (179)](https://user-images.githubusercontent.com/73052649/169023088-7b8d89d3-aec6-4263-b7f9-d316576a5c69.png)
Setelah itu, kita akan tes apakah server sudah bekerja dengan baik. ( http://127.0.0.1/ atau http://localhost/ ). Jika Server sudah berjalan dengan baik maka akan tampil halaman utama Xampp.
![Screenshot (180)](https://user-images.githubusercontent.com/73052649/169023126-3f2f1dfd-ebb8-4cd3-9c32-9a1cbf5782a8.png)

# B. Memulai PHP
Buat folder lab7_php_dasar pada root directory web server (d:\xampp\htdocs)
![Screenshot (179)](https://user-images.githubusercontent.com/73052649/169023356-603243b4-d549-40e7-b556-6e5e1e270499.png)
Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL: http://localhost/lab7_php_dasar/
![Screenshot (188)](https://user-images.githubusercontent.com/73052649/169023947-1c0f6414-3af1-4d7b-b95b-6c56beb18b71.png)

# C. PHP Dasar
Buatlah file baru dengan nama php_dasar.php, lalu masukan kode berikut.
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>PHP Dasar</title>
</head>

<body>
  <h1>Belajar PHP Dasar</h1>
  <?php
  echo "Hello World";
  ?><br>

  <!-- Variabel PHP -->
  <h1>Variabel PHP</h1>
  <?php
  $nim = "312010338";
  $nama = 'Alfiansyah Rambe';
  echo "NIM : " . $nim . "<br>";
  echo "Nama : $nama";
  ?>
</body>

</html>
```
Hasil outputnya akan seperti ini. dan untuk mengaksesnya gunakan link ini : http://localhost/lab7_php_dasar/php_dasar.php
![Screenshot (182)](https://user-images.githubusercontent.com/73052649/169024179-66065eca-e6c8-4776-994e-c9517b51f6a7.png)
# Predefine Variable $_GET
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PHP Dasar 2</title>
</head>

<body>
  <!-- Predefine variabel -->
  <h1>Predefine Variabel</h1>
  <?php
  echo 'Selamat Datang ' . @$_GET['nama'];
  ?>
</body>

</html>
```
Hasil outputnya dan akses nya : http://localhost/lab7_php_dasar/php_dasar2.php?nama=Angga 
![Screenshot (189)](https://user-images.githubusercontent.com/73052649/169024581-43b4e7ad-ac7e-45d8-a0a0-e60ed7fa8383.png)
# Membuat Form input
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Form input</title>
</head>

<body>
  <h2>Form Input</h2>
  <form method="post">
    <label>Nama: </label>
    <input type="text" name="nama">
    <input type="submit" value="Kirim">
  </form>
  <?php
  echo 'Selamat Datang ' . $_POST['nama'];
  ?>
</body>

</html
```
Maka outputnya akan seperti ini :
![Screenshot (187)](https://user-images.githubusercontent.com/73052649/169024722-68bcc446-aee6-49b9-b48d-ca01394ce876.png)
# Operator 
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Operator</title>
</head>

<body>
  <h1>Operator</h1>
  <?php
  $gaji = 1500000;
  $pajak = 0.1;
  $thp = $gaji - ($gaji * $pajak);
  echo "Gaji sebelum pajak = Rp. $gaji <br>";
  echo "Gaji yang dibawa pulang = Rp. $thp";
  ?>

</body>

</html>
```
![Screenshot (184)](https://user-images.githubusercontent.com/73052649/169024872-c37f2c6a-0e21-4b58-8fa0-64c7dddcd575.png)
# Kondisi IF
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>If</title>
</head>

<body>
  <h1>Kondisi If</h1>
  <?php
  $nama_hari = date("l");
  if ($nama_hari == "Sunday") {
    echo "Minggu";
  } elseif ($nama_hari == "Monday") {
    echo "Senin";
  } else {
    echo "Selasa";
  }
  ?>

</body>

</html>
```
![Screenshot (185)](https://user-images.githubusercontent.com/73052649/169024988-9d1c3235-ebb7-4259-98c8-b57ca8b00d45.png)
# Kondisi Switch
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Switch</title>
</head>

<body>
  <h1>Kondisi Switch</h1>
  <?php
  $nama_hari = date("l");
  switch ($nama_hari) {
    case "sunday";
      echo "Minggu";
      break;
    case "Monday";
      echo "Senin";
      break;
    case "Tuesday";
      echo "Selasa";
      break;
    default:
      echo "Sabtu";
  }
  ?>

</body>

</html>
```
![Screenshot (186)](https://user-images.githubusercontent.com/73052649/169025115-74176b1c-05fe-410a-b9c3-523d75ee305b.png)



