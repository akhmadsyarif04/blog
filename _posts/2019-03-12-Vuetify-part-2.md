---
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

![DeepinScreenshot_select-area_20190312164123.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190312164123.png)

jadi pada file app.vue itu adalah root atau file utama untuk menampilkan tamplate ke halaman browser. artinya juga bisa dibilang disinilah tamplate dari vuetify dirender menjadi html.

- Folder component itu berisi file component yang mau kita letahkan pada tampilan tamplate. misalnya : header, footer, navigasi headbar dan lain-lain.  
- Folder views adalah berisi file tamplate sesuai dengan nama konten. misal konten pada HOME, BIODATA, ARTIKEL dan lain-lain.  
- Folder plugin adalah berisi plugin yang kita install. seperti pada part 1 kita menginstall vuetify pada project kita (vue.js kita) maka disitu akan muncul vuetify.
- Folder asset adalah berisi aset-aset berharga kita yang diupload, misal nya gambar dan video.
- File Router adalah sebagai tempat yang menentukan file tamplate mana yang akan dijalankan pada folder views. misalnya kita mau ke konten BIODATA tidak mungkin kita tampilkan semua file pada folder views. Jadi didalam file router ketika kita mau ke konten BIODATA maka file router akan merender file BIODATA tergantung permintaan pada bagian path, bagian name untuk penamaan, pada component adalah file akan dipanggil jika path sesuai dengan yang diminta.

Jelas ya untuk masalah folder pada folder /src yang kita gunakan untuk tampilan website kita. 
Sekarang mari kita mulai belajar component vuetify.

1. silahkan kalian hapus terlebih dulu pada bagain app.vue menjadi seperti ini.
![DeepinScreenshot_select-area_20190312170737.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190312170737.png)

> Keterangan  
1  ```html<v-content></v-content>``` tempat dimana file pada views akan ditampilkan. bisa dibilang tempat menampilkan konten yang telah dibuat pada folder views.
2 ```html<router-view></router-view>``` untuk menggunakan file router seperti yang dijelaskan diatas.

*pada bagian script dibahas 1 per 1 ketika kita masuk materi menggunakan script tersebut nanti atau pada artikel/tutorial pada vue.js nanti yang akan saya buat atau silahkan cari digoogle. :D


2. delete file HelloWorld.vue pada folder components.
3. masuk folder views, pada file home sesuaikan seperti dibawah ini
![DeepinScreenshot_select-area_20190312172358.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190312172358.png)

4. lalu kita jalan kan dengan perintah 
```html
npm run serve
```
tunggu hingga berhasil dan mengeluarkan App running at. 
4. Hasil nya akan seperti ini kalau kita jalan kan
