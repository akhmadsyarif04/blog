---
layout:     post
title:      Depft First Search
categories: Artificial Intelligent
tags:
 - AI
published: true
---
## Depft First Search

Teknik ini melakukan pencarian pada setiap tingkatan atau level dari sebelah kiri sampai ke bagian terdalam terlebih dulu, jika solusi belum ditemukan maka lanjut ke sebelah kanan.  
Kelebihan DFS adalah pemakaian memori yang lebih kecil. DFS hanya menyimpan sekitar _bd_ simpul, di mana _b_ adalah fakor percabangan dan d adalah kedalaman solusi. Jika _b_ = 10 dan _d_ = 3, maka jumlah simpul yang disimpan di memori adalah 1 + 10 + 10 + 10 = 31.  

Kelemahan pada DFS adalah jika terdapat tingkatan yang 	sangat dalam maka tidak ada jaminan kalau solusi akan 	ditemukan. 	Dan jika terdapat 2 solusi yang ditemukan dilevel berbeda maka DFS tidak bisa menentukan solusi mana yang terbaik.

![DFS.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DFS.png)

