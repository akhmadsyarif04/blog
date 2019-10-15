---
layout: post
title: Inisialisasi Pin I/O Digital
categories: Arduino
tags:
  - Arduino
published: true
---
## Inisialisasi Pin I/O Digital

Inisialisasi mode suatu pin I/O digunakan untuk mengatur penggunaan mode pin apakah pin tersebut digunakan sebagai pin input atau pin ouput. Untuk inisialisasi mode suatu pin dapat digunakan sintaks sebagai berikut:

``
pinMode(pin, mode);  
// pin = nomor pin  
// mode = INPUT atau OUTPUT  
``

Contoh :  
>> pinMode(1, INPUT);

>> pinMode(2, OUTPUT);


Pada perintah pertama adalah pin digital 1 Arduino diatur menjadi pin input. Pada perintah kedua adalah pin digital 2 Arduino diatur menjadi pin ouput. Untuk mengatur keadaan suatu pin yang telah diatur sebagai  pin ouput pada arduino, misalnya keadaan HIGH atau LOW pada suatu pin dapat digunakan sintaks berikut :  
``
digitalWrite(pin, value);  
// pin = nomor pin  
// value = HIGH atau LOW  
``

Contoh :  
>> digitalWrite(3, HIGH);

>> digitalWrite(4, LOW);


Pada perintah 1 digital pin 3 arduino diberi ouput dengan keadaan HIGH, sedangkan perintah 2 digital 4 arduino diberi ouput dengan keadaan LOW.  

Untuk membaca nilai atau keadaan pin tertentu pada arduino yang telah diatur sebagai pin INPUT dapat menggunakan sintaks berikut :  

``
int digitalRead(pin);  
// pin = nomor pin  
``

Perintah diatas akan mengembalikan nilai HIGH dan LOW.
