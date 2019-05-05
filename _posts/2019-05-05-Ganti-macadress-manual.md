---
layout:     post
title:      Ganti Mac Address Manual
categories: linux
tags:
 - linux
 - jaringan
published: true
---
## Ganti Mac Address Manual

Mengganti mac address manual :   
`` ifconfig ``  
pada contoh kali ini mac yang dirubah adalah mac eth0  

`` ifconfig eht0 down ``  
matikan terlebih dulu eth0 nya.  
``Ifconfig eth0 ether 00:11:2w:23:d1:3e``  
> ifconfig <jaringan yang dirubah> <bagian yang rubah> <mac baru>  

`` ifconfig eth0 up ``  
lalu dihidupkan lagi jaringan eth0 nya.  
`` Ifconfig ``  
dan sekarang lihat perubahan mac eth0.
