# **Struktur Sistem Operasi**
Struktur sistem operasi modern merupakan suatu sistem yang besar
dan kompleks sehingga strukturnya harus dirancang dengan hati-hati 
dan saksama supaya dapat berfungsi seperti yang diinginkan serta 
dapat dimodifikasi dengan mudah. Struktur sistem operasi merupakan 
komponen-komponen sistem operasi yang dihubungkan dan dibentuk 
di dalam kernel.

## Kernel
Kernel merupakan Sebuah perangkat yang berfungsi sebgai mediator atau sebuah perangkat yang membuat komunikasi antara perangkat lunak dan perangkat keras komputer. 
### Fungsi Kernel Pada Sistem Operasi Komputer
- Kernel berfungsi untuk melayani perangkat lunak aplikasi untuk dapat mengakses perangkat keras atau hardware secara aman.
- Kernel juga berfungsi sebagai pengatur  kapan dan berapa lama sebuah program aplikasi dapat menggunakan satu bagian perangkat keras. hal tersebut biasanya disebut dengan **Multiplexing**
- Membantu dan mendukung perangkat lunak aplikasi untuk mengeksekusi dengan fitur abtraksi perangkat keras (hardware)

### Jenis/kategori Kernel
- **Kernel monolitik** yaitu kernel yang mengintegrasikan banyak fungsi di dalam kernel dan menyediakan lapisan abstraksi perangkat keras secara penuh terhadap perangkat keras yang berada di bawah sistem operasi.
- **Kernel Microkernel** adalah kernel yang menyediakan hanya sekumpulan kecil dari abstraksi perangkat keras sederhana, dan menggunakan aplikasi-aplikasi yang disebut dengan server untuk menyediakan fungsi-fungsi lainnya.
- **Kernel Hybrid** (modifikasi dari microkernel) adalah kernel yang persis atau mirip dengan microkernel, akan tetapi ia juga memasukkan beberapa kode atau tambahan kode di dalam ruangan kernel suapaya ia menjadi lebih cepat atau untuk meningkatkan performanya.
- **Kernel Exokernel** adalah kernel yang tidak menyediakan sama sekali abstraksi perangkat keras, akan tetapi ia menyediakan sekumpulan library yang menyediakan fungsi akses ke perangkat keras (hardware) secara langsung atau hampir-hampir langsung.

## Struktur sederhana
 Struktur sistem operasi ini yang 
menyediakan fungsional dalam ruang yang sedikit sehingga tidak dibagi 
menjadi beberapa modul, inisialisasinya terbatas pada fungsional perangkat 
keras yang terbagi menjadi dua bagian yaitu 
kernel dan sistem program. Kernel terbagi 
menjadi serangkaian interface dan device 
driver dan menyediakan sistem file, 
penjadwalan CPU, manajemen memori, dan 
fungsi-fungsi sistem operasi lainnya melalui 
system call. 

## Sistem Berlapis
Sistem operasi dibentuk secara hirarki berdasar 
lapisan-lapisan, dimana lapisan-lapisan bawah 
memberi layanan lapisan lebih atas. Lapisan 
yang paling bawah adalah perangkat keras, dan 
yang paling tinggi adalah user-interface. Sebuah 
lapisan adalah implementasi dari obyek abstrak 
yang merupakan enkapsulasi dari data dan operasi yang bisa memanipulasi data 
tersebut. Struktur berlapis dimaksudkan untuk mengurangi kompleksitas 
rancangan dan implementasi sistem operasi. Tiap lapisan mempunyai fungsional 
dan antarmuka masukan-keluaran antara dua lapisan bersebelahan.

## Mesin Virtual

Virtual machine mempunyai sistem timesharing yang berfungsi untuk, 
menyediakan kemampuan untuk multiprogramming dan perluasan mesin dengan 
antarmuka yang lebih mudah. Struktur Mesin maya ( CP/CMS, VM/370 ) terdiri 
atas komponen dasar utama : 

- *Control Program*, yaitu virtual machine monitor yang mengatur fungsi ari 
prosessor, memori dan piranti I/O. Komponen ini berhubungan langsung 
dengan perangkat keras.
- *Conventional Monitor System*, yaitu sistem operasi sederhanayang mengatur 
fungsi dari proses, pengelolaan informasi dan pengelolaan piranti. 