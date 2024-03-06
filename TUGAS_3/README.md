# FILE LAINNYA

[BACK](../README.md)

# TUGAS 3


## LINUX APT COMMAND 

### FOR USER

|Command | Description |
|--------|:------------|
|``apt show foo``| Menampilkan informasi paket foo|
|``apt search foo``| Mencari paket bernama/berkaitan foo|
|``apt-cache policy foo``| Menampilkan versi tersedia paket foo|


### Command apt untuk ADMINISTRATOR

__Pastikan__ menggunakan ``sudo`` untuk menjalankan perintah berikut (root)

|Command | Description |
|--------|:------------|
|``apt update``| Update repository metadata (list versi dll)|
|``apt install foo``| Memasang paket foo dan yang terkait|
|``apt upgrade``| Menghapus versi lama paket|
|``apt full-upgrade``| Mengupdate/hapus paket yang beneran terbaru|
|``apt remove foo``| menghapus paket foo, tidak confignya|



### HOW TO USE APT COMMAND

Mengubah Repository Apt (pastikan gunakan sudo)

![alt text](assets/1.png)

setelah melakukan update dan upgrade untuk depedency

Kita bisa install aplikasi menggunakan Aplikasi Software Bawaan
![alt text](image.png)


atau menggunakan KDE Installer, 

![alt text](image-1.png)
![alt text](image-2.png)

Informasi lengkap tentang Package Bisa diakses melalui link berikut :
[kde-full](https://wiki.debian.org/KDE#KDE.27s_software_in_Debian)



### Melihat Storage Yang terpakai di Linux Menggunakan TERMINAL

![ss1](assets/861_1.png)
### Membuat daftar Directory, diurutkan dari yang terbesar ke yang terkecil
Melihat isi direktori dengan perintah du dan sort (satuan megabyte):

![ss1](assets/861_2.png)
### NCurses Disk Usage (ncdu)
Untuk menganalisis ruang disk dalam mode konsol dengan menggunakan perintah ncdu.

![ss1](assets/861_3.png)
### baobab
Digunakan untuk menganalisa ruang pada disk dengan tampilan grafis.

![ss1](assets/861_4.png)
### Membersihkan Paket
#### Apt/aptitude/dpkg 
 Manajer paket Debian yang biasa digunakan. Saat menginstal sebuah paket, file sumber arsip/debnya disimpan di sistem pada folder /var/cache/apt/archives/ untuk memungkinkan kemungkinan instalasi ulang tanpa koneksi Internet. 
 
 Untuk membersihkan cache apt gunakan perintah apt clean.

Setelah cache dari paket yang diinstal dibersihkan, Kita juga dapat menghapus paket yang tidak berguna dari sistem, serta file konfigurasi. Peringatan! Ingatlah untuk memeriksa dengan cermat daftar paket yang direncanakan untuk dihapus, sebelum menerima operasi:

![ss1](assets/862_1.png)

Jika Anda telah mengupgrade sistem Anda, ada kemungkinan beberapa paket tidak lagi tersedia di repositori baru (paket tersebut sudah usang). Untuk membuat daftar dan menghapus paket-paket ini, gunakan apt dan periksa dengan cermat daftar paket yang direncanakan untuk dihapus:

![ss1](assets/862_2.png)
### 
Terakhir, untuk membuat daftar dan membersihkan file konfigurasi yang tetap ada meskipun aplikasi telah dihapus, gunakan perintah berikut :

![ss1](assets/862_4.png)
#### deborphan 
Mencantumkan paket-paket yang diadopsi pada sistem : paket-paket yang tidak bergantung pada paket lain. 

Ingatlah untuk memeriksa dengan cermat daftar paket yang direncanakan untuk dihapus, sebelum menjalankan operasi.

![ss1](assets/862_5.png)
### Mengosongkan trash-bin
Tiga trash-bin (wastebasket) yang berbeda harus dipertimbangkan:

#### trash-bin user
Anda dapat mengosongkannya dengan system file manager atau dengan perintah :

![ss1](assets/863.png)
#### trash-bin admin
Untuk mengosongkannya dengan cara yang benar, gunakan terminal dalam mode administrator:

![ss1](assets/864.png)
#### trash-bin eksternal
biasanya diberi nama '/media/(loginname)/your_disk/.Trash_1000'.

![ss1](assets/865.png)


## Menginstall Package EXTERNAL Extensi .deb

#### DEBI Application

Kita dapat menginstall package External (.deb) menggunakan aplikasi Gdebi yang dapat diinstall dengan cara berikut.

![alt text](assets/image-3.png)


