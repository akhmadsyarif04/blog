---
published: false
---
# SVM (Support Vector Machine)

SVM bekerja dengan baik pada set data dengan dimensi yang tinggi, bahkan SVM yang menggunakan teknik kernel harus memetakan data asli dari dimensi asalnya menjadi dimensi lain yang relatif lebih tinggi. Pada SVM hanya sejumlah data terpilih saja yang berkontribusi untuk membentuk model yang digunakan dalam klasifikasi yang akan dipelajari. Dan SVM hanya menyimpan sebagian data kecil saja dari data latih yang digunakan pada saat prediksi. Sehingga tidak semua data latih yang dilibatkan dalam setiap iterasi pelatihannya. Data-data yang berkontribusi tersebut disebut **_Support Vector_** sehingga metodenya juga disebut **_Support Vector Machine_**.

## Konsep SVM
Ide dasar dari SVM adalah memaksimalkan batas Hyperlane, yang di ilustrasikan pada gambar dibawah ini. Pada gambar a ada sejumlah pilihan Hyperlane yang mungkin untuk set data, sedangkan gambar b merupakan Hyperlane dengan margin yang paling maksimal.

![decision boudary](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/svm-matlab-decision-boundary.jpg)




Sumber : _Buku Data Mining Mengolah data menjadi informasi menggunakan MATLAB_

