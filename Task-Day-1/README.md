# Install Ubuntu Server  
Untuk menginstall Ubuntu Server kita harus menginstall Virtual Machine terlebih dahulu sebagai Virualisation, banyak opsi untul menginstal Virtual Machine, sebagai contoh:  
1.	VMware
2.	Virtual Box
3.	QEMU

## Step 1. Menginstal Virtual Machine dan Ubuntu Server  
Saya akan menggunakan VirtualBox sebagai Virtual Machine nya, saya mendownlad Virual Box versi 7.1..12 dengan OS yang saya gunakan Windows 11.
![Fotoscr](scr/Foto-0-0.jpg)
https://www.virtualbox.org/wiki/Downloads  
Dan menginstal Ubuntu Server, menggunakan versi Ubuntu 22.04.5 LTS (Jammy Jellyfish), dengan mendownload file “ubuntu-22.04.5-live-server-amd64.iso” saja  
![Fotoscr](scr/Foto-0-1.jpg)
https://releases.ubuntu.com/jammy/  
## Step 2. Membuat Virtual Machine di VirtualBox  
Berikut adalah tampilan awal dari VitualBox itu sendiri setelah kita Instal  
![Fotoscr](scr/Foto-1-0.png)
Tekan tombol “New” untuk membuat Virtual Machine baru, dan mengatur “bagian Name and Operating System”, yaitu membuat nama, tempat penyimpanan Filenya, dan memilih ISO Image berupa file Ubuntu yang sudah kita download sebelumnya, ceklis/centang bagian “Skip Unattended Installation” untuk mengatur secara langsung username, pasword dan opsi tambahan lainnya secara otomatis.   
![Fotoscr](scr/Foto-1-1.png)
Lalu atur bagian ”Hardware”, Saya akan menggunakan base memory sebesar 1 GB, dan 1 Core CPU.  
![Fotoscr](scr/Foto-1-2.png)
Mengatur Virtual Hard Disk, Saya menggunakan 10 GB penyimpanan Virtual.
Tekan Finish bila sudah selesai mengatur Virtual Machine secara keseluruhan.  
![Fotoscr](scr/Foto-1-3.png)
## Step 3. Menjalankan Virtual Machine  
Tekan Star untuk menjalankan Virtual Machine.  
![Fotoscr](scr/Foto-1-4.png)
Tekan “Try and Install Ubuntu Server.  
![Fotoscr](scr/Foto-2-0.png)
Pilih bahasa, saya menggunakan bahasa Inggris.  
![Fotoscr](scr/Foto-2-1.png)
Tekan “Continue without updating” karena saya memilih untuk tidak update.  
![Fotoscr](scr/Foto-2-2.png)
Memilih keyboard Layout, saya menggunakan Layout bahasa inggris  
![Fotoscr](scr/Foto-2-3.png)
Memilih base instalasi, ada beberapa pilihan seperti Ubuntu Server (minimized) yaitu pilihan untuk menjalakan ubuntu server secara seminimal mungkin dan ada opsi additional options, yaitu untuk menginstall beberapa driver dari third party yang lain. Tapi saya akan memilih untuk memakai Ubuntu Server saja.  
![Fotoscr](scr/Foto-2-4.png)
Menghubungkan Virtual Machine ke internet, sebelumnya bisa di cek IP Address device yang digunakan di Command Promt.  
![Fotoscr](scr/Foto-2-5.png)
Ketik “ipconfig” untuk mengetahui internet apa yang konek di device, bisa dicocokan di pengaturan windowsnya  
![Fotoscr](scr/Foto-4-0.png)
Ip saya adalah 192.168.0.100.  
![Fotoscr](scr/Foto-4-1.png)
Mengisi Network Configuration.  
`Subnet: 192.168.0.0/24`  
Artinya jaringan ini memiliki alamat awal 192.168.0.0 dan /24 menunjukkan bahwa 24 bit pertama digunakan sebagai network  
`Address: 192.168.0.123`  
Angka 123 menunjukkan alamat IP unik milik satu perangkat dalam jaringan 192.168.0.0/24. Angka ini bisa dari 1 sampai 254.  
`Gateway: 192.168.0.1`  
Angka .1 biasanya digunakan sebagai alamat router/gateway, yaitu perangkat yang menghubungkan jaringan lokal ke jaringan lain (misalnya internet).  
`Name server: 8.8.8.8, 8.8.4.4`  
angka 8.8.8.8 dan 8.8.4.4 itu menunjukan Server Google yang akan saya gunakan.  
![Fotoscr](scr/Foto-4-2.png)
Storage Configuration. Saya menggunakan Custom Storage.  
![Fotoscr](scr/Foto-4-3.png)
Dengan konfigurasi, 7 GB penyimpanan dan 2.8 GB penyimpanan cadangan.  
![Fotoscr](scr/Foto-4-4.png)
Membuat Profile dari nama, nama server, hingga username dan password.  
![Fotoscr](scr/Foto-4-5.png)
Saya memilih tidak menginstal configurasi apaapun hanya Ubuntu kosongan saja.  
![Fotoscr](scr/Foto-4-6.png)
Tunggu instalasinya hingga selesai.  
![Fotoscr](scr/Foto-4-7.png)
![Fotoscr](scr/Foto-4-8.png)
Login degan username dan password.  
![Fotoscr](scr/Foto-4-9.png)

