Nama: Kristin HAndayani Sihombing
NIM:41426025
Prodi:D4 TRPL

Pada praktikum kali ini, saya belajar tentang penggunaan variabel, tipe data, percabangan, dan perulangan pada JavaScript. Selain itu, saya juga belajar bagaimana cara mengubah tipe data, memeriksa suatu kondisi, dan menampilkan beberapa data menggunakan perulangan.

2. <File dan Console
Tujuan:
Mengetahui cara menjalankan JavaScript dan melihat hasilnya melalui Console pada browser.
Kode program:

<console.log("Hello JavaScript!");

Penjelasan:
Pada percobaan pertama, saya mencoba membuat kode JavaScript sederhana menggunakan console.log(). Perintah ini digunakan untuk menampilkan tulisan ke dalam Console browser.
Sebelum menjalankan kode, saya menghubungkan file JavaScript dengan HTML menggunakan tag script dan atribut defer. Setelah itu, saya membuka halaman melalui Live Server dan melihat hasilnya di bagian Console.

Hasil:
MAin js telah dihubungkan!
Kesimpulan:
Dari percobaan ini, saya mengetahui cara menghubungkan JavaScript dengan HTML. Saya juga belajar bahwa console.log() bisa digunakan untuk melihat hasil dari kode yang saya buat.

1. <Konversi Data
Tujuan:
Mengetahui perbedaan tipe data string dan number serta cara mengubah string menjadi angka.
Kode program:

<const teks = "2";
console.log(teks + 1);
console.log(Number(teks) + 1);

<Penjelasan setiap kode:
- const = membuat variabel.
- teks = nama variabel.
- "2" = angka 2 yang dianggap sebagai teks karena berada di dalam tanda petik.
- console.log() = menampilkan hasil ke Console.
- teks + 1 = menggabungkan teks dengan angka.
- Number(teks) = mengubah teks menjadi angka.
- Number(teks) + 1 = menjumlahkan angka 2 dengan angka 1.
-console.log(typeof teks);
-console.log(typeof Number(teks));

<Pengamatan typeof
typeof teks menghasilkan string karena "2" adalah teks.
typeof Number(teks) menghasilkan number karena sudah diubah menjadi angka.

<Uji Number("abc") dan Number.isFinite>
const hasil = Number("abc");
console.log(hasil);
console.log(Number.isFinite(hasil));

Number("abc") mencoba mengubah teks "abc" menjadi angka.
Krena "abc" bukan angka yang valid, hasilnya adalah NaN.
<NaN berarti Not a Number.

Number.isFinite(hasil) digunakan untuk memeriksa apakah nilai merupakan angka yang valid dan terbatas.
Hasil false berarti nilai tersebut bukan angka terbatas yang valid.

<string kosong>
console.log(Number(""));
console.log(Number(" "));
console.log(Number.isFinite(Number("")));

Kesimpulan percobaan saya:
<Pada percobaan kedua, saya membuat variabel bernama teks yang berisi angka 2. Namun, karena angka tersebut menggunakan tanda petik, JavaScript membacanya sebagai string atau teks.
Ketika saya menjalankan teks + 1, hasilnya adalah 21 karena angka 2 dan 1 digabungkan menjadi satu teks.
Sedangkan ketika menggunakan Number(teks) + 1, hasilnya menjadi 3 karena nilai teks tadi diubah terlebih dahulu menjadi angka.
Saya juga mencoba typeof untuk mengetahui jenis data yang digunakan. Kemudian, saya mencoba Number("abc") dan hasilnya adalah NaN karena tulisan abc tidak bisa diubah menjadi angka. Fungsi Number.isFinite() digunakan untuk memeriksa apakah hasilnya merupakan angka yang valid.

<Hasil pengujian:

Perintah: teks + 1
Hasil:21
Perintah:Number(teks) + 1
HAsil:3
Perintah:typeof teks
Hasil:string
Perintah:typeof Number(teks)
HAsil:number
Perintah:Number("abc")
hasil:NaN
peintah:Number.isFinite(Number("abc"))
Hasil:false
<Kesimpulan:
Dari percobaan ini, saya memahami bahwa string dan number memiliki fungsi yang berbeda. Walaupun string berisi angka, JavaScript tetap membacanya sebagai teks. Jadi, jika ingin melakukan perhitungan, saya harus mengubahnya terlebih dahulu menggunakan Number(). Saya juga mengetahui bahwa NaN muncul ketika suatu nilai tidak bisa menghasilkan angka yang valid.

4. Aturan Jumlah Tiket
Tujuan:
Membuat program untuk memeriksa jumlah tiket yang boleh dibeli, yaitu minimal 1 dan maksimal 5 tiket.
Kode program:

<const jumlah = Number("3");
if (!Number.isInteger(jumlah) || jumlah < 1 || jumlah > 5) {
    console.log("Jumlah tidak valid");
} else {
    console.log(jumlah * 10000);
}

<const jumlah = Number("3");>
Artinya:
- const digunakan untuk membuat variabel.
- jumlah adalah nama variabel.
- = digunakan untuk memberikan nilai.
- Number("3") mengubah teks "3" menjadi angka 3.
if digunakan untuk membuat kondisi atau pemeriksaan.

Penjelasan pada kode 2:
!Number.isInteger(jumlah)
   
   Memeriksa apakah jumlah bukan bilangan bulat.
   - 3 = bilangan bulat.
   - 2.5 = bukan bilangan bulat.
   Tanda ! berarti TIDAK.
 jumlah < 1
   
   Memeriksa apakah jumlah kurang dari 1.
jumlah > 5
   Memeriksa apakah jumlah lebih dari 5.
Tanda || artinya ATAU. Jadi, jika salah satu kondisi benar, jumlah dinyatakan tidak valid.
Penjelasan:
Pada percobaan ketiga, saya membuat variabel jumlah untuk menyimpan jumlah tiket. Nilai tersebut diubah menjadi angka menggunakan Number().
Selanjutnya, saya menggunakan if dan else untuk memeriksa apakah jumlah tiket sudah sesuai dengan ketentuan.
Bagian Number.isInteger(jumlah) digunakan untuk memeriksa apakah jumlah tiket merupakan bilangan bulat. Tanda ! berarti tidak, sedangkan || berarti atau.
Kemudian, jumlah < 1 digunakan untuk memeriksa apakah jumlah kurang dari 1 dan jumlah > 5 digunakan untuk memeriksa apakah jumlah lebih dari 5.
Jika jumlah tidak sesuai dengan ketentuan, program akan menampilkan pesan bahwa jumlah tidak valid. Tetapi jika jumlahnya sesuai, program akan menghitung harga tiket dengan mengalikan jumlah tiket dengan 10.000.

Hasil pengujian:
Input  Hasil

0      Jumlah tidak valid
1      10000
5      50000
6      Jumlah tidak valid
1.5    Jumlah tidak valid
abc    Jumlah tidak valid

<Kesimpulan:
Dari percobaan ini, saya belajar menggunakan if dan else untuk menentukan apakah suatu nilai bisa diterima atau tidak. Saya juga memahami bahwa sebelum melakukan perhitungan, input harus diperiksa terlebih dahulu supaya program tidak menerima jumlah tiket yang tidak sesuai dengan aturan.

5. <Loop Koleksi
Tujuan:
Menampilkan beberapa data yang ada di dalam array menggunakan perulangan for...of.
Kode program:

<const judul = ["HTML", "CSS", "Audit"];
for (const item of judul) {
    console.log(item);
}

Penjelasan:
Pada percobaan keempat, saya membuat sebuah array bernama judul yang berisi tiga data, yaitu HTML, CSS, dan Audit.
Setelah itu, saya menggunakan perulangan <for...of> untuk mengambil data satu per satu dari dalam array.
Variabel item digunakan untuk menyimpan data yang sedang dibaca. Kemudian, console.log(item) digunakan untuk menampilkan data tersebut ke Console.
Perulangan akan terus berjalan sampai semua data di dalam array selesai ditampilkan. Jadi, saya tidak perlu menulis console.log() satu per satu untuk setiap data.

Hasil:
HTML
CSS
Audit

<Pengujian tambahan:
Saya juga mencoba beberapa kondisi lain, yaitu menggunakan array kosong dan menambahkan satu data baru ke dalam array.
Jika array kosong, tidak ada data yang ditampilkan.
Jika terdapat tiga data, maka akan muncul tiga keluaran.
Jika ditambahkan satu data lagi, maka akan muncul empat keluaran.

<Format laporan>

1. Percobaan Konversi Data
Kasus Normal
Saya mencoba menjalankan kode "2" + 1. Hasil yang muncul adalah 21 karena angka 2 masih berbentuk string sehingga digabungkan dengan angka 1.
Kasus Batas
Saya mencoba menggunakan Number("") untuk mengubah string kosong menjadi angka. Hasil yang muncul adalah 0 karena JavaScript menganggap string kosong sebagai angka 0 ketika dikonversi menggunakan Number().
Kasus Gagal
Saya mencoba memasukkan teks "abc" menggunakan Number("abc"). Hasil yang muncul adalah NaN karena teks tersebut tidak dapat diubah menjadi angka yang valid.
2. Percobaan Aturan Jumlah Tiket
Kasus Normal
Saya mencoba memasukkan jumlah tiket sebanyak 3. Hasil yang muncul adalah 30000 karena jumlah tiket dikalikan dengan harga Rp10.000.
Kasus Batas
Saya mencoba memasukkan jumlah tiket paling sedikit, yaitu 1, dan paling banyak, yaitu 5. Hasilnya masing-masing adalah 10000 dan 50000. Kedua jumlah tersebut masih diterima oleh program.
Kasus Gagal
Saya mencoba memasukkan jumlah tiket 0, 6, 1.5, dan abc. Hasil yang muncul adalah pesan "Jumlah tidak valid" karena input tersebut tidak memenuhi ketentuan program.
3. Percobaan Loop Koleksi
Kasus Normal
Saya mencoba membuat array yang berisi tiga data, yaitu HTML, CSS, dan Audit. Setelah menjalankan perulangan for...of, ketiga data berhasil ditampilkan satu per satu di Console.
Kasus Batas
Saya mencoba menggunakan array kosong tanpa memasukkan data apa pun. Hasilnya tidak ada keluaran yang muncul karena tidak terdapat data yang dapat dibaca oleh perulangan.
Kasus Gagal
Saya mencoba memasukkan data dengan tipe yang berbeda, seperti teks dan angka, ke dalam array. Hasilnya semua data tetap dapat ditampilkan karena for...of dapat membaca setiap elemen array tanpa mengharuskan semua elemen memiliki tipe data yang sama.
4. Percobaan File dan Console
Kasus Normal
Saya menjalankan kode console.log("Hello JavaScript!"). Hasilnya tulisan Hello JavaScript! berhasil muncul di Console browser.
Kasus Batas
Saya mencoba menjalankan console.log("") dengan isi teks kosong. Hasilnya tidak ada tulisan yang terlihat di Console karena tidak ada teks yang ditampilkan.
Kasus Gagal
Saya mencoba menjalankan kode dengan tanda kurung yang tidak lengkap. Hasilnya muncul pesan SyntaxError karena penulisan kode tidak sesuai dengan aturan JavaScript.

<Kesimpulan:
Dari percobaan ini, saya memahami bahwa array bisa digunakan untuk menyimpan banyak data dalam satu variabel. Dengan menggunakan for...of, saya bisa menampilkan semua data secara berurutan tanpa harus menuliskan perintah yang sama berulang kali.

6. Kesimpulan Keseluruhan
Setelah mengerjakan praktikum ini, saya mulai memahami beberapa dasar penggunaan JavaScript, seperti variabel, tipe data, percabangan, dan perulangan.
Awalnya saya masih bingung membedakan string dan number, terutama ketika melakukan penjumlahan. Setelah mencoba menggunakan Number(), saya jadi mengetahui bahwa data yang berbentuk teks harus diubah terlebih dahulu jika ingin digunakan untuk perhitungan.
Menurut saya, praktikum ini membantu saya lebih memahami bagaimana JavaScript bekerja karena saya tidak hanya menulis kode, tetapi juga mencoba beberapa input dan melihat hasilnya secara langsung.

7. AI Use Statement
Dalam mengerjakan praktikum ini, saya menggunakan ChatGPT untuk membantu memahami beberapa materi JavaScript yang masih belum saya pahami dan membantu menjelaskan fungsi dari kode yang digunakan.
Penjelasan yang diperoleh saya pelajari kembali, kemudian kode saya jalankan menggunakan Visual Studio Code dan browser untuk memastikan hasilnya sesuai dengan yang diharapkan.#   p s w i - w e e k 0 7 - s e s i 0 3 _  
 