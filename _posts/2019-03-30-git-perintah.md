---
published: false
---
## Perintah - Perintah git yang sering digunakan

``git init``
untuk membuat folder .git pada folder

``git add`` 
menambahkan data tapi tidak disave kerepo

``git commit -m ""`` 
untuk save perubahan pada git local

``git log`` 
melihat log yang telah dilakukan

``git diff`` 
untuk melihat perubahan
> ketika sudah di __git add__ maka tidak tampil hasil __git diff__
        
``git checkout namafile``  
atau  
``git checkout kodelog -- namafile``  
mengembalikan file yang dirubah

``git reset --soft kodelog``  
``git reset --mixed kodelog``
``git reset --hard kodelog``



git branch # untuk melihat branch yang ada
git branch branch_baru # membuat branch baru 
git checkout -b branch_baru # membuat branch baru dan pindah ke yang baru
git checkout nama_branch # pindah branch

{jika ingin menghapus branch baru maka tidak boleh berada dibranch itu}
git branch -D nama_branch # mengahapus branch

git branch -m nama_branch_lama nama_branch_baru # mengubah nama branch

git merge nama_branch # menggabungkan perubaha branch

{ 
    jika terjadi konflik antar branch setelah dimerge
    maka automatis git akan memberitahu kesalahan pada atom.
    edit manual, setelah diedit maka commit lagi. maka konflik selesai dan perubahaan 
    commit sebelum nya pada branch lain ditambahkan pada branch yang menyelesaikan
    konflik tapi dibranch lain commit masih tetap seperti yang terakhir.
}
