---
layout:     post
title:      Vuetify part 1 setup project 
categories: vuetify
tags:
 - vuetify
published: true
---
## Vuetify part 1 : setup project

> 
Vuetify adalah sebuah framework dari vuejs untuk mempercantik UI aplikasi website. Dan biasa nya digunakan pada vuejs.

Pertama-tama kalian harus installasi Vue CLI dulu. apa itu Vue CLI? jadi Vue CLI itu adalah perintah pada terminal untuk memudahkan dalam development application di Vue.js.   
Ketikan perintah dibawah ini diterminal :
```html
yarn global add @vue/cli
```
atau menggunakan npm seperti dibawah ini :

```html
npm install @vue/cli -g
```

Setelah Vue CLI terinstall mari kita coba buat project baru dengan perintah :
```html
vue create project-baru
```
> project-baru adalah nama project

![DeepinScreenshot_select-area_20190308142431.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190308142431.png)

jika muncul seperti gambar dibawah ini :

![DeepinScreenshot_select-area_20190308142341.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190308142341.png)

pilih sesuai kebutuhan kalian. saya sendiri memilih yang pertama *vueshop-template (vue-router, vuex, stylus, babel, pwa, eslint, unit-mocha)

selanjutnya, ketika pembuatan project selesai kita masuk ke folder project tersebut dengan perintah :

```html
cd project-baru
```

karena yang telah kita buat hanya sebuah project vue maka untuk menggunakan vuetify kita harus menambahkan package vuetify ke dalam project kita. dengan perintah :

```html
vue add vuetify
```

![DeepinScreenshot_select-area_20190308143120.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190308143120.png)

pilih default

selanjutnya tinggal jalan kan vue tersebut dengan perintah : 
```html
npm run serve
```

*note: jalankan npm run serve harus didalam folder project yang telah dibuat

tunggu hingga finish compiling. jika sukses maka ketikan dibrowser
```html
http://localhost:8080/
```

*note: untuk menjalankan dibrowser kalian harus menyesuaikan hasil ouput dari compiling pada bagian Local atau Network seperti pada gambar dibawah ini

![DeepinScreenshot_select-area_20190308143732.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190308143732.png)

maka tampilan browser akan jadi seperti ini :

![DeepinScreenshot_select-area_20190308143837.png](https://raw.githubusercontent.com/akhmadsyarif04/blog/gh-pages/_posts/DeepinScreenshot_select-area_20190308143837.png)


selesai semoga bermanfaat dan apabila ada kesalahan atau bingung silahkan comment dibawah. next part vuetify selanjut nya.
