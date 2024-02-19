# Tugas 1: Langkah-langkah Instalasi Sistem Operasi Debian

Instalasi sistem operasi Debian dapat dilakukan menggunakan berbagai aplikasi virtualisasi seperti VirtualBox, VMWare Player, atau Vmware Fusion (untuk MAC). Berikut adalah langkah-langkah instalasi Debian dengan menggunakan VirtualBox.

### Persyaratan Sistem:
- CPU: Minimal 2 core.
- RAM: Minimal 4096 MB (4 GB).
- HDD: Minimal 25 GB dengan partisi sebagai berikut:
  - / (root): 20 GB
  - /storage: 5 GB
  - swap: 1,5 GB
- Hostname: SysAdmin-NRP

### Langkah-langkah:

1. **Persiapan:**
   - Unduh file ISO Debian dari Repo resmi [DISINI](https://kartolo.sby.datautama.net.id/debian-cd/12.5.0/amd64/iso-cd/).
   - Unduh dan instal aplikasi VirtualBox dari web resmi [DISINI](https://www.virtualbox.org/wiki/Downloads).

2. **Membuat Mesin Virtual:**
   - Buka VirtualBox dan klik tombol "New" untuk membuat mesin virtual baru.
   - Beri nama mesin virtual SysAdmin-3122500024.
   - Atur tipe dan versi sistem operasi Debian sesuai dengan berkas ISO yang Anda unduh.
   - Atur alokasi RAM minimal 4096 MB.
   - Buat hard disk virtual baru dengan ukuran minimal 25 GB.
