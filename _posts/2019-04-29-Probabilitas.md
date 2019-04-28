---
layout:     post
title:      Probabilitas
categories: Artificial-Intelligent
tags:
 - AI
published: true
---
## Probabilitas

Probabilitas atau peluang adalah suatu ukuran tentang kemungkinan suatu peristiwa (event) akan terjadi dimasa mendatang. Bisa juga diarti kan sebagai angka yang menunjukkan seberapa besar kemungkinan suatu peristiwa terjadi, diantara keseluruhan peristiwa yang mungkin terjadi.  dilambang kan degan P.  
Contoh : sebuah dadu untuk keluar mata ‘lima’ saat pelemparan dadu tersebut satu kali adalah 1/6 (kenapa 6 karena permukaan dadu ada 6).   
Rumus :  
> P (E) = X/N  

P : Probabilitas  
E : Event  
X : Jumlah kejadian yang diinginkan (peristiwa)  
N : Keseluruhan kejadian yang mungkin terjadi  

Probabilitas yang rendah menunjukkan kecilnya kemungkinan suatu peristiwa akan terjadi. Suatu probabilitas dinyatakan antara 0 dan 1 atau dalam persentase. Probabilitas 0 menunjukan peristiwa yang tidak mungkin terjadi, sedangkan probabilitas 1 menunjukan peristiwa yang pasti terjadi. 3 hal penting dalam probabilitas, yaitu :  
1. Percobaan adalah pengamatan terhadap beberapa aktivitas atau proses yang memungkinkan timbulnya paling sedikit peristiwa tanpa memperhatikan peristiwa man yang akan terjadi.
2. Hasil adalah suatu hasil dari sebuah percobaan.
3. Peristiwa adalah kumpulan dari satu atau lebih hasil yang terjadi pada sebuah percobaan atau kegiatan.

Untuk mengetahui besarnya kemungkinan dihitung dari prosentase jumlah premis yang dialami :

![1.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/1.png)

Untuk mengetahui besarnya kemungkinan dihitung dari prosentase jumlah bobot premis yang dialami :

![2.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/2.png)

Probabilitas Klasik yaitu pendekatan berdasarkan pada sebuah peristiwa mempunyai kesempatan untuk terjadi sama besar (equally likely). Probabilitas suatu peristiwa kemudian dinyatakan sebagai suatu rasio antara jumlah kemungkinan hasil dengan total kemungkinan hasil (rasio peristiwa terhadap hasil).

Probabilitas suatu peristiwa = jumlah kemungkinan hasil / jumlah total kemungkinan hasil
Jika ada a kemungkinan yang dapat terjadi pada kejadian A dan ada b kemungkinan yang dapat terjadi pada kejadian A, serta masing-masing kerjadian mempunyai kesempatan yang sama dan saling asing, maka probabilitas/peluang bahwa akan terjadi a adalah :  

> P (A) = a/a+b; dan peluang bahwa akan terjadi b adalah: P (A) = b/a+b

Contoh :  
Pelamar pekerjaan terdiri dari 10 orang pria (A) dan 15 orang wanita (B). Jika yang diterima hanya 1, berapa peluang bahwa ia merupakan wanita ?  
Jawab :  
> P (A) = 15/10+15 = 3/5

Probabilitas teorema bayes adalah teorema yang digunakan untuk menghitung peluang dalam suatu hipotesis. Teorema bayes dikembangkan dengan berbagai ilmu termasuk untuk penyelesaian masalah sistem pakar dengan menentukan nilai probabilitas dari hipotesa pakar dan nilai evidence yang didapatkan fakta yang didapat dari objek yang diagnosa.
Misalkan kawan Anda bercerita dia bercakap-cakap akrab dengan seseorang lain di atas kereta api. Tanpa informasi tambahan, peluang dia bercakap-cakap dengan perempuan adalah 50%. Sekarang misalkan kawan Anda menyebut bahwa orang lain di atas kereta api itu berambut panjang. Dari keterangan baru ini tampaknya lebih bolehjadi kawan Anda bercakap-cakap dengan perempuan, karena orang berambut panjang biasanya wanita. Teorema Bayes dapat digunakan untuk menghitung besarnya peluang bahwa kawan Anda berbicara dengan seorang wanita, bila diketahui berapa peluang seorang wanita berambut panjang.   

Misalkan:   
W adalah kejadian percakapan dilakukan dengan seorang wanita.  
L adalah kejadian percakapan dilakukan dengan seorang berambut panjang  
M adalah kejadian percakapan dilakukan dengan seorang pria  

Kita dapat berasumsi bahwa wanita adalah setengah dari populasi. Artinya peluang kawan Anda berbicara dengan wanita, 

> P (W) = 0,5 

Misalkan juga bahwa diketahui 75 persen wanita berambut panjang. Ini berarti bila kita mengetahui bahwa seseorang adalah wanita, peluangnya berambut panjang adalah 0,75. Kita melambangkannya sebagai:  

> P (L | W) = 0,75

Sebagai keterangan tambahan kita juga mengetahui bahwa peluang seorang pria berambut panjang adalah 0,3. Dengan kata lain: 
  
>  P (L | M) = 0,3 

Di sini kita mengasumsikan bahwa seseorang itu adalah pria atau wanita, atau P(M) = 1 - P(W) = 0,5. Dengan kata lain M adalah kejadian komplemen dari W.  
Tujuan kita adalah menghitung peluang seseorang itu adalah wanita bila diketahui dia berambut panjang, atau dalam notasi yang kita gunakan, P(W|L). Menggunakan teorema Bayes, kita mendapatkan: 

![3.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/3.png)

Di sini kita menggunakan aturan peluang total. Dengan memasukkan nilai-nilai peluang yang diketahui ke dalam rumus di atas, kita mendapatkan peluang seseorang itu wanita bila diketahui dia berambut panjang adalah 0,714. Angka ini sesuai dengan intuisi awal kita, bahwa peluang kawan kita itu bercakap-cakap dengan wanita meningkat. 
Secara umum, teorema bayes dinyatakan sebagai : 

![4.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/4.png)

Dalam notasi ini P(A|B) berarti peluang kejadian A bila B terjadi dan P(B|A) peluang kejadian B bila A terjadi.
