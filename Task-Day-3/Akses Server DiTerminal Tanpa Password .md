## Akses Server DiTerminal Tanpa Password.

### 1. Generate Kunci dan Gembok.

Generate kunci dan gembok menggunakan.  
`ssh-keygen`  
Lalu pilih lokasi penyimpanan.  
![sshkeygen](scr/Foto-2-0.png)

### 2. Buka File Manager.  
Buka lokasi penyimpanan kuncinya lalu,  
buka file `kunci.pub` menggunakan notepad.
![kunci.pub di file manager](scr/Foto-2-1.png)

### 3. Tampilan di notepad.

Copy kuncinya yang berupa text tersebut. 
![tampilan di notepad](scr/Foto-2-2.png)

### 4. Copy kunci ke Server.
Buka direktori dibawah ini terlebih dahulu.   
`/.ssh/authorized_keys`  
![copy ke server](scr/Foto-2-3.png)

### 5. Buka authorized_keys dan Paste kuncinya.  

Buka menggunakan command.  
`nano authorized_keys`  
Lalu paste kuncinya.
![nano](scr/Foto-2-4.png)

### 6. Akses Server diterminal tanpa password.  
`ssh -i .ssh\kunci username@ip-address`  
![powershell](scr/Foto-2-5.png)

### 7. Tampilan kalau sudah berhasil.

![ ](scr/Foto-2-6.png)
