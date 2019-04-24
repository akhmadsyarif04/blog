---
published: false
---
## Known Plaintext Attack

__Known plaintext attack__ adalah teknik pencarian kunci enkripsi berdasarkan pengetahuan mengenai pasangan asli – naskah acak. Kita akan menggunakan Ceaser chiper sebagai contoh dari enkripsi yang rentan terhadap __known plaintext attack__.

Julius caesar menukar setiap huruf dalam naskah asli dengan huruf lain dalam naskah acak. Besar atau kecil huruf dipertahankan dalam naskah acak (huruf besar ditukar dengan huruf besar, huruf kecil ditukar dengan huruf kecil), spasi, titik, koma dan tanda lainnya tidak ditukar.

Ceaser cipher adalah jenis enkripsi yang disebut simple substitution chiper dimana setiap huruf dalam naskah asli ditukar dengan huruf lain dalam naskah acak. 

Julius Caesear menukar huruf dengan cara shift transformation. Rumus umum untuk shift transformation adalah : 

![rumus-shift-transformation.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/rumus-shift-transformation.png)

dimana :
C adalah kode bilangan karakter acak,
P adalah kode bilangan karakter asli,
b adalah bersarnya shift,
n adalah besarnya perbendaharaan karakter (dengan kode 0 sampai n – 1).

jadi rumus untuk enkripsi sesuai dengan relasi ekuivalen:  
![rumus-shift-transformation-enkrip.png]({{site.baseurl}}/_posts/rumus-shift-transformation-enkrip.png)
Rumus untuk dekripsi juga sesuai dengan relasi ekuivalen :  
![rumus-shift-transformation-dekrip.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/rumus-shift-transformation-dekrip.png)  
Julius Caesar sendiri menggunakan huruf “A” sampai “Z”  (dengan code 0 sampai 25) sebagai perbendaharaan karakter untuk enkripsi (karakter selain huruf tidak dienkripsi), dan menggunakan parameter b = 3 menghasilkan rumus enkripsi.  
![contoh-rumus-julius-caesar-enkripsi.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/contoh-rumus-julius-caesar-enkripsi.png)  
Jadi untuk enkripsi, 0 (“A”) ditukar dengan 3 (“D”), 1 (“B”) dengan 4 (“E”), …. , 24 (“Y”) dengan 1 (“B”), dan 25 (“Z”) dengan 2 (“C”).  
Rumus dekripsi menjadi  
![contoh-rumus-julius-caesar-dekripsi.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/contoh-rumus-julius-caesar-dekripsi.png)

| Keterangan | Nilai/isi dari naskah |
|-------|--------|
| Naskah Asli | Jangan rahasiakan pesan ini! |  
| Naskah Setelah Di Acak | Mdqjdq udkdvldndq shvdq lql! | 

Tingkat kesukaran known-plaintext attack tergantung pada rumus yang digunakan untuk enkripsi. Semakin rumit rumus yang digunakan, semakin sukar untuk melakukan known-plaintext attack. Rumus yang bersifat linear masih tergolong sederhana dan dianggap rentan terhadap known-plaintext attack. Semakin non-linear dan semakin banyak parameter yang digunakan untuk rumus, semakin sulit untuk mengkalkulasi kunci berdasarkan rumus.

_sumber : Teori dan Aplikasi Kriptografi  
Penulis: Sentot Kromodimoeljo  
Januari 2010_
