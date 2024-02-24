<div align="center">
  <h1 style="text-align: center;font-weight: bold">Praktikum 1<br>Sistem Operasi</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br />
<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/id/4/44/Logo_PENS.png" alt="Logo PENS">
  <h3 style="text-align: center;">Disusun Oleh : <br>Kelompok 4</h3>
  <p style="text-align: center;">
    <strong>Muhammad Yafi Rifdah Zayyan (3123500001)</strong><br>
    <strong>Muhammad Daffa Erfiansyah (3123500006)</strong><br>
    <strong>Maula Shahihah Nur Sa'adah (3123500008)</strong>
  </p>

<h3 style="text-align: center;line-height: 1.5">Politeknik Elektronika Negeri Surabaya<br>Departemen Teknik Informatika Dan Komputer<br>Program Studi Teknik Informatika<br>2024/2025</h3>
  <hr><hr>
</div>

## Daftar Isi

1. [Pendahuluan](#sistem-operasi-)
2. [Soal 1](#1-jelaskan-langkah-langkah-proses-booting-)
3. [Soal 2](#2-bagaimana-cara-install-debian-di-virtual-box-)
4. [Referensi](#referensi)


## Sistem Operasi Debian 12

<b>Sistem operasi</b> (Inggris: operating system; disingkat OS) adalah perangkat lunak sistem yang mengatur sumber daya dari perangkat keras dan perangkat lunak, serta sebagai daemon untuk program komputer. Tanpa sistem operasi, pengguna tidak dapat menjalankan program aplikasi pada komputer mereka, kecuali program booting.
Sistem operasi mempunyai penjadwalan yang sistematis mencakup perhitungan penggunaan memori, pemrosesan data, penyimpanan data, dan sumber daya lainnya. Contoh sistem operasi modern adalah Linux, Android, iOS, Mac OS X, dan Microsoft Windows.

<b>Debian</b> adalah sistem operasi komputer yang tersusun dari paket-paket perangkat lunak yang dirilis sebagai perangkat lunak bebas dan terbuka dengan lisensi mayoritas GNU General Public License dan lisensi perangkat lunak bebas lainnya. Debian GNU/Linux memuat perkakas sistem operasi GNU dan kernel Linux merupakan distribusi Linux yang populer dan berpengaruh. Debian didistribusikan dengan akses ke repositori dengan ribuan paket perangkat lunak yang siap untuk instalasi dan digunakan. 

# Soal 1

## 1. Jelaskan langkah-langkah proses booting!

### Proses Booting

Proses booting pada komputer, termasuk laptop, terdiri dari beberapa tahapan yang menyusun dari saat tombol power ditekan hingga sistem operasi siap untuk digunakan. Berikut adalah tahapan-tahapan proses booting :

1. <b>Power On</b>
Saat tombol power atau tombol reset dihidupkan, sumber daya listrik akan mengalir ke komputer.
Kemudian, perangkat keras akan menerima daya untuk dinyalakan.

2. <b>Power-On Self-Test (POST)</b>
Setelah dinyalakan, komputer akan melakukan Power-On Self-Test atau POST, yang merupakan serangkaian tes perangkat keras untuk memastikan bahwa semuanya berfungsi dengan baik. 
POST akan memeriksa RAM, prosesor, kartu grafis, dan perangkat keras lainnya. 
Jika ada masalah dengan perangkat keras, komputer akan memberikan pesan kesalahan yang sesuai.

3. <b>Inisialisasi Perangkat Keras</b>
Setelah POST selesai, komputer akan menginisialisasi perangkat keras seperti hard drive, keyboard, mouse, dan perangkat lainnya. 
Proses ini melibatkan tahap mengenali perangkat keras, memuat driver yang diperlukan, dan menyiapkan perangkat untuk digunakan.

4. <b>Membaca Sektor Boot</b>
Selanjutnya, komputer akan mencari sektor boot di hard drive atau perangkat penyimpanan lainnya. 
Sektor boot sendiri adalah area khusus yang berisi instruksi awal untuk memuat sistem operasi.

5. <b>Memuat Sistem Operasi</b>
Setelah sektor boot ditemukan, komputer akan memuat sistem operasi ke dalam memori utama (RAM). 
Kemudian, sistem operasi akan mengambil alih kendali dan mulai menjalankan program-program yang diperlukan untuk mengoperasikan komputer.

## 2. Bagaimana cara install Debian 12 di Virtual Box?

## Tahap Instalasi

### Langkah 1

Download dan Install Software Virtualbox
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/1.png?raw=true)

<p>Download VirtualBox yang sesuai dengan Sistem Operasi dan spesifikasi pengguna</p>
</div>

### Langkah 2

Install Software Virtualbox
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/2.png?raw=true)

<p>Tampilan awal untuk menginstall VirtualBox kemudian pilih next untuk melanjutkan menginstall</p>
</div>

### Langkah 3

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/3.png?raw=true)

<p>Pilih penyimpanan yang diinginkan untuk standar penyimpanan biasanya pada Local Disk C/Program Files</p>
</div>

### Langkah 4

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/4.png?raw=true)

<p>Klik tombol "Yes" untuk melanjutkan install software VirtualBox</p>
</div>

### Langkah 5

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/5.png?raw=true)

<p>Klik tombol "Install" untuk melanjutkan proses instalasi software VirtualBox</p>
</div>

### Langkah 6

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/6.png?raw=true)

<p>Tunggu hingga proses penginstallan selesai</p>
</div>

### Langkah 7

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/7.png?raw=true)

<p>Setelah proses penginstallan selesai kemudian klik tombol "Finish" untuk melanjutkan pada software VirtualBox</p>
</div>

### Langkah 8

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/8.png?raw=true)

<p>Ini adalah tampilan awal pada software VirtualBox yang sudah terinstall kemudian klik tombol "New" untuk menginstall Debian</p>
</div>

### Langkah 9

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/9.png?raw=true)

<p>Berikan nama dan penyimpanan yang diinginkan pengguna dan masukan file .iso debian 12 yang sudah di download lalu pilih next</p>
</div>

### Langkah 10

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/10.png?raw=true)

<p>Pilih memory dan prosesor yang sesuai dengan spesifikasi pengguna untuk contoh pada device saya memilih memory 2048 dan prosesor 2 cpu</p>
</div>

### Langkah 11

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/11.png?raw=true)

<p>Pilih ukuran disk pada 26.50 GB kemudian klik tombol next</p>
</div>

### Langkah 12

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/12.png?raw=true)

<p>Cross check pada daftar yang ingin diinstall apakah sudah sesuai jika sudah klik tombol "Finish"</p>
</div>

### Langkah 13

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/13.png?raw=true)

<p>Tunggu hingga proses selesai</p>
</div>

### Langkah 14

Install Software Debian 12
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/14.png?raw=true)

<p>Ini adalah tampilan awal proses install pada Sistem Operasi Debian 12 pilih "Graphic Install" kemudian enter</p>
</div>

### Langkah 15

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/14a.png?raw=true)

<p>Pilih Bahasa English lalu tekan enter</p>
</div>

### Langkah 16

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/15.png?raw=true)

<p>Pilih lokasi United States lalu tekan enter</p>
</div>


### Langkah 17

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/16.png?raw=true)

<p>Ketik hostname dengan format "SysOp-NRP" untuk contoh saya isi dengan "Sysop-3123500006" kemudian tekan "Continue" untuk melanjutkan</p>
</div>

### Langkah 18

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/17.png?raw=true)

<p>Pada langkah ini kosongkan untuk domain name nya lalu tekan "Continue"</p>
</div>

### Langkah 19

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/18.png?raw=true)

<p>Buat paswword yang sesuai dengan pengguna lalu tekan "Continue" untuk melanjutkan</p>
</div>

### Langkah 20

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/19.png?raw=true)

<p>Masukkan nama pengguna kemudian klik "continue" untuk contoh saya memasukkan "daffaerfiansyah" </p>
</div>

### Langkah 21

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/21.png?raw=true)

<p>Membuat password untuk login pada Debian kemudian klik "Continue" untuk melanjutkan</p>
</div>

### Langkah 22

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/22.png?raw=true)

<p>Pilih lokasi Jam yang sesuai dengan pengguna</p>
</div>

### Langkah 23

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/23.png?raw=true)

<p>Pilih Manual kemudian klik tombol "Continue"</p>
</div>

### Langkah 24

Membuat Partisi

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/24.png?raw=true)

<p>Pilih "SCSI3 (0,0,0) (sda) - 28.5 GB AT VBOX HARDDISK" lalu klik "Continue"</p>
</div>

### Langkah 25

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/25.png?raw=true)

<p>Pilih "Yes" kemudian klik "Continue"</p>
</div>

### Langkah 26

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/26.png?raw=true)

<p>Tekan "pri/log 28.5 GB FREE SPACE" lalu klik "Continue" untuk membuat partisi</p>
</div>

### Langkah 27

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/27.png?raw=true)

<p>Pilih dan tekan "Create a new partition" kemudian klik "Continue"</p>
</div>

### Langkah 28

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/28.png?raw=true)

<p>Ketikan "20 GB" untuk membuat partisi pertama lalu tekan "Continue"</p>
</div>

### Langkah 29

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/29.png?raw=true)

<p>Pilih "Primary" lalu klik "Continue"</p>
</div>

### Langkah 30

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/30.png?raw=true)

<p>Pilih "Beginning" kemudian klik "Continue"</p>
</div>

### Langkah 31

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/31.png?raw=true)

<p>Kemudian klik "Done setting up the partition" dan klik "Continue" untuk kembali ke menu partisi</p>
</div>

### Langkah 32

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/32.png?raw=true)

<p>Kemudian klik "pri/log 8.5 GB FREE SPACE" untuk membuat partisi kedua lalu klik "Continue"</p>
</div>

### Langkah 33

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/33.png?raw=true)

<p>ketik "5 GB" kemudian klik "Continue"</p>
</div>

### Langkah 34

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/34.png?raw=true)

<p>Samakan dengan partisi pertama yaitu "Primary"</p>
</div>

### Langkah 35

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/35.png?raw=true)

<p>Samakan dengan partisi pertama yaitu "Beginning"</p>
</div>

### Langkah 36

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/36.png?raw=true)

<p>Klik "Done setting up the partition" dan klik "Continue" untuk kembali ke menu partisi</p>
</div>

### Langkah 37

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/37.png?raw=true)

<p>Pilih "pri/log 3.5 GB FREE SPACE" untuk membuat partisi ketiga</p>
</div>


### Langkah 38

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/38.png?raw=true)

<p>Ketik "1.5 GB" untuk partisi ketiga lalu tekan "Continue"</p>
</div>

### Langkah 39

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/39.png?raw=true)

<p>Tekan "Use as" lalu pilih "Swap Area" untuk menjadikan partisi ketiga sebagai swap</p>
</div>

### Langkah 40

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/40.png?raw=true)

<p>Klik "Done setting up the partition" untuk melanjutkan partisi ketiga</p>
</div>

### Langkah 41

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/41.png?raw=true)

<p>Klik "Finish partitioning and write changes to disk" untuk melanjutkan proses partisi</p>
</div>

### Langkah 42

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/42.png?raw=true)

<p>Tunggu hingga selesai</p>
</div>

### Langkah 43

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/43.png?raw=true)

<p>Pilih "No" lalu klik "Continue"</p>
</div>

### Langkah 44

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/44.png?raw=true)

<p>Pilih lokasi Indonesia kemmudian klik "Continue"</p>
</div>

### Langkah 45

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/45.png?raw=true)

<p>Pilih "kebo.pens.ac.id" lalu klik "Continue"</p>
</div>

### Langkah 46

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/46.png?raw=true)

<p>Kosongkan untuk langkah ini lalu klik "Continue"</p>
</div>

### Langkah 47

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/47.png?raw=true)

<p>Tunggu hingga proses selesai</p>
</div>

### Langkah 48

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/48.png?raw=true)

<p>Pilih "Yes" kemudian klik "Continue"</p>
</div>

### Langkah 49

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/49.png?raw=true)

<p>Centang pada 3 pilihan seperti di gambar lalu klik "Continue"</p>
</div>

### Langkah 50

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/50.png?raw=true)

<p>Tunggu hingga proses selesai</p>
</div>

### Langkah 51

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/51.png?raw=true)

<p>Pilih menu kedua seperti gambar diatas kemudian klik "Continue"</p>
</div>

### Langkah 52

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/52.png?raw=true)

<p>Tunggu hingga proses selesai</p>
</div>

### Langkah 53

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/53.png?raw=true)

<p>Klik "Continue" untuk menyelesaikan proses instalasi debian</p>
</div>

### Langkah 54

<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/System-Operation/blob/main/Minggu%201/Image%20Screenshot/54.png?raw=true)

<p>Ini adalah tampilan awal ketika Debian sudah terinstall</p>
</div>

## Referensi

[VirtualBox Download](https://www.virtualbox.org/wiki/Downloads)

[Debian 12 Download](https://www.debian.org/download)

[Sistem Operasi](https://id.wikipedia.org/wiki/Sistem_operasi)

[Debian](https://id.wikipedia.org/wiki/Debian)