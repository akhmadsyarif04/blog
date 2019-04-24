---
published: false
---
## Brute Force Search / Brute Force

Salah saru kriteria bahwa sistem enkripsi  yang baik adalah apabila dekripsi tanpa kunci dan hanya dapat dipecahkan dengan cara brute force search yaitu dimana semua kemungkinan kunci dicoba. Semakin besar jumlah kemungkinan kunci yang dicoba maka semakin besar waktu yang dibutuhkan, dan semakin besar jumlah kemungkinan kunci semakin besar keberhasilan.

Untuk kunci sebesar n bits, jumlah kemungkinan kunci adalah 2<sup>n</sup>, kunci akan ditemukan setelah kita mencoba 2<sup>n-1</sup> kemungkinan (setengah dari semua kemungkinan). Jadi enkripsi rentan terhadap brute force search jika 2<sup>n</sup> kemungkinan kunci dapat dicoba dalam waktu yang tidak terlalu lama. Untuk waktu yang diperlukan juga tergantung dari hardware yang digunakan.

Besar kunci enkripsi ikut menetukan sukses dari brute force search. Dengan kemajuan dibidang hardware untuk melakukan brute force search (hardware khusus dapat dibuat untuk melakukan brute force search terhadap kunci block cipher), enkripsi block cipher dengan besar kunci 56 bit (jadi ada 256 kemungkinan) kini dapat dipecahkan dalam waktu yang tidak terlalu lama (kira-kira puluhan menit) dengan hardware seharga 1 juta USD. Dengan hardware yang lebih banyak, waktu yang diperlukan menjadi semakin singkat dengan perbandingan waktu inverse proportional (berbanding terbalik) terhadap harga. Untuk keamanan, sebaiknya enkripsi block cipher menggunakan kunci minimum 128bit. Data encryption standard (DES) hanya menggunakan 56bit untuk kunci, jadi sebaiknya diganti dengan 3DES atau block cipher lain seperti CAST, AES dan Blowfish.