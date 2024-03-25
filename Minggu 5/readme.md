<div align="center">
  <h1 style="text-align: center;font-weight: bold">Pratikum Minggu 5<br>Proses dan Manajemen Proses<br>Sistem Operasi</h1>
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

<div>
<h1 align="center">Pratikum 4 A<br>Proses dan Manajemen Proses</h1>
<h3>A. Tugas Pendahuluan</h3>
<ul>1. Apa yang dimaksud dengan proses?
<br>2. Apa yang dimaksud perintah untuk menampilkan status proses: ps, pstree.
<br>3. Sebutkan opsi yang dapat diberikan pada perintah ps
<br>4. Apa yang dimaksud dengan sinyal? apa perintah untuk mengirim sinyal?
<br>5. Apa yang dimaksud dengan proses foreground dan background pada job control?
<br>6. Apa yang dimaksud perintah-perintah penjadwalan prioritas: top, nice, renice.
</ul>
<h3>B. Percobaan</h3>
<ul><b>Percobaan 1: Status Proses</b>
<br>1. Instruksi ps (process status) digunakan untuk melihat kondisi proses yang ada. PID adalah Nomor Identitas Proses, TTY adalah nama terminal dimana proses tersebut aktif, STAT berisi S (Sleeping) dan R (Running), COMMAND merupakan instruksi yang digunakan.
<i>$ ps</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_01.png?raw=true)

<p>Analisa:

</p>
<br>2. Untuk melihat fak tor/elemen lainnya, gunakan option –u (user). %CPU adalah presentasi CPU time yang digunakan oleh proses tersebut, %MEM adalah presentasi system memori yang digunakan proses, SIZE adalah jumlah memori yang digunakan, RSS (Real System Storage) adalah jumlah memori yang digunakan, START adalah kapan proses tersebut diaktifkan
<i>$ ps -u</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_02.png?raw=true)

<p>Analisa:

</p>
<br>3. Mencari proses yang spesifik pemakai. Proses diatas hanya terbatas pada proses milik pemakai, dimana pemakai teresbut melakukan login
<i>$ ps –u (user)</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_03.png?raw=true)

<p>Analisa:

</p>
<br>4.	Mencari proses lainnya gunakan opsi a (all) dan au (all user)
<br><i>$ ps –a</i>
<br><i>$ ps –au</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_04.png?raw=true)

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_05.png?raw=true)

<p>Analisa:

</p>
<br><b>Percobaan 2: Menampilkan Hubungan Proses Parent dan Child</b>
<br>1. Ketik <b>ps –eH</b> dan tekan Enter. Opsi e memilih semua proses dan opsi H menghasilkan tampilan proses secara hierarki. Proses child muncul dibawah proses parent. Proses child ditandai dengan awalan beberapa spasi.
<br><i>$ ps -eH</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_06.png?raw=true)

<p>Analisa:

</p>
<br>2. Ketik ps –e f dan tekan Enter. Tampilan serupa dengan langkah 2. Opsi
–f akan menampilkan status proses dengan karakter grafis (\ dan _)
<br><i>$ ps –e f</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_07.png?raw=true)

<p>Analisa:

</p>
<br>3. Ketik pstree dan tekan Enter. Akan ditampilkan semua proses pada sistem dalam bentuk hirarki parent/child. Proses parent di sebelah kiri proses child. Sebagai contoh proses init sebagai parent (ancestor) dari semua proses pada sistem. Beberapa child dari init mempunyai child. Proses login mempunya i proses bash sebagai child. Proses bash mempunyai proses child startx. Proses startx mempunyai child xinit dan seterusnya.
<br><i>$ pstree</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_08.png?raw=true)

<p>Analisa:

</p>
<br>4. Ketik pstree | grep mingetty dan tekan Enter. Akan menampilkan semua proses mingetty yang berjalan pada system yang berupa console virtual. Selain menampikan semua proses, proses dikelompokkan dalam satu baris dengan suatu angka sebagai jumlah proses yang berjalan.
<br><i>$ pstree | grep mingetty</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_09.png?raw=true)

<p>Analisa:

</p>
<br>5. Untuk melihat semua PID untuk proses gunakan opsi <b>–p</b>.
<i>$ pstree –p</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_09.png?raw=true)

<p>Analisa:

</p>
<br>6. Untuk menampilk an proses dan ancestor yang tercetak tebal gunakan opsi
–h.
<br><i>$ pstree –h</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_10.png?raw=true)

<p>Analisa:

</p>
<br><b>Percobaan 3: Menampilkan Status Proses dengan Berbagai Format</b>
<br>1.	Ketik ps –e | more dan tekan Enter. Opsi -e menampilkan semua proses dalam bentuk 4 kolom : PID, TTY, TIME dan CMD.
<br><i>$ ps –e | more</i>
<br>Jika halaman penuh terlihat prompt --More-- di bagian bawah screen, tekan q untuk kembali ke prompt perintah.

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_11.png?raw=true)

<p>Analisa:

</p>
<br>2.	Ketik ps ax | more dan tekan Enter. Opsi a akan menampilkan semua proses yang dihasilkan terminal (TTY). Opsi x menampilkan semua proses yang tidak dihasilkan terminal. Secara logika opsi ini sama dengan opsi –e . Terdapa 5 kolom : PID, TTY, STAT, TIME dan COMMAND.
<br><i>$ ps ax | more</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_12.png?raw=true)

<p>Analisa:

</p>
<br>3. Ketik ps –e f | more dan tekan Enter. Opsi –e f akan menampilkan semua proses dalam format daftar penuh.
<br><i>$ ps ef | more</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_13.png?raw=true)

<p>Analisa:

</p>
<br>4. Ketik ps –eo pid, cmd | more dan tekan Enter. Opsi –eo akan menampilkan semua proses dalam format sesuai definisi user yaitu terdiri dari kolom PID dan CMD.
<br><i>$ ps –eo pid,cmd | more</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_14.png?raw=true)

<p>Analisa:

</p>
<br>5.	Ketik ps –eo pid,ppid,%mem,cmd | more dan tekan Enter. Akan menampilkan kolom PID, PPID dan %MEM.   PPID adalah proses ID dari proses parent. %MEM menampilkan persentasi memory system yang digunakan proses. Jika proses hanya menggunakan sedikit memory system akan dita mpilkan 0.
<br><i>$ ps –eo pid,ppid,%mem,cmd | more</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_15.png?raw=true)

<p>Analisa:

</p>
<br><b>Percobaan 4: Mengontrol proses pada shell</b>
<br>1. Gunakan perintah yes yang mengirim output y yang tidak pernah berhenti
<br><i>$ yes</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_16.png?raw=true)

<p>Analisa:

</p>
<br>2. Belokkan standart output ke /dev/null
<br><i>$ yes > /dev/null</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_17.png?raw=true)

<p>Analisa:

</p>
<br>3. Salah satu cara agar perintah yes tetap dijalankan tetapi shell tetap digunakan untuk hal yang lain dengan meletakkan proses pada background dengan menambahkan karakter & pada akhir perintah.
<br><i>$ yes > /dev/null &</i>
<br>Angka dalam ”[ ]” merupakan job number diikuti PID.
<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_18.png?raw=true)

<p>Analisa:

</p>
<br>4. Untuk melihat status proses gunakan perintah jobs.
<br><i>$ jobs</i>


<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_19.png?raw=true)

<p>Analisa:

</p>
<br>5. Untuk menghentikan job, gunakan perintah kill diikuti job number atau PID proses.   Untuk identifikasi job number, diikuti prefix dengan karakter ”%”.
<br><i>$ kill %(nomor job) contoh : kill %1</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_20.png?raw=true)

<p>Analisa:

</p>
<br>6. Lihat status job setelah diterminasi
<br><i>$ jobs</i>

<br>

![App Screenshot](https://github.com/daffaerfiansyah/SysOp24-3123500006/blob/main/Minggu%205/Assets/IMG_21.png?raw=true)

<p>Analisa:

</p>

</div>