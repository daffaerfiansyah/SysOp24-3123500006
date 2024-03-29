<div align="center">
  <h1 style="text-align: center;font-weight: bold">Pratikum Minggu 3<br>Sistem Operasi</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br/>
<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/id/4/44/Logo_PENS.png" alt="Logo PENS">
  <h3 style="text-align: center;">Disusun Oleh : <br>Kelompok 4</h3>
  <p style="text-align: center;">
    <strong>Muhammad Yafi Rifdah Zayyan (3123500001)</strong><br>
    <strong>Muhammad Daffa Erfiansyah (3123500006)</strong><br>
    <strong>Maula Shahihah Nur Sa'adah (3123500008)</strong>
  </p>

<h3 style="text-align: center;line-height: 1.5">Politeknik Elektronika Negeri Surabaya<br>Departemen Teknik Informatika Dan Komputer<br>Program Studi Teknik Informatika<br>2023/2024</h3>
  <hr><hr>
</div>

## Daftar Isi

1. [Powerpoint](#ppt)
2. [IOPS dan FLOPS](#iops-flops)
   - [Benchmarking](#benchmarking)
   - [Analisa Hasil Benchmarking](#analisa-hasil-benchmarking)
   - [Tabel Perbandingan Pengujian](#tabel-perbandingan-pengujian)
     - [Analisa](#analisa-pengujian)
     
<div align="center">

## Powerpoint Siklus CPU

</div>
<p>
Berikut mengenai presentasi atau penjelasan langkah-langkah dalam siklus CPU(Fetch,Decode,Execute) dalam mengeksekusi sebuah program

Yang dapat diakses pada link berikut: [PPT Siklus CPU](https://www.canva.com/design/DAF_RTHy4wk/7QWlAIIeue3ksGOfXBmg9Q/edit)

</p>
<br>
<div align="center">

## Iops dan Flops
</div>

<h2>Definisi</h2>

<h3>IOPS</h3>
<p>Input/output operations per second(IOPS) adalah pengukuran kinerja input/output yang digunakan untuk mengkarakterisasi perangkat penyimpanan komputer seperti hard disk drive (HDD), solid state drive (SSD), dan jaringan area penyimpanan (SAN). Seperti tolak ukur, angka IOPS yang diterbitkan oleh produsen perangkat penyimpanan tidak secara langsung berhubungan dengan kinerja aplikasi dunia nyata.</p>
<h3>FLOPS</h3>
<p>Dalam komputasi, floating point operations per second (FLOPS, flops or flop/s) adalah ukuran kinerja komputer, berguna dalam bidang perhitungan ilmiah yang memerlukan perhitungan floating-point. Untuk kasus seperti itu, ini adalah ukuran yang lebih akurat daripada mengukur instruksi per detik.</p>
<br>
<h2 align="center">Melakukan Benchmarking pada PC</h2>

<p>1. Melakukan Instalasi Package GCC,Make dan Git pada Debian 12 yang sudah terinstall</p>
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%203/Assets/IMG_Install%20Gcc.png?raw=true)
<p>Lakukan perintah "$ sudo apt update" pada terminal kemudian ketik "$ sudo apt install gcc" untuk menginstall compile dan "$ sudo apt install git" untuk menginstall git pada debian</p>
</div>

<p>2. Melakukan Git clone pada Debian 12</p>
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%203/Assets/IMG_Git%20clone.png?raw=true)
<p>Arahkan direktori pada terminal yang ingin dituju lalu ketik "$ git init" kemudian "$ git clone (paste link github) lalu tekan enter</p>
</div>
<p>3. Melakukan Build Binaries,Cleaning, dan Install Binaries</p>
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%203/Assets/IMG_make.png?raw=true)
<p>Arahkan direktori pada folder flops/iops yang telah dilakukan git clone pada langkah sebelumnya kemudian buka terminal dan ketik "$ make"</p>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%203/Assets/IMG_Make%20Clean.png?raw=true)
<p>Kemudian lakukan perintah "$ make clean" lalu ketik "$ sudo make install" untuk menginstall binaries pada debian.</p>
</div>
<p>4. Melakukan Proses Benchmarking menggunakan Iops dan Flops</p>
<div align="center">

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%203/Assets/IMG_IOPS64.png?raw=true)
<p>Untuk benchmarking menggunakan iops ketik pada terminal "$ iops32 $(nproc)" atau iops64 sesuaikan dengan spesifikasi laptop yang dipakai</p>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%203/Assets/IMG_FLOPS64.png?raw=true)
<p>Untuk benchmarking pada flops sama seperti iops hanya saja mengganti dari iops menjadi flops "$ flops32 $(nproc)" atau $ flops64 $(nproc)</p>
</div>
<br>
<h2 align="center">Analisa Hasil Benchmarking</h2>

<p justify-content="center">
<p>Spesifikasi Laptop yang saya pakai:</p>
<p>AMD Ryzen 3 3200U with Radeon Vega Mobile Gfx 2.60 GHz</p>

|                      | IOPS64 (Integer)         | FLOPS64 (Floating Point)    |
|----------------------|------------------------|---------------------------|
| Total Throughput     | 6.339286 Gigaiops     | 5.637343 Gigaflops       |
| Single Core Throughput | 3.185454 Gigaiops   | 2.821573 Gigaflops       |
</p>

<p>Dengan melihat tabel di atas, dapat dilihat bahwa IOPS memiliki total throughput dan throughput single core yang lebih tinggi dibandingkan dengan FLOPS. Namun demikian, perbedaan antara total throughput dan throughput single core juga penting untuk diperhatikan karena menunjukkan seberapa baik CPU dapat mengalokasikan dan memanfaatkan sumber daya secara efisien antara inti tunggal dan total throughput.</p>
<h2>Hasil Perbandingan dengan teman kelompok</h2>


| Nama  | CPU | Max Single Core FLOPS | Max Single Core IOPS | Max CPU FLOPS    | Max CPU IOPS   |
| ----- | ----------- | --------------------- | -------------------- | ---------------- | ---------------|
| Yafi  | Intel® Core™ i5-1335U Processor  4.6 GHz | 5.6 Gigaflops         | 3.9 Gigaiops         | 11.1 Gigaflops   | 7.7 Gigaiops   |
| Daffa | AMD Ryzen 3 3200U 2.60 GHz | 3.4 Gigaflops         | 3.5 Gigaiops         | 6.5  Gigaflops   | 6.7 Gigaiops   |
| Maula | AMD Ryzen 3 3250U 2.6GHz | 4.5 Gigaflops         | 4.1 Gigaiops         | 8.2  Gigaflops   | 7.5 Gigaiops   |

<br>
</div>


## Referensi
[Wikipedia IOPS](https://en.wikipedia.org/wiki/IOPS)

[Wikipedia FLOPS](https://en.wikipedia.org/wiki/FLOPS)