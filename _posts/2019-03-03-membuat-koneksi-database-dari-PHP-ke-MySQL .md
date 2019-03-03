---
layout:     post
title:      Membuat Koneksi database dari PHP ke MySQL 
categories: php
tags:
 - php
 - mysql
published: true
---
## Membuat Koneksi database dari PHP ke MySQL 

Bagaimana cara mengkoneksikan php dengan database mysql ? pertanyaan itu sering saya dengar dari teman-teman. oke kita langsung saja.
1. buka notepadd++ atau teks editor kalian masing-masing dan buat file dengan ekstensi .php .
2. ketikan perintah seperti dibawah ini
```html
$host = 'localhost';
$user = 'root';
$pass = '';
$db = 'namadatabase';
$koneksi = mysqli_connect($host,$user,$pass,$db) or die(mysqli_error());
```
> 
keterangan : 1.$host = alamat komputer dimana SQL server berjalan.  
2.$user = nama username MySQL dimana kita akan login. Tergantung pada user SQL yang terdaftar. Secara default usernamenya root.  
3.$pass = password yang terdaftar atau yang dibuat untuk username MySQL. Secara default kosong arting '' .
4.$db = nama database diMysql kalian.  
5.or die(mysqli_error()) = ketika mysqli_connect($host,$user,$pass,$db) salah maka akan menjalankan die(mysqli_error()) yang artinya akan menampilkan error pada mysqli_connect tersebut apabila salah.

urutan dari value disesuaikan dengan urutan field database kalian. -> ketikan url localhost/namafolder/namafile.php dibrowser kalian masing-masing { catatan: sesuaikan dengan lokasi file php kalian }
-> jangan lupa jalankan phpmyadmin menjadi running.  
selesai.

Kalau ada yang salah tolong komentar nya ya.. Selamat mencoba. ^_^
