---
layout: post
title: Konsep Dasar Kriptografi part 1 Konsep Acak
categories: kriptografi
tags:
  - kriptografi
published: true
---
# Konsep Dasar Kriptografi part 1
## Konsep Acak

  Konsep acak (*randomness*) pada kriptografi adalah teknik yang tidak bisa ditebak atau tidak bersifat sistematis. Artinya penentukan nilai bersifat bebas tanpa ada aturan atau algoritma yang menentukan.  
  Sifat acak dapat dikaitkan dengan urutan events, dimana events selanjutnya dalam suatu urutan tidak mudah untuk ditebak  berdasarkan apa events sebelumnya. Sifat ini diperlukan dalam pembuatan kunci (*key generation*) supaya kunci dekripsi tidak mudah untuk ditebak.  
  
>Key generation merupakan kegiatan manajemen kunci dalam menghasilkan kunci yang acak dimana keacakan kunci merupakan bagian terpenting dalam menjamin kekuatan suatu kriptografi
  
  Sifat acak juga dapat dikaitkan dengan tidak adanya korelasi atau tidak adanya hubungan antara 2 nilai. Misal dari key dekripsi dengan key enkripsi tidak lah sama, maka bisa disebut acak. Atau juga key dekripsi A dengan key dekripsi B tidak lah sama. Dalam kriptografi, tidak di inginkan adanya hubungan antar naskah asli dengan naskah acak atau kunci dengan naskah acak yang mana nantinya akan bisa ditebak. Ini untuk mempersulit analisa frekuensi (*frekuensi analysis*) atau analisa lebih canggih seperti *linear cryptanalysis* atau *differential cryptanalysis*.  

> Analisis Frekuensi (Frekuensi Analysis), yakni teknik untuk memecahkan ciphertext berdasarkan frekuensi kemunculan karakter pada sebuah pesan.

> Linear Cryptanalysis adalah teknik memecahkan enkripsi dengan cara membuat
perkiraan linear untuk algoritma enkripsi.

> Differential Cryptanalysis adalah teknik untuk mencari kunci
enkripsi dari analisa efek perbedaan naskah asli terhadap perbedaan naskah acak.
  
  Meskipun tidak sebenarnya acak, sesuatu yang *pseudo-random* berguna dan digunakan dalam kriptografi, tetapi harus dikombinasikan dengan sesuatu yang benar-benar acak. Sebagai contoh, *pseudo-random number generator* dikombinasikan dengan sumber *entropi* (**ukuran jumlah informasi didalam pesan**) yang benar acak sebagai *seed* (**kunci enkripsi**), untuk mendapatkan sesuatu yang praktis bersifat random number generator.

Part 2 tentang konsep dasar One-time pad.


_sumber : Teori dan Aplikasi Kriptografi  
Penulis: Sentot Kromodimoeljo  
Januari 2010_