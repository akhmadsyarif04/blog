---
layout:     post
title:      Breadth First Search
categories: Artificial-Intelligent
tags:
 - AI
published: true
---
## Breadth First Search

Pencarian dilakukan pada semua level dengan cara per baris level secara beurutan. Dari kiri ke kanan. Jika telah sampai dilevel terakhir maka dilanjutkan ke bagian bawah dari sebelah kiri lagi dan seterusnya. Dengan cara seperti ini BFS menjamin ditemukan nya solusi dengan catatan jika solusi nya emang benar ada dan mengambil solusi yang terbaik jika terdapat 1 lebih solusi yang ditemukan. BFS memiliki pemakaian memori yang besar karena BFS perlu menyimpan semua tingkatan yang telah diproses sebelumnya. Jika _b_ adalah faktor percabangan (jumlah simpul anak yang dimiliki oleh suatu simpul) dan _d_ adalah kedalaman solusi (tingkatan), maka jumlah simpul yang harus disimpan adalah sebanyak O(b<sup>d</sup>). Misalkan, untuk _b_ = 10 dan _d_ = 8, maka BFS harus  membaca dan menyimpan sebanyak 10<sup>0</sup> + 10<sup>1</sup> + 10<sup>2</sup> + 10<sup>3</sup> + 10<sup>4</sup> + 10<sup>5</sup> + 10<sup>6</sup> + 10<sup>7</sup> + 10<sup>8</sup> = 111.111.111 = 10<sup>8</sup> simpul. Waktu proses yang dibutuhkan untuk menemukan solusi dilevel 8 adalah 100 detik (1,67 menit). Jika suatu simpul diproses dalam struktur data sebesar 10<sup>15</sup> bytes (10 gigabytes). Dari segi kecepatan masih bisa diterima. Tapi dari sisi memori yang diperlukan. Dengan permasalahan dan komputer yang sama , waktu proses yang diperlukan untuk menemukan solusi dilevel 14 adalah 10<sup>8</sup> detik (lebih dari 3 tahun) dan diperlukan memori sebesar 10<sup>15</sup> bytes (1.000 terabytes). Itu yang menjadi kan BFS menjadi sulit di implementasikan didunia nyata. 

![BFS.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/BFS.png)
