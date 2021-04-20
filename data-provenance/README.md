# Dokumentasi Data

Dokumentasi data atau yang sering disebut dengan data provenance adalah sebuah langkah untuk melihat sumber data yang kita peroleh. Kata provenance sendiri berasal dari bahasa perancis provenir yang berarti “berasal” atau “silsilah”.

Coba bayangkan Anda berperan sebagai seorang Data Scientist. Anda mendapatkan sebuah dataset (himpunan data) yang siap untuk dianalisis. Anda tidak tahu data ini berasal dari mana, bagaimana validitasnya, apakah ia akan berubah selama proses pengerjaan Anda, dan sebagainya. Gawat kan? Padahal dokumentasi data ini penting untuk mengetahui keabsahan data dan memungkinkan kita menggunakannya kembali di waktu yang lain.

W3C Provenance Incubator Group, sebuah organisasi yang bergerak di bidang pengembangan dan standarisasi teknologi web, menjelaskan tentang dokumentasi data sebagai berikut:

>“Catatan yang menggambarkan semua pihak dan proses dalam pembuatan, perubahan, penanganan, mau pun hal lainnya yang berpengaruh kepada data. Provenance merupakan landasan utama untuk dapat menilai keaslian dan menumbuhkan kepercayaan kepada data, sekaligus untuk mereproduksi data tersebut.”

Berikut ini contoh sebuah penggambaran dokumentasi data yang ditunjukkan dalam sebuah metadata. Metadata merupakan bagian penting dari data yang dipublikasi untuk menentukan kualitas, kredibilitas, reprodusibilitas hasil (terukur), serta menentukan apakah data dapat digunakan kembali atau tidak (reusable).

![](https://d17ivq9b7rppb3.cloudfront.net/original/academy/202102220059440cf8979447504e03a3a5b22d16d990c3.png)

Contoh data provenance di atas didapatkan dari website [kaggle](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset/metadata). Pada gambar di atas terlihat dokumentasi yang menyertakan sumber data, metodologi pembuatan data, dan juga pemilik dari dataset.

## Pentingnya Dokumentasi Data

Kepercayaan, kredibilitas, dan reproduksibilitas terhadap sebuah data dapat didasari oleh dokumentasi sumber data yang sesuai. Dalam sebuah penelitian, pengguna data tidak serta merta dapat menjadi pembuat data.

Orang yang membuat data dapat:

1. mengonfigurasikan instrumen atau simulasi dari mengumpulkan data primer; atau,
2. menerapkan metodologi dan proses tertentu guna mengekstraksi, mengubah, dan menganalisis data masukan demi menghasilkan sebuah produk data keluaran.

### Mengelola Sumber Data

Provenance dapat dicatat dalam jenis metadata tentang sebuah data. Banyak bidang metadata yang dapat dikumpulkan dalam kategori informasi asalnya. Misalnya tanggal pembuatan, pemilik, perangkat lunak atau tools lain yang digunakan, metode pemrosesan data, dan lain sebagainya. Dengan demikian, pengelolaan dan manajemen data yang baik menjadi dasar dari dokumentasi data yang akurat.

Salah satu usaha dan pendekatan yang mungkin Anda familier adalah teknologi blockchain dalam manajemen rantai persediaan. Video berikut bercerita bagaimana teknologi blockchain dapat digunakan untuk mendapatkan informasi mengenai kapan, di mana, dan bagaimana cara penangkapan ikan dapat diketahui dengan memindai barcode yang telah dipasangkan ke ikan atau pengemasannya. Dengan begitu, distributor, toko penjual, dan konsumen dapat dengan mudah mencari asal usul ikan tersebut dan bisa langsung tahu jika ikan didapatkan dari penangkapan secara ilegal.

https://www.youtube.com/watch?v=oOywU_rXgFE&feature=emb_imp_woyt

Bayangkan bahwa metadata adalah lokasi ikan ditangkap, nelayan yang menangkapnya, kapan ikan tersebut ditangkap, dan sebagainya. Sementara data adalah ikan itu sendiri.

Pendekatan yang dapat dilakukan dalam melakukan dokumentasi data sebagai berikut:

* Dicatat dalam bentuk teks, bisa menggunakan skema penulisan umum atau bisa juga dengan skema khusus dalam data provenance.
* Dicatat dan disimpan secara internal menggunakan program perangkat lunak atau dalam sistem eksternal lainnya.
* Dituliskan dalam bentuk yang dapat dibaca oleh mesin atau yang bisa dibaca oleh manusia.

Bentuk sederhananya, sebuah sumber dicatat dan disimpan dalam sebuah berkas berjudul README yang di dalamnya menjelaskan tentang pengumpulan data dan metode pemrosesan. Data sumber juga dapat dicatat dengan lebih terstruktur menggunakan elemen-elemen spesifik dalam standar metadata seperti [Dublin Core](http://dublincore.org/), hingga standar disiplin metadata khusus seperti [ISO 19115-2](https://www.iso.org/standard/67039.html).

* README, Untuk penulisan readme, kamu bisa menggunakan template yang telah distandarkan oleh Cornell University pada tautan [berikut](https://data.research.cornell.edu/content/readme).
* Data Dictionaries, atau kamus data, berisi informasi kunci tentang data yang Anda kumpulkan. Ia digunakan untuk menjelaskan suatu bagian tertentu dalam dataset. Misalnya menjelaskan arti dari nama sebuah variabel, kegunaan, deskripsi, dan lain sebagainya. Contoh dari data dictionaries dapat dilihat dari kamus data yang disediakan oleh Kementerian Pertanian Amerika Serikat pada tautan [berikut](https://data.nal.usda.gov/data-dictionary-examples).
* Data Paper, berbeda dengan makalah, jurnal, atau artikel penelitian biasa yang berfokus pada hipotesa dan hasil penelitian, data paper bertujuan utama untuk menjelaskan mengenai data dan bagaimana data tersebut dikumpulkan. Dalam kata lain, data paper dapat disebut sebagai sebuah dokumen berisi metadata.

### Tools Dokumentasi Data

* Buku Catatan
* Log dan Blockchain, jika bekerja sendiri, Anda dapat melakukan logging, atau menggunakan tools bantuan (docs, spreadsheet) yang memiliki kemampuan untuk memperlihatkan history (sejarah versi). Anda yang bekerja dengan tools modern mungkin mengenal istilah logging atau auditing. Anda dapat memanfaatkan log aplikasi untuk mencatat perubahan pada data. Pada pasar perdagangan dunia, pencatatan ini dapat dilakukan melalui shared ledger yang diterapkan pada blockchain. Setiap stakeholder (pemangku kepentingan) akan memiliki salinan dari setiap kejadian yang tercatat, termasuk perubahan-perubahan yang terjadi pada data tersebut.

### Tips Dokumentasi Data

* Gunakan Alur Ilmiah yang Terstruktur
* Informasi Harus Jelas dan Sedetail Mungkin

## Bercerita dengan Data

### Exploratory vs Explanatory

Dalam presentasi atau penyampaian hasil visualisasi, Anda harus dapat membedakan cara penyampaian antara exploratory analysis atau explanatory analysis.

Exploratory berasal dari kata explore yang berarti jelajahi, sehingga exploratory analysis adalah proses penyampaian di mana Anda membimbing dan memandu audiens dalam melihat (menjelajahi) data yang telah dikumpulkan.

Sedangkan explanatory berasal dari explain yang berarti menjelaskan, sehingga explanatory analysis adalah proses penyampaian di mana Anda tidak meminta audiens untuk menjelajahi data namun langsung ke poin-poin utama dan implikasi dari data tersebut.

Mungkin Anda tergoda untuk melakukan exploratory analysis karena dapat menunjukkan betapa banyaknya data yang telah dikumpulkan dan seberapa besar kerja keras yang dilakukan. Namun harus dimengerti bahwa mayoritas orang bosan dengan cerita presentasi yang bertele-tele. Jika kita bandingkan sebagai sebuah cerita melihat tari kecak di Bali, exploratory analysis adalah bagian di mana tokoh mempersiapkan barang-barang yang dibutuhkan dan proses untuk sampai ke Bali, sedangkan explanatory analysis adalah cerita saat melihat tari kecaknya.

### Kepada siapa kita berkomunikasi?

Hal ini sangat penting agar kita paham bagaimana mengomunikasikan hasil yang didapatkan. Tergantung siapa lawan bicara atau audiens, kita bisa memilih bagaimana berbicara dan bertindak saat menyampaikan informasi. Sebagai contoh, cara bicara kepada teman ataupun orang tua itu beda kan? Terdapat dua cara pandang yang dibutuhkan untuk dapat melakukan komunikasi yang efektif.

**Melihat dari sisi audiens**
Semakin spesifik kita tahu siapa audiens kita, semakin besar potensi komunikasi kita sukses. Sehingga kita harus menghindari penyampaian data yang terlalu umum. Kita juga perlu mengetahui kebutuhan informasi seperti apa yang ingin diketahui audiens. Berkomunikasi dengan terlalu banyak orang pada saat sama sekaligus, cenderung tidak tepat sasaran karena kebutuhan masing-masing orang dapat berbeda. Ini justru membuat kita kurang efektif dalam usaha untuk penyampaian informasi. Persempit target audiens, maka hasilnya akan lebih efektif.

**Melihat dari sisi diri sendiri**
Penting kita mengetahui hubungan kita dengan audiens, apakah mereka sudah mengenal kita? Apakah mereka menganggap kita sebagai ahli dan setiap hal yang kita sampaikan bisa dipercaya? Ini merupakan sebuah acuan untuk menyusun cara komunikasi kita, hal yang disampaikan, dan kapan harus menggunakan data. Hal ini dapat memengaruhi alur keseluruhan cerita yang ingin kita sampaikan. Jika Anda sebelumnya tidak pernah bertemu dengan audiens, berarti Anda terlebih dahulu harus membangun reputasi bahwa Anda itu benar-benar mengerti topik yang akan diberikan. Biasanya hal ini dilakukan dengan cara perkenalan diri.

### Bagaimana kita berkomunikasi dengan audiens?

**Alat**
Metode alat yang kita gunakan untuk berkomunikasi dengan audiens memiliki peran penting dalam sejumlah faktor, termasuk jumlah kontrol yang kita miliki atas bagaimana audiens memperoleh informasi dan tingkat detail yang perlu lebih dijelaskan.

Pada proses presentasi secara langsung dan tatap muka, kita dapat menanggapi audiens jika terdapat hal yang kurang jelas. Tidak semua yang kita sampaikan harus ditulis secara detail pada dokumen presentasi dan visualisasi data karena kita ada di sana untuk menjelaskan dan menjawab setiap pertanyaan yang muncul selama presentasi.

Lain halnya ketika hanya menuliskan hasil analisis dalam bentuk dokumen yang dibaca sendiri-sendiri. Jika pada presentasi langsung kita dapat mengendalikan audiens yang kurang paham, maka hal tersebut tidak efektif jika kita tidak ada di sana untuk menanggapi atau melihat ekspresi kebingungan audiens saat menemui bagian yang kurang jelas. Sehingga tingkat detail yang diperlukan pada penulisan dokumen biasanya lebih tinggi.

**Pembawaan Diri**
Pertimbangan penting lainnya adalah nada penyampaian pada audiens. Apakah kita ingin menyampaikannya dengan ceria, memotivasi, atau serius? Nada yang kita inginkan untuk komunikasi juga akan memiliki pengaruh pada pilihan desain yang akan digunakan untuk membuat proses visualisasi data. Selain itu, pernahkah kita berpikir bahwa audiens bisa lebih tahu daripada kita? Terkadang asumsi tersebut muncul. Tapi sebaiknya hapus pemikiran seperti itu. Jika kita adalah orang yang menganalisis dan mengomunikasikan data, maka kita harus percaya diri. Bahkan kita dapat melakukan interaksi dengan audiens untuk meningkatkan keterlibatan mereka atau mengurangi rasa gugup kita saat menyampaikan data tersebut.

### Bagaimana kita bisa menggunakan data untuk membantu menegaskan maksud kita?

Setelah kita menjawab pertanyaan di atas, barulah kita membahas data apa yang akan membantu menegaskan dan mendukung inti cerita atau kesimpulan yang ingin disampaikan. Salah satu cara yang dapat dilakukan adalah menggunakan metode 5W (What, Who, When, Why, Where). Gunakan data yang telah didapatkan untuk menjawab unsur dari 5W sehingga dapat menegaskan informasi penting yang ingin kita sampaikan.