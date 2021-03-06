---
layout: post
title: Vuetify part 3 Menggunakan Components Button Dan Icons
categories: vuetify
tags:
  - vuetify
published: true
---
## Menggunakan Components Button Dan Icons

Pada part 2 kemaren kita telah mengubah tampilan pada content home dengan mencoba components vuetify font dan color. Sekarang kita lanjut dengan mencoba components Button dan Icons.

Silahkan buka file Home.vue kalian pada folder Views.
Lalu gunakan script dibawah ini :

```html
    <v-btn class="pink white--text">Click Me</v-btn>
    <v-btn depressed color="pink">Click Me</v-btn>
    <v-btn flat color="pink">Click Me</v-btn>
```

maka tampilan file Home.vue seperti ini :
![DeepinScreenshot_select-area_20190313224423.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190313224423.png)

Dan hasil dibrowser ketika dijalankan ``` npm run serve ``` seperti gambar dibawah ini :

![DeepinScreenshot_select-area_20190314005422.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190314005422.png)

Penjelasan :  
``` <v-btn class="pink white--text">Click Me</v-btn> ```
>  `` pink `` = adalah untuk color background.   
`` white--text `` = untuk color font.

Penjelasan :  
``` <v-btn depressed color="pink">Click Me</v-btn> ```
> ``` depressed ``` =  menghapus shadow (bayangan) pada button.  
``` color="pink" ``` = untuk color background.

Penjelasan :
``` <v-btn flat color="pink">Click Me</v-btn> ```
> ``` flat ``` = menghapus background color pada button.

Selanjutnya tambahkan lagi script dibawah ini :
```html
        <v-btn drepressed class="pink white--text">
          <v-icon left>email</v-icon> <!-- icon dari material design icon -->
          <span>email me</span>
        </v-btn>

        <v-btn drepressed small class="pink white--text">
          <v-icon left small>email</v-icon> <!-- icon dari material design icon -->
          <span>email me</span>
        </v-btn>

        <v-btn drepressed large class="pink white--text">
          <span>email me</span>
          <v-icon right large>email</v-icon> <!-- icon dari material design icon -->
        </v-btn>

        <v-btn fab drepressed small dark color="purple">
          <v-icon>favorite</v-icon> <!--  icon dari material design icon -->
        </v-btn>
```

maka tampilan file Home.vue seperti ini :
![DeepinScreenshot_select-area_20190314005736.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190314005736.png)

Penjelasan :
```
        <v-btn drepressed class="pink white--text">
          <v-icon left>email</v-icon> <!-- icon dari material design icon -->
          <span>email me</span>
        </v-btn>
```
> `` v-icon `` = adalah untuk memanggil icon dari material desaign icon yang sudah include bersama vuetify.     
`` left `` pada `` v-icon `` = agar icon berada pada sebelah kiri dengan ada nya spasi atau jarak dengan teks. jika kita coba dengan menghapus left maka icon dan teks akan mepet berdekatan.  

Penjelasan :
```
        <v-btn drepressed small class="pink white--text">
          <v-icon left small>email</v-icon> <!-- icon dari material design icon -->
          <span>email me</span>
        </v-btn>
```
> `` small `` pada `` v-icon `` dan `` v-btn `` = jika pada ``btn`` button akan menjadi kecil. Jika pada ``v-icon`` maka icon yang mengecil. jadi tegantung dimana meletakkan prop small tersebut.

> prop adalah salah satu cara untuk berkomunikasi antar compunent, tetapi pada prop hanya dengan mengirim nilai saja tidak menerima, artinya nilai small yang sudah ditentukan vuetify dikirim untuk mengubah nilai size atribut tersebut. Karena pada vuetify prop small akan menjadi nama class ketika dirender yang mana nanti nilai class tersebut akan dibaca browser. silahkan check dengan klik kanan -> inspect element.

Pennjelasan : 
```
        <v-btn drepressed large class="pink white--text">
          <span>email me</span>
          <v-icon right large>email</v-icon> <!-- icon dari material design icon -->
        </v-btn>
```
> `` large `` adalah untuk memperbesar, kebalikan dari small tadi.  
`` right `` pada `` v-icon `` agar icon berada pada sebelah kenan dengan ada nya spasi atau jarak dengan teks. jika kita coba dengan menghapus right maka icon dan teks akan mepet berdekatan. 

Penjelasan :
```
        <v-btn fab drepressed small dark color="purple">
          <v-icon>favorite</v-icon> <!--  icon dari material design icon -->
        </v-btn>
```
> `` fab `` untuk membuat button menjadi lingkaran.  
`` drepressed ``,``small``,``color`` sudah dibahas diatas.  
`` dark `` untuk menon aktifkan penggunakan color gelap/hitam. pada awal nya jika tidak digunakan dark icon akan menjadi hitam. ketika di gunakan dark akan menjadi putih. jadi prop dark ini default nya adalah *false* ketika digunakan.

Sekarang kita coba menu dropdown :  
ketikan script dibawah pada template
```
  <v-layout row wrap>
    <v-flex xs12 sm2>
      <v-overflow-btn :items="dropdown_font" label="Overflow Btn"></v-overflow-btn>
    </v-flex>
  </v-layout>
```
Jadi seperti ini ya  
![DeepinScreenshot_select-area_20190314105214.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190314105214.png)

Penjelasan : 
> ``:items="dropdown_font"`` adalah untuk menampilkan item-item dropdown yang nanti akan kita buat dibagian javascript data.  
``:item`` adalah shorthand ``v-bind:item`` yang mana digunakan untuk directive untuk mengambil sebuah component. 
``label`` hanya sebuah label saja.  
``v-flex`` adalah untuk mengatur grid atau kolom pada suatu element.  
``xs`` adalah extra small untuk bagian display antara (kurang dari) < 600px.  
``sm`` adalah small medium untuk bagian display antara 600px > < 960px.  
xs dan sm biasa nya digunakan untuk reponsive template. menyesuaikan dari ukuran layar.  
``v-layout`` biasa nya pasti berada diantar v-container dan v-flex untuk memisahkan antar 2 element tersebut.  
untuk ``wrap`` dan ``row`` saya masih bener-bener belum tau fungsi dari kedua itu. jika ada yang lebih tau silahka komen dibawah.

Lalu ketikan script js ini pada script  
```
export default {
  data: () => ({
    dropdown_font: ['Arial', 'Calibri', 'Courier', 'Verdana'],
  })
}
```
maka seperti ini
![DeepinScreenshot_select-area_20190314105310.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190314105310.png)

Penjelasan :
> ``data`` disitu adalah tempat untuk menuliskan variabel dan nilai. Dengan nama variabel nya adalah ``dropdown_font`` dan nilai ``['Arial', 'Calibri', 'Courier', 'Verdana']`` berbentuk array. Bisa juga berupa boolean, integer, string dll. variabel dropdown_font ini yang akan dipanggil nanti di item dropdown seperti yang dijelaskan diatas.

Gambar hasil component dropdown seperti ini :
![DeepinScreenshot_select-area_20190314114532.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190314114532.png)
![DeepinScreenshot_select-area_20190314114556.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190314114556.png)

okey, untuk lebih lanjut. silahkan kalian baca di documentasi web resmi mereka pada bagian button dan icon. disini [https://vuetifyjs.com/en/components/buttons#button](https://vuetifyjs.com/en/components/buttons#button).
