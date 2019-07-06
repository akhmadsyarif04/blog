---
published: false
---
## Scanning Network

>> netdiscover -r 10.0.2.1/24

ip yang digunakan adalah ip inet yang terhubung dari subnet 1-24.

Jadi dalam jaringan berkomunikasi antar perangkat adalah dengan mengetahui mac setiap komputer, bukan dari ip.
Ketika kita mendapatkan ip address kita belum mmengetahui mana kah alamat pc lain, yang kita tahu hanyalah ruang lingkup ip misal 192.168.1.1/24. Dari ip tersebut kita bisa menanyakan ke ip lain untuk mengetahui alamat yg dituju atau mac address komputer lain.

misalnya, dari ringkup ip diatas tadi bisa kita broadcast(kirim pesan kesemua) siapa pemilik ip 192.168.1.1. Ketika ada komputer yang menggunakan ip tersebut maka dia akan mengatakan atau ngeresponse, jika diasumsikan seperti manusia seperti ini "ini ip saya". dari situ lah kita bisa mendapatkan mac dari ip tersebut. (note: mac adalah alamat yang digunakan berkomunikasi didalam jaringan). 

>> ketika kita berkomunikasi didalam jaringan, itu menggunakan ARP (address resolution protokol).
