---
published: false
---
## Cara Kerja Ethernet

Pada dasarnya penggunaan ethernet adalah berbagi kabel. Yaitu lebih dari 2 buah komputer (atau lebih) dapat menggunakan 1 kabel untuk berkomunikasi secara bersamaan. Proses komunikasi yang dilakukan pada ethernet adalah dengan cara bergantian dikarenakan menggunakan 1 kabel saja. Bisa diasumsikan dengan cara sekelompok orang yang sedang berbicara dalam 1 buah kelompok pembicaraan. Jika ada seseorang yang sedang bicara maka yang lain harusnya diam dan mendengarkan, tapi jika ada yang ikut berbicara juga maka orang lain akan terganggu. Maka dari itu agar orang lain tidak terganggu maka harus melakukan giliran dalam berbicara.  
	
Begitu juga jaringan ethernet ini, ketika ada 2 komunikasi atau proses data (baik pengiriman/penerimaan) dalam 1 jaringan/kabel maka akan terjadi tabrakan (collision). Sebelum card ethernet melakukan pengiriman data, dia harus mendeteksi lebih dulu ada tidaknya card lain yang sedang menggunakan kabel atau jaringan. Jika tidak ada maka data akan dikirimkan. Jikda ada card ethernet akan menunggu sampai kabel atau jaringan dalam keadaan kosong. Collision dideteksi oleh card dengan memeriksa kabel, yang mana jika tegangan pada kabel melebihi batas tertentu berarti terjadi collision.  

Ketika collision terjadi masing-masing dari card akan berhenti melakukan pengiriman data dan menunggu lagi dengan selang waktu yang acak untuk mencoba mengirim kembali data. Selang waktu acak yang ada pada pengiriman ketika terjadi collision ini memungkinkan collision lebih lanjut menjadi lebih kecil. Proses tersebut dikenal dengan CSMA/CD (Carrier Sense Mulple Access/Collision Detection).  

Untuk mengenali dan membedakan setiap card ethernet telah tertera kode khusus sepanjang 48 bit, yang dikernal sebagai ethernet address atau MAC Address.
