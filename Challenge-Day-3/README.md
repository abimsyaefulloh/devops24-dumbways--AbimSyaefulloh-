# Implementasikan load balancing kepada aplikasi wayshub. (Gunakan 2 server)  
Disini saya menggunakan 2 server yang sudah file wayshubnya di masing-masing server.  
- `server 1 (192.168.0.123)`  
- `server 2 (192.168.0.157)`  
![LoadBalancing](scr/Foto-1-0.png)

Tambahkan Penanda di Tiap Server, disini saya merename titlenya yaitu:  
- Server 1 `<title>WaysHub-svr123</title>`
- Server 2 `<title>WaysHub-svr157</title>`  
![LoadBalancing](scr/Foto-1-1.png)  

Konfigurasi Load Balancer Nginx hanya dilakukan di salah satu server, 
yaitu server yang berperan sebagai gateway atau host utama. Server ini akan menerima semua request dari client, 
lalu mendistribusikannya ke dua backend server menggunakan teknik load balancing.  
Disini saya menggunakan server 1 sebagai host dan membuat sebuah configurasi di:  
`/etc/nginx/sites-enabled/`  
![LoadBalancing](scr/Foto-1-2.png)  

Lalu menambahkan configurasi berikut.  
![LoadBalancing](scr/Foto-1-3.png)   

Setelah mengedit configurasinya selanjutnya.  
Jalankan `sudo nginx -t` untuk mengecek configurasi kita sudah benar atau belum.  
Jalankan `sudo systemctl reload nginx` untuk mereset atau mereload config baru.  
Jalankan `sudo sytemctl status nginx` untuk mengecek nginx nya berjalan atau tidak.  
![LoadBalancing](scr/Foto-1-4.png)   

Jalankan webnya di 2 server,  
`npm start`  
![LoadBalancing](scr/Foto-1-5.jpg)   
Refresh browser untuk menganti server.  
![LoadBalancing](scr/Foto-1-6.jpg)   
