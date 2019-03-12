---
layout: post
title: Vuetify part 2 Memulai Koding Vuetify dan Menggunakan Component Text dan Color
categories: vuetify
tags:
  - vuetify
published: true
---
## Memulai ngoding dengan component Vuetify.

Sebelumnya kita telah membuat project baru dan installasi vuetify pada vue.js kita.
Sakarang mari kita belajar menambahkan dan mengedit vuetify pada project kita sendiri.
Dimana letak tamplate buat tampilan website nya? jadi didalam vue.js ada pada folder 
```html
/src 
```
didalam folder project. Disana ada file dengan nama app.vue. lihat gambar dibawah

![DeepinScreenshot_select-area_20190312164123.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190312164123.png)

jadi pada file app.vue itu adalah root atau file utama untuk menampilkan tamplate ke halaman browser. artinya juga bisa dibilang disinilah tamplate dari vuetify dirender menjadi html.

- Folder component itu berisi file component yang mau kita letahkan pada tampilan tamplate. misalnya : header, footer, navigasi headbar dan lain-lain.  
- Folder views adalah berisi file tamplate sesuai dengan nama konten. misal konten pada HOME, BIODATA, ARTIKEL dan lain-lain.  
- Folder plugin adalah berisi plugin yang kita install. seperti pada part 1 kita menginstall vuetify pada project kita (vue.js kita) maka disitu akan muncul vuetify.
- Folder asset adalah berisi aset-aset berharga kita yang diupload, misal nya gambar dan video.
- File Router adalah sebagai tempat yang menentukan file tamplate mana yang akan dijalankan pada folder views. misalnya kita mau ke konten BIODATA tidak mungkin kita tampilkan semua file pada folder views. Jadi didalam file router ketika kita mau ke konten BIODATA maka file router akan merender file BIODATA tergantung permintaan pada bagian path, bagian name untuk penamaan, pada component adalah file akan dipanggil jika path sesuai dengan yang diminta.

Jelas ya untuk masalah folder pada folder /src yang kita gunakan untuk tampilan website kita. 
Sekarang mari kita mulai belajar component vuetify.

1. silahkan kalian hapus terlebih dulu pada bagain app.vue menjadi seperti ini.
![DeepinScreenshot_select-area_20190312170737.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190312170737.png)

> Keterangan  
1  ```<v-content></v-content>``` tempat dimana file pada views akan ditampilkan. bisa dibilang tempat menampilkan konten yang telah dibuat pada folder views.  
2 ```<router-view></router-view>``` untuk menggunakan file router seperti yang dijelaskan diatas.

*pada bagian script dibahas 1 per 1 ketika kita masuk materi menggunakan script tersebut nanti atau pada artikel/tutorial pada vue.js nanti yang akan saya buat atau silahkan cari digoogle. :D


2. delete file HelloWorld.vue pada folder components.
3. masuk folder views, pada file home sesuaikan seperti dibawah ini
![DeepinScreenshot_select-area_20190312172358.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190312172358.png)

4. lalu kita jalan kan dengan perintah 
```html
npm run serve
```
tunggu hingga berhasil dan mengeluarkan App running at. 

5. Hasil nya akan seperti ini dibrowser.
![DeepinScreenshot_select-area_20190312172602.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190312172602.png)

penjelasan :   
``` <p class="red white--text"> ``` 
> red = adalah untuk background dari text  
white--text = untuk pewarnaan pada text

untuk penamaan color bisa kalian rubah default dari vuetify pada folder plugins -> file vuetify.js tambahkan 
script seperti dibawah ini

```javascript
theme: {
    primary: '#9652ff',
    success: '#3cd1c2',
    info: '#ffaa2c',
    error: '#f83e70'
  }
```
maka seluruh script pada file vuetify.js seperti gambar ini :
![DeepinScreenshot_select-area_20190312194523.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190312194523.png)


untuk daftar color pada vuetify bisa kalian lihat disini : [https://vuetifyjs.com/en/framework/colors#colors](https://vuetifyjs.com/en/framework/colors#colors)

penjelasan :
``` <p class="pink lighten-4 red--text"> ```  
> lighten-4 = adalah agar contrass cahaya terang pada background. lebih besar maka lebih terang, lebih kecil maka akan gelap.  
jika pada text maka text--darken-4.

penjelasan :
``` <h1 class="display-4"> ```  
> display-4 = untuk memperbesar text atau font beda dengan h1 h2 dll.  
misalkan aja pada display-1 dengan h1 pada header Homepage. bisa dilihat bahawa display-1 lebih besar dibanding h1

penjelasan : 
``` <p class="subheading font-weight-bold"> ```
