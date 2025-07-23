## Akses Server DiTerminal Tanpa Password

### 1. Generate Kunci dan Gembok

generate kunci dan gembok menggunakan  
`ssh-keygen`
![sshkeygen](scr/Foto-2-0.png)

### 2. Buka File Manager

Buka file `kunci.pub` menggunakan notepad
![kunci.pub di file manager](scr/Foto-2-1.png)

### 3. Tampilan di notepad

copy kuncinya yang berupa text tersebut
![tampilan di notepad](scr/Foto-2-2.png)

### 4. Copy kunci ke Server

Copy ke  
`/.ssh/authorized_keys`  
![copy ke server](scr/Foto-2-3.png)

### 5. Buka authorized_keys

Buka menggunakan command  
`nano authorized_keys`  
![nano](scr/Foto-2-4.png)

### 6. Akses Server diterminal tampa password

![powershell](scr/Foto-2-5.png)

### 7. Tampilan kalau sudah berhasil

![ ](scr/Foto-2-6.png)
