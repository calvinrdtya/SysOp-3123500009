<div align="center">
  <h1 style="text-align: center;font-weight: bold">Praktikum 1<br>Sistem Operasi</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br />
<div align="center">
  <img src="img/logo pens.png" alt="Logo PENS">
  <h3 style="text-align: center;">Disusun Oleh :</h3>
  <p style="text-align: center;">
    <strong>Calvin Raditya Sandy Winarto (3123500009)</strong><br>
    <strong>Zada Devi Mariama (3123500015)</strong>
  </p>

<h3 style="text-align: center;line-height: 1.5">Politeknik Elektronika Negeri Surabaya<br>Departemen Teknik Informatika Dan Komputer<br>Program Studi Teknik Informatika<br>2024/2025</h3>
  <hr>
</div>
<br>

# Daftar Isi

- [Daftar Isi](#daftar-isi)
- [Apa itu Sistem Operasi?](#apa-itu-sistem-operasi)
- [Proses Booting](#proses-booting)
  - [Langkah-Langkah Booting](#langkah-langkah-booting)
- [Soal](#soal)
- [Instalasi](#instalasi)
  - [Proses Instalasi Virtual Box](#proses-instalasi-virtual-box)
- [Instalasi Debian](#instalasi-debian)
- [Referensi](#referensi)
# Apa itu Sistem Operasi?
  **Sistem operasi (OS)** adalah program yang, setelah pertama kali dimuat ke komputer melalui program boot, mengelola semua program aplikasi lain di komputer. Program aplikasi memanfaatkan sistem operasi dengan membuat permintaan layanan melalui antarmuka program aplikasi yang ditentukan ( API ). Selain itu, pengguna dapat berinteraksi langsung dengan sistem operasi melalui antarmuka pengguna, seperti antarmuka baris perintah (CLI) atau UI grafis (GUI).
<br><br>

# Proses Booting
Apa itu Booting?
Booting adalah proses awal ketika komputer atau perangkat lainnya dinyalakan atau di-restart. Proses booting bertujuan untuk memuat sistem operasi dan perangkat lunak lainnya ke dalam memori sehingga komputer dapat berfungsi secara normal.

## Langkah-Langkah Booting
1) **Power On**
    - Saat tombol daya ditekan atau sumber daya lainnya diaktifkan, listrik mengalir ke komponen-komponen perangkat keras komputer.
2) **POST (Power-On Self-Test)**
    - Setelah tombol power ditekan, laptop melakukan POST (Power-On Self-Test).
    - POST adalah proses pemeriksaan awal perangkat keras seperti RAM, prosesor, dan perangkat penyimpanan untuk memastikan bahwa semuanya berfungsi dengan baik.
3) **BIOS/UEFI**
    - Jika POST berhasil, laptop memuat BIOS (Basic Input/Output System) atau UEFI (Unified Extensible Firmware Interface).
    BIOS/UEFI menyediakan antarmuka perangkat keras dan menentukan perangkat penyimpanan yang akan di-boot
4) **Inisialisasi Perangkat Keras**
    - Komputer akan menginisialisasi perangkat keras seperti hard drive,     keyboard, mouse, dan perangkat lainnya. Proses ini melibatkan tahap mengenali perangkat keras, memuat driver yang diperlukan, dan menyiapkan perangkat untuk digunakan.
5) **Pemilihan Perangkat Boot**
    - Di dalam BIOS/UEFI, laptop mencari perangkat penyimpanan yang diatur  sebagai perangkat boot. Perangkat boot biasanya adalah hard disk internal atau SSD, tetapi dapat diatur untuk boot dari perangkat lain seperti USB atau CD/DVD jika diperlukan.
6) **Boot Loader**
    - Setelah perangkat boot dipilih, boot loader (misalnya, GRUB untuk Linux atau bootloader Windows) dimuat ke dalam memori. Boot loader bertanggung jawab untuk memuat sistem operasi yang sebenarnya.
7) **Sistem Operasi**
    - Boot loader memuat sistem operasi yang telah diinstal pada perangkat penyimpanan.
    Sistem operasi kemudian dimuat ke dalam memori RAM dan proses booting berlanjut.
8) **Login**
    - Setelah proses booting selesai, sistem operasi menampilkan layar login. Pengguna dapat memasukkan informasi login seperti username dan password.
9) **Desktop/Interface Pengguna**
    - Setelah login berhasil, sistem operasi memuat desktop atau antarmuka pengguna.
<br><br>

# Soal
1. Buatlah tulisan tentang langkah-langkah instalasi sistem operasi Debian. Anda bisa menggunakan aplikasi virtualisasi seperti VirtualBox, VMWare Player, Vmware Fusion (MAC), dls. Kebutuhan sistem adalah sebagai berikut :
    - CPU : 2 core
    - RAM : 4096 (min)
    - HDD : 25GB dengan partisi :
        - / : 20 GB
        - /storage : 5 GB
        - swap : 1,5 GB
    - Hostname : SysAdmin-NRP
<br><br>

# Instalasi
  ## Proses Instalasi Virtual Box

1) Buka situs resmi **VirtualBox** di https://www.virtualbox.org/
[![img-1](img/1.png)]()

2) Pilih versi **VirtualBox** yang sesuai dengan Sistem Operasi anda, lalu pilih **Donwloads**.
[![img-1](img/2.png)]()

3) Buka file installer yang telah diunduh.
[![img-1](img/3.png)]()

4) Pilih Next pada pop up **VirtualBox**
[![img-1](img/4.png)]()

5) Selanjutnya, pilih Install
[![img-1](img/5.png)]()

6) Tunggu hingga proses instalasi selesai
[![img-1](img/6.png)]()

7) Klik finish, maka anda sudah berhasil menginstall VirtualBox 
[![img-1](img/7.png)]()


# Instalasi Debian
1) Buka aplikasi **Oracle VM VirtualBox Manager**, kemudian pilih **New**.
[![img-1](img/8.png)]()
[![img-1](img/new.png)]()

2) Sesuaikan **Name dan Folder**. Pada bagian Iso Image, pilih **file ISO Debian** yang sudah di download. Click pada bagian **Skip Unattended Installation** dan Next.
[![img-1](img/9.jpeg)]()

3) Pada bagian Hardware, setting Base Memory minimal sebesar **4096 MB** dan Processor minimal sebesar **2 Core**. Kemudian pilih Next.
[![img-1](img/10.png)]()

4) Bagian Virtual Hard Disk setting Disk Size sebesar **26,5** GB yang nantinya akan dibagi menjadi 3 partisi, kemudian! Next.
[![img-1](img/11.jpeg)]()

5) Akan muncul tampilan untuk mengedit **username, hostname serta password**, setelah itu click Next.
[![img-1](img/12.jpeg)]()

6) Setelah selesai, pada bagian Summary click tombol Finish.
[![img-1](img/13.png)]()

7) Pilih **Debian** dan click Start untuk memulai.
[![img-1](img/14.png)]()

8) Pilih bahasa yang nantinya ingin anda gunakan, kemudian click Continue.
[![img-1](img/15.png)]()

9) Pilih Lokasi anda, kemudian click Continue.
[![img-1](img/16.png)]()
[![img-1](img/17.png)]()
[![img-1](img/18.png)]()

10) Pilih sesuai default bahasa anda, Lalu click Continue.
[![img-1](img/19.png)]()

11) Konfigurasi keyboard yang ingin anda gunakan, click Continue dan tunggu hingga selesai.
[![img-1](img/20.png)]()

12) Tunggu hingga proses selesai.
[![img-1](img/21.png)]()

13) Pada bagian Konfigurasi Network masukkan **Hostname** anda dan kosongkan untuk bagian Domain Name, kemudian click Continue.
[![img-1](img/22.png)]()

14) Pada Bagian Set Up users and password sesuaikan Password, Fullname dan Username anda, kemudian click Continue.
  [![img-1](img/23.png)]()
  [![img-1](img/24.png)]()

15) Pada bagain Configure the clock sesuaikan waktu yang ada di lokasi anda, kemudian click Continue dan tunggu hingga selesai.
[![img-1](img/25.png)]()

16) Pilih manual untuk setting partisi, kemudian pilih **SCSI3 (0,0,0) (sda) - 28.5 GB ATA VBOX HARDDISK**. Pada bagian Create new empty partition table on this device pilih Yes.
[![img-1](img/26.png)]()
[![img-1](img/27.png)]()

17)  Setelah itu, pilih free space yang tersedia.
[![img-1](img/28.png)]()

18) Kemudian click **Create a new partition**.
[![img-1](img/29.png)]()

18) Untuk Partition Size masukkan sebesar 20 GB dengan type **Primary**. location partition pilih **Beginning**
[![img-1](img/30.png)]()
[![img-1](img/31.png)]()
[![img-1](img/32.png)]()

19) Pastikan Bootable flag dalam keaadan On, kemudian pilih **Done setting up the partition**. Setelah selesai, ulangi step sebelumnya untuk setting **partisi /storage sebesar 5 GB dan swap sebesar 1,5 GB**.
[![img-1](img/33.png)]()
[![img-1](img/34.png)]()
[![img-1](img/35.png)]()

20) Setelah halaman **VirtualBox** terbuka, pilih new
[![img-1](img/36.png)]()

21) Setelah halaman VirtualBox terbuka, pilih new
[![img-1](img/37.png)]()

22) Setelah selesai, pilih **Finish partitioning and write changes to disk** dan tunggu hingga selesai.
[![img-1](img/56.png)]()

23) Pada pilihan **Write the changes to disk?** pilih **Yes** lalu **Continue**
[![img-1](img/45.png)]()

24) Untuk **Configure the package manager** pada bagian Scan extra installation media pilih **No**.
[![img-1](img/46.png)]()

25) Selanjutnya untuk Debian archive mirror country pilih **Indonesia** dan Debian archive mirror pilih **kebo.pens.ac.id**.
[![img-1](img/47.png)]()
[![img-1](img/48.png)]()

26) Biarkan kosong untuk bagian HTTP proxy information dan tunggu hingga selesai.
[![img-1](img/49.png)]()
[![img-1](img/50.png)]()

27) Pada bagian **Participate in the package usage survey?** pilih **No**, lalu click Continue. Tunggu hingga selesai.
[![img-1](img/51.png)]()
[![img-1](img/53.png)]()

28) Untuk Software selection pilih **Debian desktop environment**, **GNOM** dan **Standart system utilities**, kemudian tunggu hingga selesai.
[![img-1](img/54.png)]()
[![img-1](img/55.png)]()

29) Pada bagian **Install the GRUB boot loader** untuk Install the GRUB boot loader pilih Yes dan Device for boot loader pilih **/dev/sda (ata-VBOX_HARDDISK_VBf5fb021a-7667d996)**. Click Continue dan tunggu hingga selesai.
[![img-1](img/new/51.png)]()
[![img-1](img/new/52.png)]()

30) Setelah selesai, click Continue dan sistem akan Rebooting.
[![img-1](img/new/53.png)]()

31) Setelah semuanya selesai maka akan ke halaman login **Debian**.
[![img-1](img/new/54.jpeg)]()
[![img-1](img/new/55.jpeg)]()
<br><br>

# Referensi
- https://www-techtarget-com.translate.goog/whatis/definition/operating-system-OS?_x_tr_sl=en&_x_tr_tl=id&_x_tr_hl=id&_x_tr_pto=tc
- https://www.gramedia.com/literasi/pengertian-sistem-operasi/
- https://telkomuniversity.ac.id/pengertian-data-fungsi-jenis-jenis-manfaat-dan-contohnya/
- https://bsi.today/sistem-operasi/

[def]: #langkah-langkah-booting