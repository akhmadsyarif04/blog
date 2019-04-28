---
layout:     post
title:      Forward Chaining
categories: Artificial-Intelligent
tags:
 - AI
published: true
---
## Forward Chaining

Forward chaining adalah pelacakan ke depan yang memulai dari sekumpulan fakta-fakta dengan mencari kaidah yang cocok dengan dugaan/hipotesa yang ada menuju kesimpulan. Dapat diartikan bahwa forward chaining adalah pelacakan dari informasi yang didapat sehingga menghasilkan kesimpulan. Contoh :  
    
if (Informasi Masukan)  
Then (Konklusi)  
If Lampu1 dinyalakan  
And lampu1 tidak menyala  
And lampu1 dihubungkan dengan sekring  
And sekring masih bagus  
Then Lampu1 rusak  
	
Dan berikut gambar cara kerja metode forward chaining :  

![forward chaining.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/forward chaining.png)


Urutatan langkah forward chaining :  
1. Tampilkan semua daftar premis.
2. User memilih premis yang dialami
3. Sistem mencari aturan yang premisnya terdiri dari premis-premis yang dipilih oleh user.
4. Sistem akan menampilkan konklusi dari aturan tersebut.

Metode forward chaining cocok digunakan untuk menangani masalah pengendalian (controlling) dan peramalan (prediction). Contoh lagi forward chaining :  
Jika penderita terkena penyakit epilepsi Ideopatik dengan CF (Certain Factor) antara 0.4/0.6. Maka berikan obat carbamazepine.
