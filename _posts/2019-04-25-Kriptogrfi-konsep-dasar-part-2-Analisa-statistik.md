---
published: false
---
## Analisa Statistik

Semua algoritma enkripsi sebelum data encryption standard (DES) rentan terhadap analisa statistik, kecuali one-time pad. Sebagai contoh, mari lihat bagaimana enkripsi dengan cara Shift transformation seperti Caesar Cipher yang rentan terhadap cara enkripsi analisa statistik yang sederhana yaitu analisa frekuensi.

Enkripsi dengan cara Shift transformation sangat rentan terhadap analisa frekuensi sebagai berikut: dengan rumus enkripsi  
> C ≡ P + b (mod n)

jika n diketahui dan sepasang C dan P dapa diterka dengan akurat, maka parameter b (kunci) dapat dicari. Setiap “pencarian” b  dapat dicoba cukup dengan sepasang nilai untuk C dan P.  Sebagai contoh menggunakan naskah acak pada tabel enkripsi dengan caesar cipher, huruf “D” dan “Q” adalah yang terbanyak digunakan dalam naskah acak. Karena dalam bahasa Indonesia, Huruf “A” adalah huruf dengan statistik penggunaan terbesar. Jika naskah asli dalam bahasa Indonesia , maka besar kemungkinan huruf “D” atau “Q” merupakan huruf acak untuk “A”. Jadi besar kemungkinan, jika kita menggunakan kode untuk “D” atau “Q” sebagai nilai C dan kode untuk “A” sebagai nilai P, rumus enkripsi akan menghasilkan nilai b yang benar. Jadi mari coba 2 kemungkinan: pasangan “D-A” (yang menghasilkan b = 3) dan pasangan “Q-A” (yang menghasilkan b = 16). Hasil yang dicari adalah nilai b yang jika digunakan untuk mendekripsi naskah acak akan menghasilkan naskah asli yang “masuk akal”.

Hasil analisa frekuensi
	
berdasarkan hasil analisa frekuensi, yang “masuk akal” hanya b=3 dengan hasil dekripsi “Jangan rahasiakan pesan ini!”, jadi kita dapat cukup yakin bahwa parameter b=3.
	Analisa frekuensi diatas didasarkan pada pengetahuan bahwa naskah asli adalah dalam bahasa Indonesia, dimana huruf “A” lebih dominan. Tentunya naskah asli tidak akan selalu mempunyai statistik penggunaan akan mirip dengan data empiris, yang berarti semakin besar kemungkinan analisa frekuensi akan sukses.

Data empiris adalah suatu sumber pengetahuan yang diperoleh dari observasi atau percobaan. 

	Untuk shift transformation, karena rumus transformasi sangat sederhana hanya dengan satu parameter, setiap percobaan cukup dengan menggunakan satu persamaan. Strategi pencarian yang baik adalah dengan mencoba pasangan yang mempunyai frekuensi penggunaan yang besar (huruf acak yang  frekuensinya besar dalam naskah acak dipasangkan dengan huruf asli yang frekuensinya juga besar menurut data empiris). Semakin besar frekuensi terbesar dalam data empiris, secara umum berarti semakin besar redundancy dari segi teori informasi, yang akan mempermudah analisa frekuensi.
	Jika rumus transformasi lebih rumit dengan lebih dari satu parameter. Maka setiap percobaan harus dilakukan dengan lebih dari satu persamaan, dengan banyaknya persamaan yang dibutuhkan sedikitnya sama dengan banyaknya parameter yang harus dicari.
	Untuk sukses dalam analisa frekuensi, dibutuhkan pengetahuan empiris mengenai statistik penggunaan huruf, naskah acak yang dapat dianalisa harus cukup besar, rumus atau seminimnya jenis enkripsi harus diketahui (jika rumus tidak diketehui tetapi jenis enkripsi diketahui berupa simple substitution, setiap huruf acak harus dipasangkan dengan huruf asli. Untuk analisa frekuensi yang rumit, penggunaan komputer sangat membantu.