# Apa itu Git?
Git adalah sebuah version control system,  
apa itu version control system adalah alat/software yang digunakan untuk:  
- Mencatat, mengatur, dan melacak setiap perubahan yang dibuat.  
- Kembali ke versi sebelumnya kalau terjadi error.  
- Kerja bareng tim tanpa file tabrakan.  

# Membuat repository "dumbways-batch-24" dan membuat 3 file berisi text. 
Buka menu repositories diGithub dan tekan tombol `NEW`  
![Repo](scr/Foto-1-0.png)  
Buat nama repository
`dumbways-batch-24`  
Pilih `Public` agar orang lain dapat melihat repository kita.  
Checklist bagian `Add a README file` untuk menambahkan file README.md secara otomatis.  
![Repo](scr/Foto-1-1.png)  
Tampilan awal kalau sudah jadi, lalu `+ Create new file` untuk membuat file baru.  
![Repo](scr/Foto-1-2.png)  
Isi nama file dan isi textnya.  
![Repo](scr/Foto-1-3.png)  
Membuat 3 file yang berisi text.  
![Repo](scr/Foto-1-4.png)  

# Manage repository tugas (devops24-dumbways-AbimSyaefulloh) menggunakan terminal  
Buka repository yang akan dimanage di terminal, lalu salin url nya.  
![Repo](scr/Foto-2-0.png)  
Buka terminal lalu jalankan command `git clone` dan paste url nya.  
![Repo](scr/Foto-2-1.png)  
Tapilan kalau berhasil dan periksa isi repositorynya.  
![Repo](scr/Foto-2-2.png)  
Di sini saya coba membuat file `fileAbim` dan mengisinya dengan text `Hallo Abim`  
![Repo](scr/Foto-2-3.png)  
Lalu Push ke Github kita.  
`git add fileAbim` = menambahkan fileAbim untuk diPush ke github.  
`git commit -m "NamaCommitNya"`= command untuk commitnya, untuk menyimpan catatan/pesan perubahan.  
`git remote set-url origin git@github.com:abimsyaefulloh/devops24-dumbways--AbimSyaefulloh-.git` =  
untuk mengelola alamat remote repository GitHub dari HTTPS (login username + token) menjadi SSH (gak butuh login).  
`git push origin main` = untuk push ke Github dan memilih branchenya di main  
![Repo](scr/Foto-2-4.png)  
Cek diGithub kita apakan sudah terupload.  
![Repo](scr/Foto-2-5.png)  

# Demonstrasi mencari perubahan text pada suatu file di GitHub
Membuka direktory yang sudah di clone sebelumnya,  
dan jalankan perintah `git pull origin master` untuk mengupdate isi direktory kita.
![Repo](scr/Foto-3-0.png)  
Edit text yang ada di file1.  
![Repo](scr/Foto-3-1.png)  
![Repo](scr/Foto-3-2.png)  
Cek perubahan menggunakan `git status`.  
![Repo](scr/Foto-3-3.png)  
Memasukkan file `file1` ke dalam staging area — yaitu persiapan sebelum di-commit ke dalam riwayat Git.
![Repo](scr/Foto-3-4.png)  
Menyimpan pesan tentang perubahan yang sudah ada di staging, dengan pesan commit "2nd commit".  
![Repo](scr/Foto-3-5.png)  
lalu git status lagi, untuk mengecek perubahan.  
![Repo](scr/Foto-3-6.png)  


