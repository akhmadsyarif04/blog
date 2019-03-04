---
layout:     post
title:      Apa itu ndisasm
categories: Linux
tags:
 - linux
 - assembly
published: true
---
Ndisasm adalah program untuk Netwide Assembler (NASM). NASM itu apa gan? jadi NASM itu adalah sebuah assembler dan disassembler untuk Intel arsitektur x86. ini juga bisa digunakan untuk menulis untuk 16-bit, 32-bit (IA-32), dan 64-bit (x85-64). NASM adalah assembler terkenal di kalangan linux.  

Ngomong-ngomong dari tadi kita bicara Assembler, apa itu assembler? jadi assembler itu adalah tool untuk menerjemahkan bahasa rakitan atau bisa juga disebut Assembly. Assembly adalah bahasa program tingkat rendah yang mana bahasa program tersebut mendekati bahasa mesin. Kalian tau kan bahasa mesin cuman mengenal 0 dan 1. contoh bahasa mesin :
![](https://www.dictio.id/uploads/db3342/original/3X/5/7/578465169337151d40334eacf60c39853ddf3b2b.jpg)

nah lo, pusing kan. wkwkwk  
maka dari itu dibuatlah bahasa program assembly yang mana lebih manusiawi. ya walaupun masih jauh juga sih. wkwkwk nih contoh bahasa assembly :
```html
section .text

global _start

_start:
pop rax ; pop number of argc (diabaikan)
pop rax ; pop argv[0] (diabaikan karena berisi nama program)
pop rax ; pop argv[1] (ini dipakai untuk stringtoint)
call stringtoint ; ECX berisi argument bertipe integer sebagai counter

_print:
push rcx    ; selamatkan counter di stack karena ECX dipakai juga di _print_hello
call _print_hello   ; print hello world
pop rcx      ; ambil lagi counter dari stack karena akan dipakai untuk looping 
loop _print     ; kurangi ECX 1, bila belum 0 kembali ke _print

; ini system call exit(0)
mov rbx,0
mov rax,1
int 0x80

_print_hello:   ; systemcall write(1, msg, len)
mov rdx,len
mov rcx,msg
mov rbx,1
mov rax,4
int 0x80
ret

stringtoint:  ; mengubah string dilokasi yang ditunjukan EAX menjadi integer di ECX
; EAX address of string
xor rcx,rcx     ; clear ECX
xor rbx,rbx    ; clear EBX
mov bl,[rax]    ; BL berisi kode ASCII string di lokasi yang ditunjuk EAX
sub bl,0x30    ; kode ASCII angka adalah 30h-39h, dikurangkan dengan 30h yang artinya berisi 0-9
add rcx,rbx     ; ECX ditambah EBX, ECX berisi nilai integer
ret

section .data
msg db "HELLO WORLD!", 0xa
len equ $ - msg

```

ini cuman untuk menampilkan HELLO WORLD aja. haha  

oke, cukup perkenalan nya. sekarang kita coba ndisasm pada terminal linux.

untuk melihat opsi dari ndisasm bisa kalian check dengan perintah :
```html
ndisasm -h
```

1. -h : untuk menampilkan opsi pada peritnah ndisasm.
2. -v : untuk menampilkan versi dari ndisasm yang sedang digunakan.
3. -o origin : untuk mendapatkan alamat memori yang ada pada sebelah kiri.
4. -s sync-point : Menentukan alamat sinkronisasi secara manual, sehingga ndisasm tidak akan mengeluarkan instruksi mesin apa pun yang mencakup byte di kedua sisi alamat. Oleh karena itu instruksi yang dimulai pada alamat itu akan dibongkar dengan benar.
5. -e bytes : Menentukan jumlah byte yang harus dibuang dari awal file sebelum memulai pembongkaran (assembly). Ini tidak diperhitungkan dalam perhitungan offset assembly: instruksi assembly pertama akan ditampilkan mulai dari alamat load yang diberikan.
6. -k start,bytes : menentukan panjang bytes ketika melakukan assembly. dimulai pada offset berapa, dan yang dilewati akan tetap diproses tapi tidak ditampilkan. 
7. -a atau -i : mengaktifkan metode sinkronisasi automatis, di mana ndisasm akan mencoba menebak di mana sinkronisasi harus akan dilakukan, dengan cara memeriksa alamat target dari relative jumps dan pemanggilan disassembles. 
8. -b : untuk menentukan dalam bentuk 16bit atau 32bit atau 64bit hasil conversi tersebut.
9. -u : untuk menentukan bentuk conversi nya menjadi 32bit, lebih spesifik dari pada -b 32.
10. -p vendor : menentukan jenis instruksi dari vendor mana. nama vendor seperti Intel, AMD, CYRIX, dan IDT. default nya adalah Intel.

contoh penggunakan ndisasm untuk conversi string ke assembly :
buat file test.txt dengan isi :
> We loved with a love that was more than love

kemudian jalankan diterminal pada folder tempat menyimpan file test.txt tadi
```html
ndisasm -b 64 test.txt
```
ouput nya seperti dibawah ini : 
![DeepinScreenshot_select-area_20190304110926.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190304110926.png)

- sebelah kiri adalah alamat memori.  
- tengah adalah urutan dari bytes (opcode dan operands) mewakilkan dari harsi intruction(instruksi) pada bahasa assembly sebelah kanan.  
- sebelah kanan adalah intruksi dari bahasa assembly.

Semoga bermanfaat dan mencoba. 

*jika ada kesalahan dalam blog ini mohon komentar dibawah agar penulis bisa memperbaiki, dan bermanfaat untuk orang lain. Terimakasih.

sumber : 
https://www.systutorials.com/docs/linux/man/1-ndisasm/  
https://en.wikipedia.org/wiki/Netwide_Assembler
