---
published: false
---
## One Time Pad

Teknik one-time pad adalah teknik enkripsi yang sempuna (perfect encryption) asalkan proses pembuatan kunci bener-bener acak.

Proses enkripsi one-time pad
![1.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/1.png)

Dengan one-time pad, operasi exclusive or (xor) dilakukan pada naskah asli, sedangkan pada kunci dengan cara Bitwise (Bitwise adalah operator xor digunakan sebagai operasi dasar yang paling banyak digunakan dalam enkripsi berbasis byte.) seperti pada gambar diatas. Operasi xor akan menghasilkan 0 jika argumen sama. Misalnya 0 dengan 0 maka hasil nya adalah 0, dan 1 dengan 1 maka hasilnya 0. Dan menghasilkan 1 jika argumen nya berbeda. Misalnya 0 dengan 1 maka hasilnya 1, 1 dengan 0 hasilnya 1.

Proses dekripsi one-time pad    
![2.png]({https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/2.png)

Proses dekripsi sama dengan proses enkripsi, akan tetapi xor dilakukan pada naskah acak dan kunci dekripsi. Catatan, kunci enkripsi dan dekripsi itu sama.  
Operasi exclusive or sangat berperan dalam kriptografi: semua algoritma enkripsi simetris modern menggunakan operasi exclusice or. Simbol⊕sering kali digunakan dalam petanda exclusive or.  
Key management (pengelola kunci) menjadi sangat penting dan merupakan kelemahan one-time pad yang membuatnya tidak layak untuk menggunakan dengan skala besar. Besar kunci harus sama dengan besar naskah asli, dan kunci tidak boleh digunakan berkali-kali. Selain masalah key generation ( Key generation merupakan kegiatam manajemen kunci dalam menghasilkan kunci yang acak dimana keacakan kunci merupakan bagian terpenting dalam menjamin kekuatan suatu kriptografi ) ,  masalah key distribution menjadi kendala penggunaan skala besar pada enkripsi one-time pad.  
One-time pad dapat digunakan dalam berkomunikasi sangat rahasia asal dengan volume yang kecil atau tidak terlalu besar. Jika pada penggunaan skala besar suatu sistem teknologi informasi, one-time pad tidak praktis untuk digunakan. Walaupun begitu konsep one-time pad ini ditiru dalam teknik enkripsi stream cipher.
