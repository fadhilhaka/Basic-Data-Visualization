# Menggambarkan Kuantitatif Data ke Bentuk Diagram

Jenis grafik dalam Google Sheets bisa dikombinasikan dengan jenis model lainnya. Misalnya, diagram batang dapat dikombinasikan dengan diagram garis. Namun, penerapannya juga harus sesuai dan tidak dipaksakan supaya data dapat mudah dipahami.

## [Latihan](https://docs.google.com/spreadsheets/d/1Kak3PcB6Tx6_v8gYcPnFDHNvi8F5NorwebheH6uGxhY/edit#gid=105042482)

Latihan ini akan menggunakan [data](https://dicodingacademy.blob.core.windows.net/picodiploma/visualisasi_data_academy/AB_NYC_2019.csv) kamar Airbnb yang disewakan di kota New York.

### Langkah 1: Persiapan

Pastikan semua tools dan data sudah dipersiapkan. Setelah semua siap, maka buat Google Sheet baru.

Untuk memasukkan data dari komputer ke Google Sheet, klik File → Import dan pilih/taruh berkas yang ingin dimasukkan.

Sheet akan terisi dengan data dari berkas yang kita unggah.

### Langkah 2: Visualisasi

Pilih kolom dan baris mana yang ingin kita visualisasikan, namun sebelumnya, kita perlu memahami maksud dari data tersebut. 

Pertama kita mengetahui arti tiap kolom pada data tersebut:

* Id : Identifier unik untuk tiap tempat sewa
* Name : Nama tempat
* Host_id : Identifier penyedia kamar/tempat
* Host_name : Nama penyedia kamar/tempat
* Neighbourhood_group : Kelompok lingkungan dari tempat tinggal yang disediakan host (penyedia kamar/tempat), merupakan pengelompokan dari neighbourhood
* Neighbourhood : Nama dari lingkungan tempat tinggal yang disediakan host
* Latitude & longitude : Garis lintang dan garis bujur dari tempat tinggal yang disediakan
* Room_type : Tipe kamar yang disediakan
* Price : Harga sewa per malam dalam dolar Amerika
* Minimum_nights : Jumlah minimum malam yang disewa untuk setiap penyewaan
* Number_of_reviews : Jumlah ulasan oleh pelanggan
* Last_review : Tanggal review terakhir oleh pelanggan
* Reviews_per_month : Rata-rata ulasan jika dibagi per bulan
* Calculated_host_listings_count : Jumlah tempat milik host yang telah didaftarkan ke Airbnb
* Availability_365 : Beberapa hari dalam setahun, tempat tersedia untuk pemesanan

Setelah kita mengetahui maksud dari kolom dan isian data tersebut kita mulai dapat membuat pertanyaan pada diri sendiri, sebagai contohnya “Saya ingin melihat perbandingan rata-rata harga tiap tipe kamar.”

Dari sana kita tahu bahwa kolom yang kita gunakan adalah room_type dan price dengan menggunakan semua baris. Untuk mulai membuat visualisasi maka pilih semua data yang tersedia di kolom I (room_type) dan J (price). 

Cara cepat untuk melakukan hal tersebut adalah dengan menekan tombol shift pada keyboard sambil klik kolom I dan J. 

Setelah data yang dibutuhkan telah dipilih, kita dapat memvisualisasikan dengan klik Insert → Chart.

Secara standar grafik yang pertama terbentuk adalah jenis Column chart (grafik kolom) di mana X-axis berupa room_type dan Y-axis (Series) berupa sum (penjumlahan) dari price.

Nah bisa kita lihat bahwa grafik yang terbentuk tidaklah rapi. Terlalu banyak data poin pada X-axis. Hal tersebut dikarenakan kita tidak melakukan grouping atau pengelompokan. Oleh karena itu silakan centang tombol Aggregate untuk melakukan agregasi terhadap data room_type yang sama.

Untuk mengubah jenis grafik yang diinginkan dan sesuai dengan jenis data yang kita pilih, klik Chart type pada Chart editor.

Hal yang perlu diperhatikan adalah setiap tipe grafik masing-masing memiliki kebutuhan data yang berbeda-beda. Seperti halnya pada grafik kolom, data yang dibutuhkan adalah X-axis dan satu data Y-axis (Series). Sementara itu jika ingin membuat Combo chart (grafik kombo yang kombinasikan grafik Line dengan Column), Y-axis perlu ditambahkan data lainnya sebagai perbandingan.

Untuk melakukan styling pada font, legend, warna, dan lainnya, lakukan konfigurasi sesuai jenis grafik yang kita pilih pada bagian Customize.

## Kesalahan Umum dalam Visualisasi Data

Visualisasi akan efektif jika dibuat dengan mematuhi kaidah yang ditentukan. Namun, terkadang penerapan visualisasi data dilakukan dengan cara yang sebaliknya: tak tepat dan tak patuh pedoman. Sehingga penerapan visualisasi data kadang berujung pada informasi yang membingungkan dan ambigu.

### Nilai Persentase Tidak Sesuai

Jika menggunakan satuan persen maka total data yang disajikan totalnya harus 100%. Apabila menggunakan satuan derajat maka data yang disajikan totalnya harus 360 derajat. 

Besar porsi irisan juga harus sesuai dengan nilai datanya. Jangan pula menampilkan terlalu banyak irisan yang bisa berujung bias.

Idealnya irisan diagram lingkaran tak lebih dari empat irisan supaya perpotongan irisannya terlihat jelas. Sehingga kita tahu data mana yang lebih besar atau lebih kecil.

Lalu bagaimana kalau data yang ingin ditulis berjumlah enam? Kita dapat menggunakan “lainnya”, namun perlu ditambahkan keterangan kategori lainnya itu berisi apa saja. 

Jika data yang dibutuhkan sangat banyak misal lebih dari 100 data, maka kita perlu menuliskan data dalam bentuk tabel, bukan diagram lingkaran.

### Terlalu Banyak Data

### Tidak Mengikuti Standar Penulisan

### Terdapat Sumbu yang Terpotong

### Penggunaan Grafik 3D yang Kurang Sesuai

### Susah Dibandingkan

[Referensi](https://viz.wtf/)