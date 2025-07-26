# NodeJS  
Clone Repository terlebih dahulu, dengan tekan tombol `<> CODE`, lalu salin urlnya.  
![Repo](scr/Foto-1-0.png)  
Jalankan command git clone dan paste urlnya  
`git clone https://github.com/dumbwaysdev/wayshub-frontend.git`  
Lalu bisa dicek isi direktorinya.  
![Repo](scr/Foto-1-2.png)  
Nyalakan ufw port 3000 nya, untuk kita bisa menjalakannya di port 3000,  
`sudo ufw allow 3000`  
lalu cek statusnya  
`sudo ufw status`  
![Repo](scr/Foto-1-2.png)  
Periksa versi node kita, jika versinya terlalu tinggi, maka kita bisa menurunkan versi kebawahnya. 
Sesuai dengan tugasnya saya memakai node versi 12.  
![Repo](scr/Foto-1-3.png)  
Buka `cat package.json` untuk melihat informasi nama, dependensi, dll.  
![Repo](scr/Foto-1-4.png)  
Jalankan `npm install` untuk menginstal dependensi dan package-package yang dibutuhkan.  
![Repo](scr/Foto-1-5.png)  
Jalankan `npm start` untuk menjalankan webnya.  
![Repo](scr/Foto-1-6.png)  

# Python  
Nyalakan ufw port 5000 nya,  
`sudo ufw allow 5000`  
lalu cek statusnya    
`sudo ufw status`  
![Repo](scr/Foto-2-0.png)  
Cek versi python3 `python3 --version`  
![Repo](scr/Foto-2-1.png)  
Buat direktori python,  
`mkdir python`  
dan buat file pythonnya  
`nano appAbim.py`    
![Repo](scr/Foto-2-2.png)    
Isi filenya menggunakan codingan berikut, pastikan mengisi portnya di 5000.  
![Repo](scr/Foto-2-3.png)    
Jalankan app nya di web diport 5000 dengan command diterminal `python3 appAbim.py.`  
![Repo](scr/Foto-2-4.png)    

# Deploy app menampilkan text "Golang geming!"  
Download Golang terlebih dahulu.   
`link`  
![Golang](scr/Foto-3-0.png)   
Akses root terlebih dahulu, dan menjalankan tutorial golang yang ada diwebsitenya.  
copy dan jalankan scriptnya.  
![Golang](scr/Foto-3-1.png)   
Buat direketory baru bernama golang, dan buat file index.go, yang berisi text "Golang geming".  
![Golang](scr/Foto-3-2.png)   
berikut codingan untuk menampilkan text "Golang geming", yang berjalan di port 3000.    
![Golang](scr/Foto-3-3.png)   
jalankan diweb local 3000
![Golang](scr/Foto-3-4.png)   


