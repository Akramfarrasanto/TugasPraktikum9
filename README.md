#  praktikum-9

Exception Handing

```
- Exception Adalah suatu kesalahan atau error yang terjadi saat proses eksekusi perogram yang sedang berjalan;
- Kesalahan ini Biasanya disebabkan Karena Salah satu Programnya ada Masalah atau tidak terdetek.
```

Assertion

```
- Assertion(Pernyataan) merupakan kewajaran suatu proram yang kamu bisa aktif atau nonaktif ketika kamu selesai menjalankan sebuah program
```

Assert Expression (Arguments)

```
- Jika pernyataan gagal, Python menggunakan ArgumentExpression ArgumentExpression sebagai argumen argumen untuk AssertionError AssertionError. Pengecualian AssertionError Pengecualian AssertionError dapat ditangkap dan ditangani ditangani seperti pengecualian lainnya menggunakan try- kecuali pernyataan, tetapi jika dibiarkan, mereka akan menghentikan program dan menghasilkan backtrace.
```

Contoh kode di bawah menghasilkan hasil sebagai berikut:
![gambar1](https://user-images.githubusercontent.com/115552876/208419972-6dc25672-db3f-45c4-b8a3-40bcf78c1a77.jpeg)

Menangani Pengecualian

```
Jika Anda memiliki beberapa kode mencurigakan yang mungkin mengeluarkan pengecualian, Anda dapat mempertahankan program Anda letakkan kode yang mencurigakan di *try: blok. Setelah coba: blok, sertakan pernyataan sertakan *except: statemen, diikuti oleh blok kode yang menangani masalah seanggun mungkin.
```

Contoh kode di bawah menghasilkan hasil sebagai berikut:
![gambar2](https://user-images.githubusercontent.com/115552876/208420079-59426106-2c12-4a23-9921-9f5b40338167.jpeg)

![gambar3](https://user-images.githubusercontent.com/115552876/208420218-ca91a387-3276-491f-bb53-bf6dd818375f.jpeg)

Fasal Kecuali tanpa pengecualian

```
- Anda juga dapat menggunakan pernyataan exception tanpa exception yang didefinisikan sebagai berikut:
try: You do your operations here; ...................... except: If there is any exception, then execute this block. ...................... else: If there is no exception then execute this block.

Pernyataan coba-kecuali jenis ini menangkap semua pengecualian pengecualian yang terjadi. Menggunakan percobaan seperti try-expect pernyataan tidak dianggap sebagai praktik pemrograman yang baik, karena mereka menangkap semuanya pengecualian tetapi tidak membuat programmer mengidentifikasi kemungkinan penyebab masalah terjadi.
```

Kalau kecuali dengan berbagai pengecualian

```
- Anda juga dapat menggunakan pernyataan exception yang sama untuk menangani beberapa exception sebagai berikut:
try: You do your operations here; ...................... except(Exception1[, Exception2[,...ExceptionN]]]): If there is any exception from the given exception list, then execute this block. ...................... else: If there is no exception then execute this block.
```

kalau coba-akhirnya

contoh:
- Jika Anda memiliki izin untuk membuat file dalam mode tulis yang dapat ditulis, maka ini akan menghasilkan hasil berikut:
![gambar4](https://user-images.githubusercontent.com/115552876/208420350-6e05ddd2-be3a-401b-a579-7b8a5490b941.jpeg)

- Contoh yang sama dapat ditulis lebih bersih sebagai berikut:
![gambar5](https://user-images.githubusercontent.com/115552876/208420471-953b44e0-eebb-49d8-852a-8a41bb327662.jpeg)

Ketika exception dilempar ke dalam blok try, eksekusi segera dilanjutkan ke akhir memblok. Setelah semua pernyataan di blok akhirnya dieksekusi, pengecualian dimunculkan lagi dan ditangani dalam pernyataan kecuali jika ada di lapisan berikutnya yang lebih tinggi dari percobaan-kecuali penyataan.

Argumen Pengecualian

- berikut adalah contoh untuk satu pengecualian:
![gambar6](https://user-images.githubusercontent.com/115552876/208420558-9614db04-0310-4585-88a8-5dea01a97380.jpeg)


Melempar Pengecualian 

- Pengecualian dapat berupa string, kelas, atau objek. Sebagian besar pengecualian adalah pengecualian dari inti Python menimbulkan adalah kelas, dengan argumen=argumen yang merupakan turunan dari kelas. Mendefinisikan pengecualian barucukup mudah dan dapat dilakukan sebagai berikut:
![gambar7](https://user-images.githubusercontent.com/115552876/208420782-439df0ee-3184-43e8-a00d-327a3706dd71.jpeg)


Pengecualian yang ditetapkan pengguna

- Python juga memungkinkan Anda membuat pengecualian sendiri dengan menurunkan kelas-kelas dari yang standar pengecualian bawaan;
- Berikut adalah contoh-contoh yang terkait dengan RuntimeError. Di sini, kelas dibuat yang merupakan subkelas dari subkelas RuntimeError. Ini berguna saat Anda perlumenampilkan tampilan informasi yang lebih spesifik saat e pengecualian tertangkap;
- Di blok coba, pengecualian yang ditentukan pengguna dimunculkan dan ditangkap di blok kecuali. Itu variabel e digunakan untuk membuat instance dari kelas Networkerror.
![gambar8](https://user-images.githubusercontent.com/115552876/208420913-9ebab4c9-02c2-445f-8367-466657b359f5.jpeg)

