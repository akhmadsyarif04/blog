---
published: false
---
## Certainly Factor
           	
Certainly factor adalah diperkenalkan oleh Shortliffe Buchanan dalam pembuatan MYCIN. Pada tahun 1975 untuk mengakomadasi ketidakpastian pemikiran (inexact reasoning) seorang pakar. Teori ini dikembangkan bersamaan dengan pembuatan sistem pakar MYCIN. Team pengembang MYCIN mencatat bahwa dokter sering kali menganalisa informasi yang ada dengan ungkapan seperti misalnya : mungkin, kemungkinan besar, hampir pasti. Secara umum, rule direpresentasikan dalam bentuk sebagai berikut (John Durkin, 1994) :

> IF E1 [AND/OR] E2 [AND/OR] … En THEN H (CF = Cfi)

Dimana :  
    • E1 … En : fakta-fakta yang ada.  
    • H : hipotesa atau konklusi yang dihasilkan.  
    • CF : tingkat keyakinan (Certainty Factor) terjadinya hipotesa H akibat adanya fakta-fakta E1 s/d En  
    
Sebagai contoh, berikut ini adalah sebuah aturan dengan CF yang diberikan oleh seorang pakar :  
JIKA batuk, DAN demam, DAN sakit kepala, DAN bersin-bersin, MAKA influensa, CF : 0,7  

>	CF (H,E) = MB (H,E) – MD(H,E)

1. CF (H,E) :  Certaintty Factor dari hipotesis H yang dipengaruhi oleh gejala (evidence) E. Besarnya CF berkisaran antara -1 sampai 1. Nilai -1 menunjukan ketidakpercayaan mutlak sedangkan nilai 1 menunjukan kepercayaan mutlak.  
2. MB (H,E) : ukuran kenaikan kepercayaan (measure of increased belief) terhadap hipotesis H yang dipengaruhi oleh gejala E.  
3. MD (H,E) : ukuran kenaikan ketidakpercayaan (measure of increased disbelief) terhadap hipotesis H yang dipengaruhi oleh gejala E.  

Jika semua evidence diketahui dengan pasti maka persamaannya akan menjadi:  
> CF (E,e) = CF (H,E)

Dalam aplikasinya, CF (H,E) merupakan nilai kepastian yang diberikan oleh pakar terhadap suatu aturan, sedangkan CF(E,e) merupakan nilai kepercayaan yang diberikan oleh pengguna terhadap gejala yang dialaminya.  

Definisi menurut David McAllister Certainty Factor adalah suatu metode untuk membuktikan apakah suatu fakta itu pasti ataukah tidak pasti yang berbentuk metric yang biasanya digunakan dalam sistem pakar.