<div align="center">
  <h1 style="text-align: center;font-weight: bold">Praktikum 1<br>Sistem Operasi</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br />
<div align="center">
  <img src="https://i.ibb.co/DC3QHnM/logo-pens.png" alt="Logo PENS">
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
- [Perbedaan LEGACY dan UEFI](#perbedaan-legacy-dan-uefi)
- [Kesimpulan](#kesimpulan)
- [Referensi](#referensi)

# Perbedaan LEGACY dan UEFI

| # | LEGACY | UEFI |
| --- | --- | --- |
| Deskripsi | Legacy Bios, alat yang membantu firmware Bios dalam memproses boot yang berfungsi untuk menyimpan daftar penyimpanan yang bisa untuk di boot seperti Floopy Disk Drives, Optical Disk Drive, Hard Disk Drive, dll. | UEFI ( Unified Extensible Firmware Interface), teknologi terbaru yang dibuat untuk penyempurnaan dari BIOS yang lama menjadi BIOS yang memiliki fungsi yang lebih optimal. |
| Skema Partisi | Menggunakan MBR (Master Boot Record), merupakan sistem partisi versi lawas.  | Menggunakan GPT (Guid Partition Table), merupakan sistem partisi yang mendukung hardware canggih di jaman modern saat ini. |
| Partisi | Mampu menampung lebih dari 2TB, dapat membuat lebih dari 128 partisi utama, bisa menyimpan lebih dari satu bootloader. | 1.	MBR legacy hanya mampu menampung partisi sekitar 2TB, hanya bisa membuat 4 partisi utama, hanya mampu mennyimpan 1 bootloader
| User Interface | pengguna hanya dapat menggunakan keyboard. | pengguna tidak hanya menggunakan keyboard, tetapi juga dapat menggunakan mouse. |
| Language | Ditulis dalam Bahasa Low-level yang bergantung pada arsitektur prosesor spesifik | ditulis dalam  Bahasa pemrograman High-Level “C” yang memungkinkan pengguna untuk memeperbarui atau memperbaiki bug dengan mudah. |
| User friendly  | hanya mampu dijalankan pada mode 16-bit. | lebih ramah pengguna karena mampu dijalankan pada mode 32-bit atau 64-bit.
| Security | tidak menyediakan fitur keamanan. | Menyediakan fitur keamanan yang mencegah malware menginfeksi sistem saat sistem dinyalakan.
| Booting Storage | Mendukung 2.2 Terabyte ukuran drive. | Mendukung hingga 9 Zetabyte ukuran drive.
| Booting time | Waktu booting lebih lama. | Waktu booting UEFI lebih cepat.

![img](../assets/flow_legacy.png)



# Kesimpulan
Perbedaan utama antara BIOS Legacy dan UEFI (Unified Extensible Firmware Interface) terletak pada teknologi dan fitur yang mereka tawarkan. BIOS Legacy beroperasi dalam mode real atau 16-bit dengan kapasitas addressing terbatas pada 32-bit, yang membatasi kemampuan sistem untuk mengakses RAM dan perangkat keras modern. Selain itu, BIOS Legacy kurang memiliki fitur keamanan tingkat tinggi dan sering diakses melalui antarmuka teks sederhana. Sebaliknya, UEFI beroperasi dalam mode 32-bit atau 64-bit, mendukung addressing 64-bit untuk akses ke kapasitas RAM yang lebih besar dan perangkat keras modern. UEFI juga menonjol dengan fitur keamanan canggih seperti Secure Boot, yang memastikan integritas boot loader dan sistem operasi. Antarmuka pengguna grafis yang ditingkatkan dan kemampuan inisialisasi perangkat keras yang lebih fleksibel membuat UEFI menjadi pilihan utama dalam sistem komputer modern, sementara BIOS Legacy masih hadir dalam beberapa implementasi.

# Referensi

- [UEFI and LEGACY](https://www.freecodecamp.org/news/uefi-vs-bios/#:~:text=UEFI%20supports%20drive%20sizes%20upto,UEFI%20provides%20faster%20boot%20time.)
- [What is the Difference Between UEFI and Legacy?](https://itslinuxfoss.com/difference-between-uefi-and-legacy/)
- [Perbedaan Uefi dan Legacy](https://seberkas.com/perbedaan-uefi-dan-legacy/#google_vignette)
- [ARTI DAN PERBEDAAN MBR GPT LEGACY UEFI](https://tecotak.com/mbr-gpt-legacy-uefi/)
