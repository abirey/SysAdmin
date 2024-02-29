---
theme: uncover
_class: lead
paginate: true
backgroundColor: #fff
marp: true
transition: fade
---



# **Kelompok 1**

*System Administrator*

**3122500024** Muhamad Reza Muktasib
**3122500012** Awal Raya
**3122500011** Ali Azhar P.B

---

# Software Sources

Package yang ada pada sistem operasi kita (DEBIAN) didapatkan dari sumber link repository yang berada pada __/etc/apt/sources.list__

```markdown
# Cara Membuka dan Mengedit File SourceList

apt edit-sources

# Atau menggunakan text-editor nano

nano /etc/apt/sources.list
```

---
![alt text](image.png)
Beberapa istilah yang ada di dalam file ``sources.list``

| Istilah  | Deskripsi |
|----------:|:-------------|
|``deb``| wujud paket berupa biner |
|``deb-src``| wujud paket berupa source code|
|``http:..https:``| alamat internet dari server repo|
|``bookworm``| cabang struktur repository|
|``main non-free``| bagian dari repository|

---

> ### Kenapa `Bookworm` bukan `stable`
 Bookworm adalah versi debian sekarang, dan stable bermakna bahwa versi sekarang stabil. sehingga kita dapat membedakan versi dari kernel jika terdapat pembaruan. contoh ``Debian 13 Trixie`` rilis maka ``Bookworm`` menjadi ``oldstable`` dan sekarang berganti ke ``Trixie``.




---

#### Repository, Branches, Sections/Component

software package pada debian di letakan di dalam repository yang dimana dibagi menjadi ``2 bagian``, __cabang(_branch_)__ dan __komponen(_section_)__

---

# Cabang ( Branchs )

aktif: ``stable (stabil)``, ``testing (pengujian)`` dan ``unstable (tidak stabil)``.

|Jenis |Deskripsi|
|----|:-----|
|``stable``| Rilis distribusi resmi terbaru dari Debain.|
|``testing``| Berisi _package_ yang belum ada di stable, tapi dalam antrian untuk rilis stabil.|
|``unstable``| Merupakan versi dimana terjadi pengembangan aktif terhadap Debian.|

---

# Komponen ( Section )

| Komponen         | Keterangan                                          |
|:--------------------|:-----------------------------------------------------|
| ``main   ``            | Mematuhi __DFSG__ tanpa adanya ketergantungan "non-free" |
| ``non-free-firmware`` | Firmware non-free disertakan secara default sejak Debian 12 |
| ``contrib ``           | Mematuhi __DFSG__ dengan beberapa ketergantungan "non-free" |
| ``non-free``           | Tidak mematuhi __DFSG__                                   |

---

### Apa itu DFSG?

DFSG adalah panduan filosofis Debian untuk perangkat lunak bebas.
di main sendiri seluruhnya 100% gratis. sementara bagian contrib, non-free, dan non-free-firmware dapat mengandung software sebagian atau sepenuhnya non-free yang mungkin diperlukan untuk fungsi hardware tertentu (driver) contoh **NVIDIA**.

---

##### Backport Packages

<style>
    p, li {
        font-size: 30px;
    }
</style>
debian memberikan sebuah repo spesial bernama baacports yang dimana berisi lebih banyak versi dari aplikasi sebelumnya, repo ini secara default tidak aktif tetapi secara default regular repo yang menjadi prioritas tingggi

##### Apa itu Backport?

Backport adalah mekanisme yang memungkinkan aplikasi yang saat ini disimpan di repositori development Debian, untuk di-porting kembali ke versi “stabil”.


---
## Cara: memodifikasi repository


memodifikasi software sources dari sistem kita  ke dalam 	kontrib atau non free harus siap dengan beberapa dampak seperti 
kurangnya kebebasan untuk paket semacam ini
1. kurangnya dukungan dari proyek Debian (Anda tidak dapat memelihara perangkat lunak tanpa memiliki kode sumbernya)
kontaminasi sistem Debian Anda yang sepenuhnya gratis.
2. hal ini seperti membunuh pink rabbits
dilansir dari sourceforge Pink Rabbit Linux is a Linux Distribution which facilitates making your own Linux Distribution.

---

```markdown
# jalankan

apt edit-sources
```

Contoh Pengisian free packages

```deb http://deb.debian.ofg/debian/ bookwofm main```

Contoh Pengisian free packages dan tipe lain

```deb http://deb.debian.org/debian/ bookworm main contrib non-free non-free-firmware```


---

# APT (Advanced Package Tool) di Terimnal

User, Administrator

---

### Command apt untuk USER

|Command | Description |
|--------|:------------|
|``apt show foo``| Menampilkan informasi paket foo|
|``apt search foo``| Mencari paket bernama/berkaitan foo|
|``apt-cache policy foo``| Menampilkan versi tersedia paket foo|

---
### Command apt untuk ADMINISTRATOR
<style>
    table {
        font-size: 30px;
    }
</style>
__Pastikan__ menggunakan ``sudo`` untuk menjalankan perintah berikut (root)

|Command | Description |
|--------|:------------|
|``apt update``| Update repository metadata (list versi dll)|
|``apt install foo``| Memasang paket foo dan yang terkait|
|``apt upgrade``| Menghapus versi lama paket|
|``apt full-upgrade``| Mengupdate/hapus paket yang beneran terbaru|
|``apt remove foo``| menghapus paket foo, tidak confignya|
---

|Command | Description |
|--------|:------------|
|``apt autoremove``| auto menghapus paket tidak dibutuhkan|
|``apt purge foo``| Menghapus paket foo dengan confignya|
|``apt clean``| Menghapus cache lokal paket yang terinstall|
|``apt autoclean``| Menghapus cache lokal paket yang lama(tertinggal)|
|``apt-mark showmanual``| tandai paket sebagai "manual install"|

contoh all in one command
```apt update && apt full-upgrade && apt autoclean```

menghapus paket usang
```apt autoremove --purge```

---

##### Versi Mudah install Paket dengan Aplikasi _Software_

langkah Install: **Buka, Cari, Klik Tombol Install**

---
langkah Delete: **Klik Bagian Installed, Klik Uninstall, Confirm, Done**

---
langkah upgrade: **Bagian Update, Klik Download, Klik Restart and Update**

---
langkah modifikasi source repo: **Klik Hamburger menu di kanan atas, Klik Software Repositories, Konfigurasi, Klik Reload.**

---
##### Versi Mudah install Paket dengan Aplikasi _KDE_


---
##### Versi Mudah install Paket dengan Aplikasi _Synaptic_

---

# Membersihkan System
cara membersihkan ruang disk yang penuh
terdapat beberapa **Tool** yang dapat digunakan
sebelum itu mari kita gunakan terminal

```
df -h
```