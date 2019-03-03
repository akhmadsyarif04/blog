---
published: true
---
## Apa itu CSS?

CSS adalah singkatan dari Cascading Style Sheets. Berisi rangkaian instruksi yang kita tentukan untuk mempercantik tampilan web. Perancangan desain text/tampilan web dapat dilakukan dengan mendefinisikan fonts (huruf) , colors (warna), margins (ukuran), latar belakang (background), ukuran font (font sizes) dan lain-lain. Elemen-elemen seperti colors (warna) , fonts (huruf), sizes (ukuran) dan spacing (jarak) disebut juga styles. Cascading Style Sheets juga bisa berarti meletakkan styles yang berbeda pada layers (lapisan) yang berbeda. CSS terdiri dari style sheet yang memberitahukan browser bagaimana suatu dokumen akan disajikan. Fitur-fitur baru pada halaman web lama dapat ditambahkan dengan bantuan style sheet. Saat menggunakan CSS, Anda tidak perlu menulis font, color atau size pada setiap paragraf, atau pada setiap dokumen. Setelah Anda membuat sebuah style sheet, Anda dapat menyimpan kode tersebut sekali saja dan dapat kembali menggunakannya bila diperlukan.
Contoh sintak CSS internal :
> <html>
  <head>
    <style>
      h1{
        color:red;
      }
    </style>
  </head>
  <body>
    <h1>Text H1</h1>
  </body>
<html>
  
Contoh sintak CSS inline : 
> <html>
<head>
  <title>CSS</title>
</head>
<body>
  <h1 style="color:blue">Text H1</h1>
</body>
</html>
  
Contoh sintak CSS external :

#Pertama bikin file nama_file.html tambahkan <link rel="stylesheet" type="text/css" href="nama_file.css"> kedalam html dan letakkan diatas </head> seperti dibawah ini : 
 > <html>
<head>
  <title>CSS</title>
  <link rel="stylesheet" type="text/css" href="nama_file.css">
</head>
<body>
  <h1>Text H1</h1>
</body>
</html>
  
nama_file.css pada href="nama_file.css"> sesuaikan dengan nama file css anda.
#Kedua bikin file nama_file.css dan copy kode dibawah ini : 
  
> h1{
  font-size:15px;
}

  
Selanjutnya kita akan mengenal nama-nama setiap bagian CSS :

> h1{
  font-size:15px;
}

    h1 -> Selector
    { } -> Deklarasi
    font-size -> Properti
    15px -> Nilai/Value


Sekian dan terimakasih, semoga bermanfaat. ^_^ 