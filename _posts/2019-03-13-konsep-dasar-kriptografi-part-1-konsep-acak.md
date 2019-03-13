---
published: false
---
# Konsep Dasar Kriptografi part 1
## Konsep Acak

  Konsep acak (randomness) pada kriptografi adalah teknik yang tidak bisa ditebak atau tidak bersifat sistematis. Artinya penentukan nilai bersifat bebas tanpa ada aturan atau algoritma yang menentukan.  
  Sifat acak dapat dikaitkan dengan urutan events, dimana events selanjutnya dalam suatu urutan tidak mudah untuk ditebak  berdasarkan apa events sebelumnya. Sifat ini diperlukan dalam pembuatan kunci (key generation) supaya kunci dekripsi tidak mudah untuk ditebak.  
  
>Key generation merupakan kegiatan manajemen kunci dalam menghasilkan kunci yang acak dimana keacakan kunci merupakan bagian terpenting dalam menjamin kekuatan suatu kriptografi
  
  Sifat acak juga dapat dikaitkan dengan tidak adanya korelasi atau tidak adanya hubungan antara 2 nilai. Misal dari key dekripsi dengan key enkripsi tidak lah sama, maka bisa disebut acak. Atau jua key dekripsi A dengan key dekripsi B tidak lah sama. Dalam kriptografi, di inginkan adanya hubungan antar naskah asli dengan naskah acak atau kunci dengan naskah acak yang mana nantinya akan bisa ditebak. Ini untuk mempersulit analisa frekuensi (frekuensi analysis) atau analisa lebih canggih seperti linear cryptanalysis atau differential cryptanalysis.  
  
  
  Meskipun tidak sebenarnya acak, sesuatu yang pseudo-random berguna dan digunakan dalam kriptografi, tetapi harus dikombinasikan dengan sesuatu yang benar acak. Sebagai contoh, pseudo-random number generator dikombinasikan dengan sumber ukuran jumlah informasi didalam pesan (entropi) yang benar acak sebagai kunci enkripsi (seed), untuk mendapatkan sesuatu yang praktis bersifat random number generator.  