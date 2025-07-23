# Diagram Jaringan Komputer
![diagram](scr/Diagram-Jaringan-Komputer-.png)

# Daftar Command Linux 

## Perintah Dasar

- sudo = Menjalankan perintah sebagai administrator/root (seperti Run as Administrator di Windows)
- sudo apt update = Mengupdate daftar paket dari repository agar sistem tahu versi terbaru
- apt = Package manager bawaan Debian/Ubuntu untuk mengelola aplikasi (install, remove, update)
- mkdir = Membuat folder atau direktori baru
- ls = Melihat daftar file dan folder dalam direktori saat ini
- ls -la = Melihat semua file termasuk yang tersembunyi (.), dengan detail lengkap
- cp = Meng-copy/menduplikasi file atau folder
- mv = Memindahkan file/folder atau mengganti namanya
- rm = Menghapus file
- rm -r = Menghapus folder beserta isinya (recursive)
- pwd = Menampilkan path lengkap direktori saat ini
- cd = Berpindah ke direktori lain
- cd .. = Kembali ke direktori satu tingkat di atas
- touch = Membuat file kosong baru
- echo = Menampilkan teks ke terminal
- echo "teks" > file.txt = Menulis dan mengganti seluruh isi file dengan teks baru
- echo "teks" >> file.txt = Menyisipkan teks ke akhir file tanpa menghapus isinya
- cat = Menampilkan isi file di terminal
- nano = Membuka file dengan text editor sederhana di terminal
- find = Mencari file atau folder dari direktori tertentu
- find -type f -"nama file" = Mencari file dengan nama spesifik
- grep = Mencari teks di dalam file
- chmod = Mengubah permission (izin akses) sebuah file atau folder
- chown = Mengubah kepemilikan (owner) file atau folder ke user/grup lain
- history = Menampilkan daftar perintah yang pernah dijalankan di terminal
- clear = Membersihkan layar terminal
- ip a = untuk mengetahui IP Address kita
- systemctl = system control untuk mengatur beberapa aplikasi yang berjalan diserver 
- htop = Monitoring sistem yang penggunaan CPU, RAM, Swap, dan Task yang sedang bejalan
- nmon = Monitoring sistem tingkat lanjut untuk CPU, RAM, disk I/O, network, filesystem, dan lainnya dalam satu tampilan 
- lsof = Menampilkan daftar file yang sedang dibuka atau diproses dan kita bisa mencari secara spesific file yang sedang diproses ada dimana
- ufw = Uncomplicated Firewall (firewall yang gak ribet) digunakan untuk mengatur izin keluar/masuk koneksi jaringan (port, IP, protokol) ke server
- poweroff = untuk mematikan server
- reboot = untuk merestar server

## Command untuk akses recovery mode dan akses root

- Tekan Shift atau ESC pada saat porses booting Ubuntu server
- Jika tekan Shift atau ESC pun gak ngaruh, itu karena GRUB-nya langsung dilewati (hidden dan timeout-nya 0). 
  Cara agar mengedit konfigurasinya, dan cara akes GRUB (GRand Unified Bootloader)/(sebuah bootloader sistem operasi):

1. Buka terminal seperti biasa, lalu jalankan perintah berikut:  
   sudo nano /etc/default/grub

2. Ubah baris:  
   GRUB_TIMEOUT=0  
   GRUB_TIMEOUT_STYLE=hidden

3. Menjadi:  
   GRUB_TIMEOUT=10  
   GRUB_TIMEOUT_STYLE=menu

4. Lalu simpan:  
   sudo update-grub

5. Dan restart sistem:  
   sudo reboot

6. Saat booting ulang, tekan Shift (BIOS) atau ESC (UEFI) untuk membuka GRUB menu.

7. Pilih menu:  
   Advanced options for Ubuntu

8. Lalu pilih yang ada tulisan:  
   Ubuntu, with Linux "versi yang digunakan" - (recovery mode)

9. Pilih opsi root.
    
10. Dan kita sudah mengakses terminal sebagai root.

# Perbedaan antara SH (Shell) dan BASH (Bourne-Again SHell)
### SH (Shell)
**SH (Shell)** adalah shell standar Unix yang pertama kali digunakan, juga dikenal sebagai *Bourne Shell*. Nama programnya biasanya `sh`, dan dirancang untuk menjalankan perintah serta skrip secara sederhana. Shell ini bersifat ringan dan minim fitur, sehingga cocok untuk skrip dasar dan digunakan demi kompatibilitas antar sistem Unix.

### BASH (Bourne-Again SHell)
**BASH (Bourne-Again SHell)** adalah pengembangan dari SH yang dibuat oleh GNU dan menjadi shell default di banyak distro Linux seperti Ubuntu. Nama programnya biasanya `bash`, dan menawarkan fitur-fitur modern seperti autocomplete dengan TAB, riwayat perintah (history), penggunaan array, serta ekspresi logika `[[ ... ]]` yang lebih fleksibel. Dengan kemampuan scripting yang lebih lengkap, BASH menjadi pilihan utama untuk pengguna dan pengembang Linux saat ini.

## INTINYA
- **Shell (SH)** adalah bahasa skrip awal di Unix, sedangkan **BASH** adalah versi modern dan lebih lengkap yang jadi standar di Linux.
- **Unix** adalah sistem operasi asli, tertutup (komersial)
- **Linux** adalh operasi **open source** yang dibuat mirip **Unix (disebut: Unix-like system)**, tapi dibuat dari nol







