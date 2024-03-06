<div align="center">
  <h1 style="text-align: center;font-weight: bold">Praktikum 1<br>Sistem Operasi</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br />
<div align="center">
  <img src="../assets/week-1/logo_pens.png" alt="Logo PENS">
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
    [![img-1](/assets/week-1/Booting/1.jpeg)](img)
2) **POST (Power-On Self-Test)**
    - Setelah tombol power ditekan, laptop melakukan POST (Power-On Self-Test).POST adalah proses pemeriksaan awal perangkat keras seperti RAM, prosesor, dan perangkat penyimpanan untuk memastikan bahwa semuanya berfungsi dengan baik.
    [![img-1](/assets/week-1/Booting/2.png)](img)
3) **Inisialisasi Perangkat Keras**
    - Inisialisasi perangkat keras Setelah POST selesai, komputer akan menginisialisasi perangkat keras seperti hard drive, keyboard, mouse, dan perangkat lainnya. Proses ini melibatkan tahap mengenali perangkat keras, memuat driver yang diperlukan, dan menyiapkan perangkat untuk digunakan.
    [![img-1](/assets/week-1/Booting/3.jpeg)](img)
4) **Boot Loader**
    - Setelah inisialisasi perangkat keras selesai, BIOS atau UEFI mencari boot loader di media penyimpanan yang telah ditentukan, biasanya hard drive atau SSD. Jika ada beberapa sistem operasi yang terinstal, pemuat boot, seperti GRUB (Grand Unified Bootloader) untuk sistem Linux, memungkinkan pengguna untuk memilih sistem operasi mana yang akan dimuat. Selanjutnya, loader boot memuat kernel sistem operasi yang dipilih ke dalam memori.
    [![img-1](/assets/week-1/Booting/4.png)](img)
5) **Memuat Sistem Operasi**
    - Boot loader memuat sistem operasi yang telah diinstal pada perangkat penyimpanan.
    Sistem operasi kemudian dimuat ke dalam memori RAM dan proses booting berlanjut.
    [![img-1](/assets/week-1/Booting/5.jpg)](img)
6) **Login**
    - Setelah proses booting selesai, sistem operasi menampilkan layar login. Pengguna dapat memasukkan informasi login seperti username dan password.
    [![img-1](/assets/week-1/Booting/6.jpg)](img)
7)  **Desktop/Interface Pengguna**
    - Setelah login berhasil, sistem operasi memuat desktop atau antarmuka pengguna.
    [![img-1](/assets/week-1/Booting/7.png)](img)
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

1) Buka situs resmi **VirtualBox** di <https://www.virtualbox.org/>
[![img-1](/assets/week-1/1.png)](img)

1) Pilih versi **VirtualBox** yang sesuai dengan Sistem Operasi anda, lalu pilih **Donwloads**.
[![img-1](/assets/week-1/1.png)](img)

1) Buka file installer yang telah diunduh.
[![img-1](/assets/week-1/3.png)](img)

1) Pilih Next pada pop up **VirtualBox**
[![img-1](/assets/week-1/4.png)](img)

1) Selanjutnya, pilih Install
[![img-1](/assets/week-1/5.png)](img)

1) Tunggu hingga proses instalasi selesai
[![img-1](/assets/week-1/6.png)](img)

1) Klik finish, maka anda sudah berhasil menginstall VirtualBox
[![img-1](/assets/week-1/7.png)](img)

# Instalasi Debian

1) Buka aplikasi **Oracle VM VirtualBox Manager**, kemudian pilih **New**.
[![img-1](/assets/week-1/8.png)](img)
[![img-1](/assets/week-1/new.png)](img)

2) Sesuaikan **Name dan Folder**. Pada bagian Iso Image, pilih **file ISO Debian** yang sudah di download. Click pada bagian **Skip Unattended Installation** dan Next.
[![img-1](/assets/week-1/9.jpeg)](img)

3) Pada bagian Hardware, setting Base Memory minimal sebesar **4096 MB** dan Processor minimal sebesar **2 Core**. Kemudian pilih Next.
[![img-1](/assets/week-1/10.png)](img)

4) Bagian Virtual Hard Disk setting Disk Size sebesar **26,5** GB yang nantinya akan dibagi menjadi 3 partisi, kemudian! Next.
[![img-1](/assets/week-1/11.jpeg)](img)

5) Akan muncul tampilan untuk mengedit **username, hostname serta password**, setelah itu click Next.
[![img-1](/assets/week-1/12.jpeg)](img)

6) Setelah selesai, pada bagian Summary click tombol Finish.
[![img-1](/assets/week-1/13.png)](img)

7) Pilih **Debian** dan click Start untuk memulai.
[![img-1](/assets/week-1/14.png)](img)

8) Pilih bahasa yang nantinya ingin anda gunakan, kemudian click Continue.
[![img-1](/assets/week-1/15.png)](img)

9) Pilih Lokasi anda, kemudian click Continue.
[![img-1](/assets/week-1/16.png)](img)
[![img-1](/assets/week-1/17.png)](img)
[![img-1](/assets/week-1/18.png)](img)

10) Pilih sesuai default bahasa anda, Lalu click Continue.
[![img-1](/assets/week-1/19.png)](img)

11) Konfigurasi keyboard yang ingin anda gunakan, click Continue dan tunggu hingga selesai.
[![img-1](/assets/week-1/20.png)](img)

12) Tunggu hingga proses selesai.
[![img-1](/assets/week-1/21.png)](img)

13) Pada bagian Konfigurasi Network masukkan **Hostname** anda dan kosongkan untuk bagian Domain Name, kemudian click Continue.
[![img-1](/assets/week-1/22.png)](img)

14) Pada Bagian Set Up users and password sesuaikan Password, Fullname dan Username anda, kemudian click Continue.
  [![img-1](/assets/week-1/23.png)](img)
  [![img-1](/assets/week-1/24.png)](img)

15) Pada bagain Configure the clock sesuaikan waktu yang ada di lokasi anda, kemudian click Continue dan tunggu hingga selesai.
[![img-1](/assets/week-1/25.png)](img)

16) Pilih manual untuk setting partisi, kemudian pilih **SCSI3 (0,0,0) (sda) - 28.5 GB ATA VBOX HARDDISK**. Pada bagian Create new empty partition table on this device pilih Yes.
[![img-1](/assets/week-1/26.png)](img)
[![img-1](/assets/week-1/27.png)](img)

17) Setelah itu, pilih free space yang tersedia.
[![img-1](/assets/week-1/28.png)](img)

18) Kemudian click **Create a new partition**.
[![img-1](/assets/week-1/29.png)](img)

18) Untuk Partition Size masukkan sebesar 20 GB dengan type **Primary**. location partition pilih **Beginning**
[![img-1](/assets/week-1/30.png)](img)
[![img-1](/assets/week-1/31.png)](img)
[![img-1](/assets/week-1/32.png)](img)

19) Pastikan Bootable flag dalam keaadan On, kemudian pilih **Done setting up the partition**. Setelah selesai, ulangi step sebelumnya untuk setting **partisi /storage sebesar 5 GB dan swap sebesar 1,5 GB**.
[![img-1](/assets/week-1/33.png)](img)
[![img-1](/assets/week-1/34.png)](img)
[![img-1](/assets/week-1/35.png)](img)

20) Setelah halaman **VirtualBox** terbuka, pilih new
[![img-1](/assets/week-1/36.png)](img)

21) Setelah halaman VirtualBox terbuka, pilih new
[![img-1](/assets/week-1/37.png)](img)

22) Setelah selesai, pilih **Finish partitioning and write changes to disk** dan tunggu hingga selesai.
[![img-1](/assets/week-1/56.png)](img)

23) Pada pilihan **Write the changes to disk?** pilih **Yes** lalu **Continue**
[![img-1](/assets/week-1/45.png)](img)

24) Untuk **Configure the package manager** pada bagian Scan extra installation media pilih **No**.
[![img-1](/assets/week-1/46.png)](img)

25) Selanjutnya untuk Debian archive mirror country pilih **Indonesia** dan Debian archive mirror pilih **kebo.pens.ac.id**.
[![img-1](/assets/week-1/47.png)](img)
[![img-1](/assets/week-1/48.png)](img)

26) Biarkan kosong untuk bagian HTTP proxy information dan tunggu hingga selesai.
[![img-1](/assets/week-1/49.png)](img)
[![img-1](/assets/week-1/50.png)](img)

27) Pada bagian **Participate in the package usage survey?** pilih **No**, lalu click Continue. Tunggu hingga selesai.
[![img-1](/assets/week-1/51.png)](img)
[![img-1](/assets/week-1/53.png)](img)

28) Untuk Software selection pilih **Debian desktop environment**, **GNOM** dan **Standart system utilities**, kemudian tunggu hingga selesai.
[![img-1](/assets/week-1/54.png)](img)
[![img-1](/assets/week-1/55.png)](img)

29) Pada bagian **Install the GRUB boot loader** untuk Install the GRUB boot loader pilih Yes dan Device for boot loader pilih **/dev/sda (ata-VBOX_HARDDISK_VBf5fb021a-7667d996)**. Click Continue dan tunggu hingga selesai.
[![img-1](/assets/week-1/new/51.png)](img)
[![img-1](/assets/week-1/new/52.png)](img)

30) Setelah selesai, click Continue dan sistem akan Rebooting.
[![img-1](/assets/week-1/new/53.png)](img)

31) Setelah semuanya selesai maka akan ke halaman login **Debian**.
[![img-1](/assets/week-1/new/54.jpeg)](img)
[![img-1](/assets/week-1/new/55.jpeg)](img)
<br><br>

# Referensi

- <https://www-techtarget-com.translate.goog/whatis/definition/operating-system-OS?_x_tr_sl=en&_x_tr_tl=id&_x_tr_hl=id&_x_tr_pto=tc>
- <https://www.gramedia.com/literasi/pengertian-sistem-operasi/>
- <https://telkomuniversity.ac.id/pengertian-data-fungsi-jenis-jenis-manfaat-dan-contohnya/>
- <https://bsi.today/sistem-operasi/>
- <https://asani.co.id/blog/booting-adalah/>
