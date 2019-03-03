---
published: true
---
## Membuat Tampilan Hover, visited, active pada CSS

Pada link dihtml kita bisa menata tampilan link tersebut dengan propertis CSS misalkan warna background(background-color) , gaya tulisan(font-family), atau warna tulisan (color) dll. Untuk menata tampilan link anda bisa lakukan dengan menyesuaikan selector yang ada pada HTML. Apa itu selector ? bisa anda lihat pengertian selector dibagian menu home penjelasan CSS blog ini.

Oke sekarang kita akan masuk kepengenalan link state pada CSS :

    a:link /* ini untuk link normal */
    a:visited /* ini apabila link sudah dikunjungi */
    a:hover /* ini apabila cursor berada pada objek/teks link */
    a:active /* ini apabila link sudah diklik */


Bikin file stylelink.html lalu copas code dibawah ini :

```html
<html>
<head>
  <title>Link style</title>
  <style>
  a:link {
    color:black;
  }
 
  a:visited {
    color:red;
  }
 
  a:hover {
    color:blue;
  }
 
  a:active {
    color:green;
  }
  </style>
</head>
<body>
  <a href="#">Link</a>
</body>
</html>
```

Dan untuk menghilangkan garis pada link anda bisa gunakan text-decoration: none;  
Kalau sudah save, dan coba jalankan dibrowser anda. Selamat mencoba. ^_^
