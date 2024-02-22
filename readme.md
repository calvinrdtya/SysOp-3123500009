# Proses Booting
### Apa itu Booting?
Booting adalah proses awal ketika komputer atau perangkat lainnya dinyalakan atau di-restart. Istilah "booting" sendiri berasal dari kata "bootstrap," yang awalnya merujuk pada konsep mengangkat diri sendiri dengan tali sepatu. Proses booting bertujuan untuk memuat sistem operasi dan perangkat lunak lainnya ke dalam memori sehingga komputer dapat berfungsi secara normal.

## Langkah-Langkah Booting
1) Power On
    - Saat tombol daya ditekan atau sumber daya lainnya diaktifkan, listrik mengalir ke komponen-komponen perangkat keras komputer.
2) POST (Power-On Self-Test)
    - Setelah tombol power ditekan, laptop melakukan POST (Power-On Self-Test).
    - POST adalah proses pemeriksaan awal perangkat keras seperti RAM, prosesor, dan perangkat penyimpanan untuk memastikan bahwa semuanya berfungsi dengan baik.
3) BIOS/UEFI
    - Jika POST berhasil, laptop memuat BIOS (Basic Input/Output System) atau UEFI (Unified Extensible Firmware Interface).
    BIOS/UEFI menyediakan antarmuka perangkat keras dan menentukan perangkat penyimpanan yang akan di-boot
4) Inisialisasi Perangkat Keras
   - Komputer akan menginisialisasi perangkat keras seperti hard drive, keyboard, mouse, dan perangkat lainnya. Proses ini melibatkan tahap mengenali perangkat keras, memuat driver yang diperlukan, dan menyiapkan perangkat untuk digunakan.
5) Pemilihan Perangkat Boot
    - Di dalam BIOS/UEFI, laptop mencari perangkat penyimpanan yang diatur sebagai perangkat boot. Perangkat boot biasanya adalah hard disk internal atau SSD, tetapi dapat diatur untuk boot dari perangkat lain seperti USB atau CD/DVD jika diperlukan.
6) Boot Loader
    - Setelah perangkat boot dipilih, boot loader (misalnya, GRUB untuk Linux atau bootloader Windows) dimuat ke dalam memori. Boot loader bertanggung jawab untuk memuat sistem operasi yang sebenarnya.
7) Sistem Operasi
    - Boot loader memuat sistem operasi yang telah diinstal pada perangkat penyimpanan.
    Sistem operasi kemudian dimuat ke dalam memori RAM dan proses booting berlanjut.
8) Login
   - Setelah proses booting selesai, sistem operasi menampilkan layar login. Pengguna dapat memasukkan informasi login seperti username dan password.
9) Desktop/Interface Pengguna
    - Setelah login berhasil, sistem operasi memuat desktop atau antarmuka pengguna.