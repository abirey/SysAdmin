# DAFTAR TUGAS AKAN SAYA TAMPILKAN PADA BAGIAN INI
### [TUGAS 1](#tugas-1)
  #### _[FILE](https://github.com/Reza1290/SysAdmin-3122500024/main/TUGAS1.md)_


---

# TUGAS 1

**DAFTAR ISI**

- [SOAL 1](#langkah-langkah-instalasi-sistem-operasi-debian)
  - [Requirements](#persyaratan-sistem)
  - [Persiapan](#persiapan)
  - [Mulai](#langkah-langkah)



## Langkah-langkah Instalasi Sistem Operasi Debian

Instalasi sistem operasi Debian dapat dilakukan menggunakan berbagai aplikasi virtualisasi seperti VirtualBox, VMWare Player, atau Vmware Fusion (untuk MAC). Berikut adalah langkah-langkah instalasi Debian dengan menggunakan VirtualBox.


------------



### Persyaratan Sistem:
- CPU: Minimal 2 core.
- RAM: Minimal 4096 MB (4 GB).
- HDD: Minimal 25 GB dengan partisi sebagai berikut:
  - / (root): 20 GB
  - /storage: 5 GB
  - swap: 1,5 GB
- Hostname: SysAdmin-NRP


### Persiapan:
   - Unduh file ISO Debian dari Repo resmi [DISINI](https://kartolo.sby.datautama.net.id/debian-cd/12.5.0/amd64/iso-cd/).
   [TUTORIAL DOWNLOAD](#download)
   - Unduh dan instal aplikasi VirtualBox dari web resmi [DISINI](https://www.virtualbox.org/wiki/Downloads).
   [TUTORIAL INSTALL](#download)



### LANGKAH LANGKAH

1. **Membuat Virtual Machine**
   - Buka VirtualBox dan klik tombol "New" untuk membuat mesin virtual baru.
   - Beri nama mesin virtual SysAdmin-3122500024.
     
   ![CREATE](https://github.com/Reza1290/SysAdmin-3122500024/assets/70069286/411502a5-8282-4e85-ac03-59b31a322b0e)

   - **Pastikan Centang Kotak ** Supaya dapat melakukan Custom Install.
     
   - Atur alokasi RAM minimal 4096 MB. Disini saya alokasi 8GB
   - Atur alokasi core CPU minimal 2 Core, disini saya alokasi 6 Core dari 12 Core
     
   ![SPEK](https://github.com/Reza1290/SysAdmin-3122500024/assets/70069286/f8dcbcba-39e2-45af-9896-c70f6b26c257)
    
   - Buat hard disk virtual baru dengan ukuran minimal 25 GB.
     
   ![DISK SIZE](https://github.com/Reza1290/SysAdmin-3122500024/assets/70069286/5d2bd9a7-7e5b-41d2-bae9-7a65e0c05abc)



2. **Instalasi OS Debian**
   
Setelah kita melakukan setup pada bagian VM, selanjutnya Machine dapat kita jalankan dengan menekan tombol Start, setelah VM Menyala maka akan disuguhkan tampilan HOME dari Debian OS.

![HOME DEBIAN](https://github.com/Reza1290/SysAdmin-3122500024/assets/70069286/5933edad-5a74-458a-98f3-d38ad5ba25ca)


