![diagram](scr/ReverseProxy.png)  
### Penjelasan

##  Reverse Proxy dengan nama domain yang disesualikan nama diri sendiri
Mebuka web yang sudah dideploy.  
![diagram](scr/Foto-1-0.png)  

Buka Notepad sebagai Admin.  
![diagram](scr/Foto-1-1.png)  

buka file host di  
`Local Disk (C:) > Windows > System > drivers > etc`  
![diagram](scr/Foto-1-2.png)   

Menambahkan configurasi  
`192.168.0.123 abimsyaefulloh.xyz`  
![diagram](scr/Foto-1-2.png)  

Buka tab baru diterminal, lalu buka direktori  
`cd /etc/nginx/`  
dan buka direktori  
`cd sites-enabled`  
buat file configurasi baru di **sites-enabled**  
`sudo nano wayshub-frontend.conf`  
![diagram](scr/Foto-1-3.png)  

Buat codingan berikut, untuk membuat nama server dan lokasi portnyad, lalu simpan filenya.   
![diagram](scr/Foto-1-4.png)  

Jalankan `sudo nginx -t` untuk mengecek configurasi kita sudah benar atau belum.  
Jalankan `sudo systemctl reload nginx` untuk mereset atau mereload config baru.  
Jalankan `sudo sytemctl status nginx` untuk mengecek nginx nya berjalan atau tidak.  
Terakhir kita buka abimsyaefulloh.xyz dibrowser kita.  
![diagram](scr/Foto-1-5.png)  
terlihat webnya bisa diakses menggunakan configurasi yang sudah dibuat sebelumnya.
