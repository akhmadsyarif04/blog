---
published: false
---
## Backward Chaining

Backward chaining adalah pelacakan kebelakang (atau kebalikan dari forward chaining) yang memulai penalarannya dari kesimpulan (goal), dengan mencari sekumpulan hipotesa-hipotesa menuju fakta-fakta yang mendukung sekumpulan hipotesa-hipotesa tersebut. Berikut gambaran proses penalaran metode backward chaining :  

Urutan langkah backward chaining :
1. Sistem akan melist dalam memori daftar konklusi yang ada.
2. Masing-masing konklusi secara sekuensial dicari premisnya.
3. Masing-masing premis di tanyakan ke user.
4. Jika jawaban ya, dilanjutkan ke premis berikutnya.
5, Jika jawabannya tidak dilanjutkan ke konklusi selanjutnya.

Metode backward chaining merupakan cara yang efisien untuk memecahkan masalah yang dimodelkan  sebagai masalah pemilihan struktur. Tujuannya mengambil pilihan terbaik dari banyak kemungkinan. Metode runut balik cocok diterapkan untuk memecahkan masalah diagnosis. Contoh :  

Lampu1 rusak,
If Lampu1 dinyalakan
And lampu1 tidak menyala
And lampu1 dihubungkan dengan sekring
And sekring masih bagus
