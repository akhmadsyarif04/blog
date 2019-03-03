---
published: true
---
Kalin ini saya akan membuat tutorial tentang clon dan push file-file html ke-Github yang sangat terkenal :D
saya anggap kalian sudah membuat repository jadi kita langsung ke bagian clone. buka terminal kalian, terus ketikan yang dibawah ini

```html
git clone https://github.com/username/namarepository
```

untuk https://github.com/username/namarepository sesuai kan dengan yang https seperti gambar dibawah ini

kalau sudah enter,
lanjut ketikan perintah dibawah ini

```html 
cd namarepositori
```

namarepositori kalian sesuai kan dengan nama repositori yang kalian bikin tadi.
kalau sudah masuk kedalam folder repositori kalian dihome, selanjutnya copas file yang ingin kalian masukan ke github kedalam folder tadi.
Selanjutnya ketikan perintah dibawah ini.

```html
git add --all
git commit -m "fush"
```

kalau terjadi error dengan pesan seperti ini

git config --global user.email "you@example.com"  
git config --global user.name "you name"

ketikan seperti ini.
```html
git config --global user.email "emailgithub kalian"
git config --global user.name "username github kalian"
```
kalau udah lanjut masukan perintah

```html
git commit -m "fush"
```

kalau tidak ada error lanjut

```html
git push origin master
```
nanti kalian akan diminta masukan username dan password github kalian.
kalau sudah selesai maka kita telah berhasil mempush atau memasukan file ke repositori github kalian.
selanjutnya silahkan cek repo kalian digithub kalian masing-masing.

semoga artikel ini membantu. kalau ada salah komen ya ^_^
