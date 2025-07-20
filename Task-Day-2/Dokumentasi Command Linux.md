## Command Linux

- `sudo` = Menjalankan perintah sebagai administrator (seperti Run as Admin di Windows)
- `sudo apt update` = Mengupdate daftar paket yang ada di repo
- `apt` = Buat install, update, atau hapus aplikasi di Ubuntu/Debian
- `mkdir` = Bikin folder baru
- `ls` = Lihat isi folder saat ini
- `ls -la` = Lihat semua isi folder, termasuk yang tersembunyi
- `cd` = Pindah folder
- `cd ..` = Naik 1 level folder
- `pwd` = Nunjukin path lokasi kita sekarang
- `touch` = Bikin file kosong
- `cp` = Copy file atau folder
- `mv` = Pindah atau rename file/folder
- `rm` = Hapus file
- `rm -r` = Hapus folder dan isinya
- `echo` = Nampilin teks
- `echo "teks" > file.txt` = Nulis teks ke file, isinya diganti total
- `echo "teks" >> file.txt` = Nyisipin teks ke akhir file
- `cat` = Baca isi file
- `nano` = Edit file lewat terminal
- `find` = Cari file atau folder
- `grep` = Cari teks di dalam file
- `chmod` = Ubah izin file
- `chown` = Ganti pemilik file
- `history` = Lihat riwayat command
- `clear` = Bersihin terminal
- `ip a` = Lihat IP address
- `systemctl` = Buat manage service di Linux
- `htop` = Lihat monitoring sistem (CPU, RAM, proses)
- `nmon` = Monitoring sistem lebih lengkap (CPU, RAM, network, dll)
- `lsof` = Lihat file apa aja yang lagi dibuka sistem
- `ufw` = Firewall bawaan Ubuntu yang gampang dipakai
- `poweroff` = Mematikan sistem
- `reboot` = Restart sistem

## Cara Akses Recovery Mode & Root
Kalau waktu boot kita tekan **Shift** atau **ESC** tapi GRUB gak muncul, kemungkinan GRUB-nya diset **hidden dan timeout 0**.
### Cara munculin GRUB:
1. Edit file grub config:
   ''sudo nano /etc/default/grub
