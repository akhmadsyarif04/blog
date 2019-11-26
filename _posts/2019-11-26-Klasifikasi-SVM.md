---
published: false
---
# SVM (Support Vector Machine)

SVM bekerja dengan baik pada set data dengan dimensi yang tinggi, bahkan SVM yang menggunakan teknik kernel harus memetakan data asli dari dimensi asalnya menjadi dimensi lain yang relatif lebih tinggi. Pada SVM hanya sejumlah data terpilih saja yang berkontribusi untuk membentuk model yang digunakan dalam klasifikasi yang akan dipelajari. Dan SVM hanya menyimpan sebagian data kecil saja dari data latih yang digunakan pada saat prediksi. Sehingga tidak semua data latih yang dilibatkan dalam setiap iterasi pelatihannya. Data-data yang berkontribusi tersebut disebut **_Support Vector_** sehingga metodenya juga disebut **_Support Vector Machine_**.

## Konsep SVM
Ide dasar dari SVM adalah memaksimalkan batas Hyperlane, yang di ilustrasikan pada gambar dibawah ini. Pada gambar (a) ada sejumlah pilihan Hyperlane yang mungkin untuk set data, sedangkan gambar (b) merupakan Hyperlane dengan margin yang paling maksimal.

![decision boudary](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/svm-matlab-decision-boundary.jpg)

Konsep klasifikasi dengan SVM dapat dijelaskan secara sederhana sebagai usaha mencari Hyperlane terbaik yang berfungsi sebagai pemisah duah buah kelas data pada input space (Nugroho, 2007). Gambar diatas memperlihatkan beberapa data yang merupakan anggota dari dua buah kelas data yaitu +1 dan -1. Data yang tergabung pada kelas -1 disimbolkan dengan bentuk lingkaran, sedangkan data pada kelas +1 disimbolkan dengan bentuk bujur sangkar.  

Hyperlane (batas keputusan) pemisah terbaik antara dua kelas dapat ditemukan dengan mengukur margin Hyperlane tersebut dan mencari titik maksimalnya. Margin adalah jarak antara Hyperlane dengan data terdekat dari masing-masing kelas. Data yang paling dekat disebut sebagai _Support Vector_. Garis solid pada gambar diatas (b) menunjukan Hyperlane yang terbaik, yaitu terletak tepat pada tengah-tengah kedua kelas, sedangkan data lingkaran dan bujur sangkar yang melewati garis batas margin (garis putus-putus) adalah _Support Vector_.



Sumber : _Buku Data Mining Mengolah data menjadi informasi menggunakan MATLAB_


