---
published: false
---
## Operasi Dasar

Operasi terpenting terhadap unit data dalam kriptografi adalah exclusive or (xor), seperti yang digunakan pada enkripsi one-time pad.  

Jika one-time pad dapat digunakan dalam skala besar, maka enkripsi hanya memerlukan operasi xor. Akan tetapi, one-time pad tidak praktis untuk penggunaan skala besar, oleh sebab itu diperlukan operasi lainnya yaitu substitusi dan permutasi.  

Substitusi adalah proses penukaran unit data secara utuh, seperti yang dilakukan dalam Caesar cipher dimana huruf ditukar dengan huruf. Operasi ini membuat efek confusio (pembingungan) terhadap analisa statistik. Spesifikasi dan implementasi operasi ini dapat dilakukan menggunakan tabel jika tabel tidak terlalu besar, dengan nilai yang hendak ditukar digunakan sebagai indeks tabel, dan nilai dalam tabel digunakan sebagai nilai penukar. Contoh dari operasi substitusi menggunakan tabel adalah operasi substitusi S1 yang digunakan algoritma DES, seperti terlihat pada tabel dibawah. Tabel mempunyai 4 baris (dengan indeks 0,1,2,3) dan 16 kolom (dengan indeks 0 sampai dengan 15). Input 6 bit digunakan sebagai indeks baris dan kolom, dengan bit 1 dan bit 6 menentukan indeks baris dan bit 2  sampai dengan bit 5 menentukan indeks kolom. Sebagai contoh, jika input 6 adalah 011011, maka indeks baris adalah 1 (karena bit 1 dan bit 6 mempunyai nilai dari 0 ujung kiri dan 1 ujung kanan ketika didesimalkan maka menjadi 1), dan indeks kolom adalah 13 (karena bit 2, 3, 4, dan 5 mempunyai nilai 1101 ketika didesimal kan maka menjadi 13). Dengan input 011011, S1 akan menghasilkan 4 bit 0101 karena berasal dari baris 1 kolom 13 yang telah dihitung diatas tadi dan dalam tabel S1 mempunyai nilai 5 pada baris 1 kolom 13, yang dalam notasi biner 4 bit adalah 0101.  

Jika tabel terlalu besar, biasanya operasi substitusi mempunyai rumus untuk mengkalkulasi nilai  tukar, seperti rumus enkripsi Caesar cipher dan rumus untuk S-box AES. Caesar cipher dan S-box untuk DES tidak memiliki rumus yang elegan, dapat juga diimplementasikan menggunakan tabel karena tabel tidak terlalu besar. Akan tetapi, S-boxes untuk DES tidak memiliki rumus yang elegan, jadi biasanya diimpermentasikan menggunakan tabel.  

Permutasi adalah proses penukaran posisi dalam unit data. Operasi ini membuat efek diffusion (pembauran) yang mempersulit analisa statistik. Dalam kriptografi,  komponen data dalam operasi permutasi biasanya berupa bit. Contoh operasi permutasi adalah Initial Permutation yang digunakan algoritma DES, seperti terlihat pada tabel dibawah ini. Posisi akhir bit digunakan sebagai indeks tabel, jadi nilai output bit n sama dengan nilai input bit T (n) dimana T (n) adalah nilai komponen n dalam tabel.  

Sebagai contoh, nilai output bit 1 sama dengan nilai input bit 58 pada tabel dibawah ini, karena komponen pertama dalam tabel mempunyai nilai 58. Permutasi bit dapat diimplementasikan dalam hardware secara efisien karena hanya dibutuhkan koneksi antara posisi awal bit dengan posisi akhir bit. Jadi untuk Initial Permutation hanya diperlukan 64 koneksi (karena jumlah dari semua bit dalam tabel adalah 64), dengan bit 58 input menjadi bit 1 output, bit 50 input menjadi bit 2 output, dan seterusnya.  

Initial permutation