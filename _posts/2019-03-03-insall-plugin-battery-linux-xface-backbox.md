---
layout:     post
title:      install plugin battery xface
categories: linux
tags:
 - linux
 - backbox
 - xface
published: true
---
Kemaren saya mengalami tragedi dimana tragedi tersebut sangat-sangat mengesalkan, yaitu icon plugin battery panel dilinux backbox saya HILANG.. bukan hanya icon nya tapi juga plugin nya ikut hilang. T_T
Saya juga tidak tau penyebab nya apa. Jadi saya langsung searching google cara mengembalikan icon battery tapi tidak pernah ketemu. Hampir semua tutorial yang saya cari cuman untuk memasang icon panel battery nya saja bukan mengembalikan plugin nya.

Oke langsung saja, { pada kasus ini saya menggunakan backbox }

1. buka terminal kalian dan ketikan perintah ini :
```html
sudo apt-get update
sudo apt-get install xfce4-battery-plugin
```

2. setelah itu klik kanan pada panel
3. pilih panel
4. pilih add new items
5. cari battery
6. klik dan add
tralaaaa, plugin dan icon battery kembali ada.

Semoga bermanfaat.. ^_^ Thanks untuk https://www.howtoinstall.co/en/ubuntu/utopic/xfce4-battery-plugin .
