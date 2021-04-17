# Pengenalan Formula pada Spreadsheet

Formula merupakan sebuah langkah atau rumus untuk melakukan perhitungan matematis sehingga mendapatkan nilai tertentu. Istilah formula sendiri sudah sangat umum ditemui dalam aplikasi spreadsheet seperti Microsoft Excel, LibreOffice Calc, dan Google Spreadsheet.

## Operator

Operator adalah simbol atau tanda yang memiliki fungsi tertentu dan digunakan untuk melakukan pemrosesan atau perhitungan data.

Penggunaan operator matematika erat kaitannya dengan perhitungan entah itu penjumlahan, pengurangan, dan lainnya. Begitu pula dengan perhitungan dalam Google Spreadsheet, operator selalu digunakan dalam penulisan rumus. 

Penggunaan operator dalam spreadsheet baik itu Microsoft Excel, Google Spreadsheet, maupun lainnya, mengikuti aturan urutan umum perhitungan matematika. Misalnya operator perkalian dan pembagian akan berjalan lebih dulu. Baru setelahnya operator penjumlahan dan pengurangan. Setiap penulisan formula dalam spreadsheet pun pasti diawali dengan tanda “=” . 

### Operator Aritmatika

| Operator | Kegunaan |
|:--------:|----------|
| + | Penjumlahan |
| - | Pengurangan |
| / | Pembagian |
| * | Perkalian |
| ^ | Pangkat |
| % | Persen atau modulus |

### Operator Perbandingan

Dalam spreadsheet biasanya kita menggunakan jenis operator perbandingan untuk fungsi-fungsi logika seperti IF, OR, AND, dan NOT. Hasilnya adalah kondisi nilai True atau False. Contohnya sebagai berikut:

| Operator | Kegunaan |
|:--------:|----------|
| = | Sama dengan ... |
| > | Lebih dari ... |
| >= | Lebih dari atau sama dengan ... |
| <= | Kurang dari atau sama dengan ... |
| <> | Tidak sama dengan ... |

[How to use AND and OR in google sheet](https://www.howtogeek.com/447561/how-to-use-the-and-and-or-functions-in-google-sheets/)

### Operator Text

Operator text yang dimaksud adalah ampersand (“&”) yang berfungsi untuk menggabungkan beberapa string text menjadi satu string tunggal. Ia biasanya menggunakan formula Concatenate.

### Operator Referensi

Operator referensi dalam spreadsheet berguna untuk menunjukkan lokasi sel yang digunakan dalam penerapan sebuah rumus atau range data. Berikut macam-macam operator referensi yang sering digunakan dalam spreadsheet:

| Operator | Kegunaan |
|:--------:|----------|
| “:” (Titik dua) | Biasa disebut dengan operator range yang berfungsi untuk menghasilkan satu referensi ke semua sel yang ada di antara dua referensi. Misalnya, sel A1:A10 artinya data terpilih adalah A1, A2, A3, A4, … , A10. |
| “;” (titik koma/semicolon) | Disebut juga dengan operator union yang berfungsi untuk menggabungkan beberapa referensi rentang sel menjadi satu. Misalnya, A1:A3;B3:B6;A4. Referensi sel tidak harus rentang data tetapi bisa menggunakan sel tunggal juga. |
| “ “ (Spasi) | Bisa disebut juga dengan operator titik potong yang berfungsi untuk menunjukkan irisan dari dua referensi sel. Misalnya A1:A5 A1:C3. Sehingga titik temu referensi tersebut ada di sel A1. A1 rentang datanya sampai A5 dan juga C3. |

## Elemen Formula

Penulisan formula dalam spreadsheet diawali dengan tanda sama dengan “=”. Sedangkan bagian-bagian dalam sebuah formula dapat terdiri dari satu atau lebih elemen berikut:

* Fungsi
* Referensi sel (single/range)
* Operator
* Konstanta

### Sama dengan (“=”)

Tanda sama dengan “=” merupakan elemen yang paling awal ditulis dalam sebuah formula apa pun sebelum lanjut ke elemen lainnya.

### Fungsi

Fungsi merupakan sebuah penamaan yang telah ditentukan untuk melakukan kalkulasi data berdasarkan susunan argumen dalam aplikasi spreadsheet. Misal, kita ingin menghitung rata-rata menggunakan fungsi AVERAGE, total data menggunakan fungsi SUM.

### Referensi Sel

Sebuah formula pasti merujuk pada sebuah alamat sel tertentu, rujukan alamat bisa disebut dengan referensi sel.

Dengan menggabungkan operator matematika dengan referensi sel, Anda dapat menerapkannya di rumus matematika dalam Google Spreadsheet.

### Operator

Operator juga termasuk salah satu elemen dalam penulisan formula spreadsheet.

### Konstanta

Konstanta merupakan nilai masukan yang bukan berasal dari perhitungan karena nilainya selalu sama dan tidak pernah berubah. Bentuk dari konstanta bisa berupa teks atau angka, misalnya dalam contoh di atas konstanta ditunjukkan dengan angka 2.

## Fungsi

### SUM

Kita sering menemui rumus ini dalam spreadsheet. Rumus SUM dapat membantu untuk mendapatkan nilai total dari rentang sel yang dipilih. Penggunaannya dengan cara menyorot semua baris atau kolom yang ingin diketahui jumlahnya. Penulisannya sebagai berikut:

~~~
=SUM(data ke-1, data ke-2, …. , data ke-n) 
~~~

### SUMIF

Selanjutnya kita membahas fungsi SUMIF. Fungsi ini berbeda dari SUM yang biasa karena SUMIF ini berfungsi untuk menjumlahkan data dengan kriteria tertentu. Penulisan fungsi dari SUMIF sebagai berikut:

~~~
=SUMIF(range,”kriteria”,sum_range)
~~~

### SUMIFS

Apabila SUMIF hanya bisa menggunakan satu kriteria saja, pada SUMIFS kita bisa menggunakan lebih dari satu kriteria. Penulisannya sebagai berikut:

~~~
=SUMIFS(sum_range, kriteria_range1, “kriteria1”, kriteria_range2, “kriteria2”, dan seterusnya)
~~~

### AVERAGE

Masih ingatkah Anda dengan rata-rata aritmatika? Fungsi AVERAGE sama dengan rata-rata aritmatika yang menjumlahkan semua data kemudian dibagi dengan jumlah data yang ada. Penggunaannya hampir sama dengan rumus SUM yaitu sebagai berikut:

~~~
=AVERAGE(data ke-1, data ke-2, … , data ke-n)
~~~

### COUNT

Count merupakan fungsi yang dapat menghitung banyaknya sel terpilih dalam rentang tertentu yang berisi nilai numerik. Penggunaan fungsi COUNT sebagai berikut:

~~~
=COUNT(data ke-1, data ke-2, … , data ke-n)
~~~

### COUNTA

Sama seperti COUNT, COUNTA dapat menghitung jumlah sel terpilih dalam rentang tertentu. Namun bedanya dalam COUNTA kita dapat menghitung semua sel yang terpilih, tak peduli apa pun jenis data yang ada di dalamnya (angka, teks, tanggal, kondisi benar atau salah, hingga kesalahan perhitungan). Tetapi terdapat satu yang dilewati dalam perhitungan COUNTA yaitu sel yang kosong. Penggunaan rumus COUNTA sebagai berikut:

~~~
=COUNTA(data ke-1, data ke-2, … , data ke-n)
~~~

### COUNTIF dan COUNTIFS

COUNTIF sering digunakan untuk menghitung banyaknya data pada kumpulan sel dengan kriteria tertentu. Sistematika penulisannya sebagai berikut:

~~~
=COUNTIF(range,kriteria)
~~~

* Range : Data COUNTIF yang dihitung.
* Kriteria : Kondisi tertentu yang diinginkan untuk diketahui. Bisa berisi teks, operasi logika, ataupun angka.

Sedangkan COUNTIFS berfungsi untuk menghitung banyaknya data pada kumpulan sel berdasarkan kriteria (lebih dari satu). Sistematika penulisannya sebagai berikut:

~~~
=COUNTIFS(kriteria_range1,kriteria1, kriteria_range2, kriteria2, dan seterusnya)
~~~

* Kriteria_range1 : range pertama yang dihitung jumlah datanya.
* Kriteria1 adalah kondisi tertentu yang diinginkan untuk diketahui.
* Kriteria_range2,kriteria2 adalah kriteria atau kondisi berikutnya yang ingin diketahui.

### Min dan Max

Kedua fungsi ini berguna untuk menentukan nilai terendah (MIN) dan tertinggi (MAX) dari suatu rentang data yang terpilih. Contoh penggunaan rumus min max seperti berikut:

~~~
=MIN(data ke-1, data ke-2, …, data ke-n)

=MAX(data ke-1, data ke-2, …, data ke-n)
~~~

### Trim

Selanjutnya fungsi TRIM digunakan untuk menghilangkan ruang kosong yang tidak dibutuhkan pada sebuah teks. Fungsi ini hanya berjalan pada sel tunggal bukan pada rentang sel. Penggunaan rumusnya adalah sebagai berikut:

~~~
=TRIM(teks)
~~~

### Replace

Selanjutnya terdapat fungsi Replace. Tahukah Anda apakah fungsi Replace dalam spreadsheet? Replace dapat digunakan untuk mengganti string baik berupa angka maupun teks biasa. Sistematika penulisan Replace sebagai berikut:

~~~
=REPLACE(text, position, length, new_text)
~~~

* Text, Dapat diisi dengan teks secara langsung atau alamat sel.
* Position, Posisi atau urutan dari huruf yang ingin diganti.
* Length, Panjang karakter yang ingin kita ganti.
* New_text, Teks baru yang ingin kita gunakan untuk mengganti teks lama, bisa berupa angka atau huruf.

### Unique

Unique merupakan sebuah fungsi yang dapat kita gunakan untuk mencari data yang unik dari sebuah data yang mungkin saja ada yang sama. Sistematika penulisannya sebagai berikut:

~~~
=UNIQUE(range)
~~~

### IF

Fungsi IF digunakan untuk membuat perbandingan logis antara sebuah data dengan kondisi penguji yang yang diberikan. Penggunaannya sebagai berikut:

~~~
=IF(Sel yang ingin diuji, [nilai jika benar], [nilai jika salah])
~~~

[Nested IF](https://www.howtogeek.com/449861/how-to-use-the-google-sheets-if-function/)

>NOTE
>>Jika Anda mencoba menerapkan rumus misalnya seperti =SUMIF(range,”kriteria”,sum_range) dan terjadi error atau tidak dapat terbaca di Excel atau Spreadsheet, maka gunakan tanda titik koma (;) sehingga menjadi =SUMIF(range;”kriteria”;sum_range). Hal tersebut disebabkan pengaturan delimiter dari setiap komputer terkadang berbeda-beda.