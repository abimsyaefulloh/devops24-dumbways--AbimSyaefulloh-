### 1. cat
Untuk menampilkan isi file teks dan menggabungkan beberapa file.  
Contohnya:
- Menampilkan isi file: fileMSG dan fileBrnRot  
  `cat fileMSG`
  `cat fileBrnRot`

- Menggabungkan file: fileMSG dan fileBrnRot kedalam file baru bernama fileGabungan  
  `cat fileMSG fileBrnRot > fileGabungan`
![text manipulation](scr/Foto-3-0.png)

## 2. echo
Perintah echo digunakan untuk mencetak teks dan menulis text ke file yang ada diterminal  
Contohnya:  
- Mencetak text  
`echo "hallo Uncle Roger"`  
`echo "Tung Tung Sahur"`  
- Menulis text ke file  
`echo "hallo Uncle Roger" > fileMSG`  
`echo "Tung Tung Sahur" > fileBrnRot`  
![text manipulation](scr/Foto-3-1.png)

## 3. grep
Mencari text dari file tertentu.  
Contohnya:  
- Mencari text **Uncle** difile **fileMSG**  
`grep Uncle fileMSG`  
- Mencari text **Uncle** di suatu direktori  
`grep Uncle *`  
- Mencari ada bebera text **Uncle** yang ada dalam satu direktori  
`grep -c Uncle *`  
![text manipulation](scr/Foto-3-2.png)

## 4. sed  
Digunakan untuk find & replace, hapus baris, atau manipulasi lainnya.  
Tapi sebagai contoh singkat saya hanya akan mempraktekan `-i` saja.  
Contohnya:  
- Mengganti kata **wasupp** menjadi **Hallo** di file1.  
`sed -i 's/wasupp/Hallo/g' file1`  
![text manipulation](scr/Foto-3-3.png)
