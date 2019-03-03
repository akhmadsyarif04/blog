---
layout:     post
title:      Memasukan Data keDatabase SQL Menggunakan PHP  
categories: php
tags:
 - php
 - mysql
published: true
---
## Memasukan Data keDatabase SQL Menggunakan PHP 

Saya anggap anda telah bisa membuat koneksi kedatabase SQL. Jadi kita akan langsung kequery INSERT pada SQL yang mana fungsi nya untuk menambahkan data dari inputan PHP ke database SQL. Oke tanpa basa basi langsung saja kecara pertama.

```html
$query = "INSERT INTO namatable (field1,field2,field3) VALUE ('ayam','naga','singa')"
```

> keterangan : 1.$query = nama vaiabel untuk query sql insert.  
2.namatable = isikan sesuai nama table didatabase kalian sesuai yang ingin kalian masukan data.  
3.field1,field2,field3 = nama field didalam table yang ingin kalian masukan data.  
4.'ayam','naga','singa' = nilai yang ingin kalian masukan.  

urutan dari value disesuaikan dengan urutan field database kalian.  
selanjutanya kita beri perintah untuk menjalankan query tersebut
```html
mysqli_query($link,$query);
```
> keterangan :  
1.$query = nama vaiabel query insert tadi.  
2.$link = nama variabel koneksi kedatabase.  

nah sekarang data telah ditambahkan kedalam database.  
kalian bisa menyesuaikan dengan program kalian masing-masing. misal dari nilai yang dimasukan, didapat dari
form website. maka perlu ditampung terlebih dulu nilai tersebut kevariabel atau pada query sql VALUE ( ) kalian isi dengan :

```html
$query = "INSERT INTO namatable (field1,field2,field3) VALUE ($_POST['nama_input'],$_POST['nama_input'],$_POST['nama_input'])"
```

Kalau ada yang salah tolong komentar nya ya.. Selamat mencoba. dan semoga bermanfaat. ^_^
