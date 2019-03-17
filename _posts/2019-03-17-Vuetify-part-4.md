---
published: false
---
## Breakpoint dan Display

Pada tutorial sebelum nya kita sudah mencoba button dan icon. nah sekarang kita coba bagian breakpoint dan display. silahkan kalian masuk ke website resmi dari vuetifyjs.com [breakpoints](https://vuetifyjs.com/en/framework/breakpoints#breakpoints) dan [Display](https://vuetifyjs.com/en/framework/display#visibility). saya akan mencoba menjelaskan pada bagian breakpoin. disana terdapat table Viewport yang mana macam-macam ukuran device. 

> 
``xs`` (_extra small_) yaitu lebar nya (<600px) kurang dari 600px maka true.  
``sm`` (_small_) yaitu lebarnya kurang dari 960px maka true.  
``md`` (_medium_) yaitu lebarnya kurang dari 1264px maka true.  
``lg`` (_large_) yaitu lebarnya kurang dari 1904px maka true.  
``xl`` (_extra large_) yaitu lebarnya ( > 1904px) lebih dari 1904px maka true.

disana juga tercantum type dari setiap ukuran, adan tablet, laptop, dan dekstop.

langsung praktek aja. 
1. buka kembali file home.vue kalian, hapus script terdahulu dan ketikan dibawah ini.
```html
    <v-btn class="hidden-md-and-down">Click me</v-btn>
```

maka jadi seperti ini bagian home.vue
![DeepinScreenshot_select-area_20190317190621.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190317190621.png)

2. lalu jalan kan _npm run seve_ dan check dibrowser
![DeepinScreenshot_select-area_20190317190730.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190317190730.png)
akan terlihat normal seperti biasa.

3. klik kanan dan _inspect element_.
4. pilih icon ini, pada pojok kanan. (_note: saya menggunakan firefox_)
![DeepinScreenshot_select-area_20190317190947.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190317190947.png)
