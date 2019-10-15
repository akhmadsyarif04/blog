---
published: false
---
## Inisialisasi Pin I/O Digital

Inisialisasi mode suatu pin I/O digunakan untuk mengatur penggunaan mode pin apakah pin tersebut digunakan sebagai pin input atau pin ouput. Untuk inisialisasi mode suatu pin dapat digunakan sintaks sebagai berikut:

``
pinMode(pin, mode);  
// pin->nomor pin  
// mode-> INPUT atau OUTPUT
``

Contoh :  
>> pinMode(1, INPUT);

>> pinMode(2, OUTPUT);


Pada perintah pertama adalah pin digital 1 Arduino diatur menjadi pin input. Pada perintah kedua adalah pin digital 2 Arduino diatur menjadi pin ouput. Untuk mengatur keadaan suatu pin yang telah diatur sebagai  pin ouput pada arduino