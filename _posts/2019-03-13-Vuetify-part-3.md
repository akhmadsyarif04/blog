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

Penjelasan :  
``` <v-btn class="pink white--text">Click Me</v-btn> ```
>  `` pink `` = adalah untuk color background.   
`` white--text `` = untuk color font.

Penjelasan :  
``` <v-btn depressed color="pink">Click Me</v-btn> ```
> ``` depressed ``` = 

