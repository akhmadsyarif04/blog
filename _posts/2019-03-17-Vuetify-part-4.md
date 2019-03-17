---
published: false
---
## Breakpoint, Visibilty, Overflow, dan Display

### Visibility dan Breakpoint
Pada tutorial sebelum nya kita sudah mencoba button dan icon. nah sekarang kita coba bagian breakpoint dan display. silahkan kalian masuk ke website resmi dari vuetifyjs.com [breakpoints](https://vuetifyjs.com/en/framework/breakpoints#breakpoints) dan [Display](https://vuetifyjs.com/en/framework/display). saya akan mencoba menjelaskan pada bagian breakpoin. disana terdapat table Viewport yang mana macam-macam ukuran device. 


disana juga tercantum type dari setiap ukuran, adan tablet, laptop, dan dekstop.

langsung praktek aja. 
jadi format dari visibility adalah ``hidden-{breakpoint}-{condition}``.  

> bagian breakpoint di isi dengan salah satu dari dibawah ini :  
``xs`` (_extra small_) yaitu lebar nya (<600px) kurang dari 600px maka true.  
``sm`` (_small_) yaitu lebarnya ( 600px >< 960px) kurang dari 600px dan kurang dari 960px maka true.  
``md`` (_medium_) yaitu lebarnya (960px >< 1264px) kurang dari 960px dan kurang dari 1264px maka true.  
``lg`` (_large_) yaitu lebarnya (1264px >< 1904px) kurang dari 1264px dan kurang dari 1904px maka true.  
``xl`` (_extra large_) yaitu lebarnya ( > 1904px) lebih dari 1904px maka true.

> bagian condition di isi dengan salah satu dari dibawah ini :  
``only`` = sembunyikan elemen sesuai aturan dari breakpoint hanya pada nilai size yang dilaluinya. misal breakpoint ``md`` yang memiliki 2 nilai, maka dibawah dari 1264px sampai 960px akan disembunyikan. dibawah 960px akan tampil dan diatas atau pas 1264px akan tampil juga.  
``and-down`` = sembunyikan elemen dari nilai size breakpoint tertinggi sampai size 0px. sedangkan diatas nilai size breakpoint akan ditampilkan.  
``and-up`` = menampilkan elemen dari nilai size breakpoint tertinggi sampai size 0px. sedangkan diatas nilai size breakpoint akan disembunyikan.  

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

![DeepinScreenshot_select-area_20190317200704.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190317200704.png)

maka akan menjadi tampilan yang bisa kira resize sesuai yang kita mau atau sesuai size dari smartphone.

5. silahkan rubah size tersebut hingga kurang dari 1264px, kenapa 1264px ? karena yang digunakan tadi adalah md yaitu lebar kurang dari 1264px. ketika dibawah dari 1264px maka button tersebut akan terhidden atau menghilang. seperti gambar dibawah ini :
![DeepinScreenshot_select-area_20190317201008.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190317201008.png)

penjelasan :
> karena kita menggunakan breapoint ``md`` dan visibility ``and-down`` maka dari nilai 1264px kebawah, button dilayar akan menghilang.  
sebaliknya jika menggunakan visibility ``and-up`` maka dari nilai 1264px kebawah akan tampil.  
jika menggunakan ``only`` hanya pada size yang dilalui 1264px sampai 960px yang disembunyikan.

### Overflow
Overflow berfungsi jika ada konten didalam elemen yang melebihi atau keluar dari element parent nya atau element yang membungkus konten tersebut. Format penulisan nya adalah :
```
     overflow-hidden - sembunyikan overflow pada sumbu x dan y
     overflow-y-hidden - sembunyikan overflow pada sumbu y
     overflow-x-hidden - sembunyikan overflow pada sumbu x
```

### Display
Display biasa nya berfungsi untuk mengatur posisi setiap element.

