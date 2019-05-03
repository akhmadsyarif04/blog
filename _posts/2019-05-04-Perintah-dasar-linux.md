---
published: false
---
## Perintah Dasar Linux atau Terminal

###Files dan Navigating

| Command | Ket |   
| ------------- |:-------------|
| ls| list directory (semua file/folder)|
| ls -l| list directory dalam format list |
| ls -la| list directory beserta hidden file dalam format list |
| cd dir| ganti directory ke directory lain |
| cd _| ganti ke directory utama |
| cd| ganti directory ke home directory |
| pwd| menampilkan directory saat ini |
| mkdir dir| membuat directory |
| rm -f dir| delete file |
| rm -r dir| delete directory |
| rm -rf dir| delete directory |
| rm -rf / | menghapus semua dengan target system utama |
| cp file1 file2| copy file1 ke file2 |
| mv file1 file2| rename file1 menjadi file2 |
| mv file1 /dir/file2| memindah file1 ke directory dengan nama file2 |
| touch file| membuat file |
| cat file| menampilkan isi file |
| cat > file  | memasukan teks kedalam file  |
| cat >> file | menambahkan teks ke dalam file  |
| tail -f file  | menampilkan isi file  |

###Networking

| Command | Ket |   
| ------------- |:-------------|
|ping host | ping host|
| whois domain  | mendapatkan whois domain  |
| dig domain  | mendapatkan DNS domain  |
| dig -x domain  | reserve lookup host  |
| wget file  | download file  |
| wget -e file  | melanjutkan download yang berhenti  |
| wget -r url  | unduh file secara rekursif dari url  |
| curl url  | tampilkan halaman web dari url  |
| curl -o meh.html url  | menulis halaman ke meh.html  |
| ssh user@host  | konek ke ssh  |
| ssh -p port user@host  | konek ke ssh dengan port  |
| ssh -D user@host  | konek dan menggunakan port bind  |


###Processes

| Command | Ket |   
| ------------- |:-------------|
| ps | menampilkan proses yang aktif |
| ps aux   | menampilkan secara detail  |
| kill pid  | mematikan proses dengan id prosess  |
| killall proc  | mematikan semua proses dengan nama proc  |


###System Info

| Command | Ket |   
| ------------- |:-------------|
| date | menampilkan tanggal dan waktu |
| uptime  |  menampilkan waktu |
| whoami  | sedang login menggunakan apa/akses siapa yang digunakan  |
| w  | menampilkan siapa yang online  |
| cat /proc/cpuinfo  | menampilkan cpu info  |
| cat /proc/meminfo  | menampilkan memory info  |
| free  | menampilkan memory dan swap yang digunakan  |
| du   | menampilkan penggunaan tempat pada directory  |
| du -sh  | menampilkan dalam format GB  |
| df  | menampilkan disk yang digunakan  |
| uname -a  | menampilkan kernel config  |

###Compressing

| Command | Ket |   
| ------------- |:-------------|
| tar cf file.tar files | memasukan file kedalam file.tar |
| tar xf file.tar | extract  |
| tar tf file.tar  | menampilkan isi dari tar  |

###Permissions

| Command | Ket |   
| ------------- |:-------------|
|  chmod octal file | untuk mengubah Permissions dari sebuah file    |
| chmod -R octal folder  | untuk mengubah Permissions semua file yang ada difolder  |

> octal :  
1 = execute (x)  
2 = write (w)  
4 = read ( r )   

contoh : sudo chmod 752 file
> ket :   
7 artinya execute,write,read untuk owner  
5 artinya execute,read untuk group  
2 artinya write untuk world  
