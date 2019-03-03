---
published: false
---
Pada kali ini saya pengen berbagi cara menggunakan xxd command pada terminal untuk convert hexadump atau sebaliknya.

Perintah **XXD** di linux memungkinkan kita untuk membuat hexadump atau sebalik. contoh syntax dasarnya adalah :
```html
xxd [OPTIONS] [file]
```

contoh convert teks menjadi hexadump.  
Buat 1 file txt dengan isi file tersebut seperti dibawah :

> We loved with a love that was more than love

simpan dengan nama test.txt.  
kemudian pada terminal ketikan seperti ini :

```html
xxd test.txt
```

hasil nya seperti dibawah ini :
![DeepinScreenshot_select-area_20190303230252.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190303230252.png)


### Cara memulai convert dari baris tertentu

contoh disini dimulai dari baris 2 dan seterus nya.  
dengan perintah :
```html
xxd -s 0x20 test.txt
```

hasil nya seperti dibawah ini :
![DeepinScreenshot_select-area_20190303230252.png]({{site.baseurl}}/_posts/DeepinScreenshot_select-area_20190303230252.png)
silahkan kalian bandingkan dengan yang pertama tadi.  

### Cara membatasi ouput 
```html
xxd -l 0x10 test.txt
```

### Cara megatur kolom ouput 
```html
xxd -c 4 test.txt
```

### Cara convert ke binary
```html
xxd -b test.txt
```

### Cara mengconvert dari hexadump ke String
```html
xxd -r -p test.txt
```