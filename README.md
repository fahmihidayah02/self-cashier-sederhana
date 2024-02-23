# self-cashier-sederhana
# Latar Belakang Masalah
Andi adalah seorang pemilik supermarket. Beliau ingin memperbaiki proses bisnis di supermarket miliknya, yaitu dengan membuat sistem kasir self-service agar customer bisa langsung menginputkan barang yang dibelinya saat ingin melakukan pembayaran secara mandiri. Hal ini dilakukan agar customer yang berada di luar kota juga bisa membeli barang dari supermarket tersebut.
Untuk memecahkan masalah tersebut adalah dengan membuat program Cashier Self-Service untuk memperbaiki proses bisnis di supermarket milik Andi.

# Objective
Tujuan dari pembuatan projek ini adalah membuat sistem kasir self-service yang dapat melakukan beberapa metode yaitu:

1.	Customer dapat menginput barang, jumlah barang, dan juga harga barang dengan metode `tambah_barang()`.

2.	Jika customer salah input, ia dapat mengubah salah satu inputanya:

    •	mengubah nama barang dengan metode `update_nama_barang()`.
  	
    •	mengubah jumlah barang dengan metode `update_jumlah_barang()`.
  	
    •	mengubah harga barang dengan metode `update_harga_barang()`.

4.	Jika customer ingin menghapus salah satu barang dari daftar barang belanjanya, dapat menggunakan metode `hapus_barang()`.

5.	Jika customer ingin menghapus semua barang dari daftar belanjanya, dapat menggunakan metode `reset_transaction()`


6.	Sebelum dapat menghitung total belanjanya, isi dari daftar belanja customer dicek dulu dengan metode `cek_order()`. Metode ini mengecek apakah ada inputan yang masih salah pada daftar barang belanja customer.

7.	Sistem dapat menghitung semua total belanja dan juga diskon yang didapatkannya dengan metode `total_belanja()`.

8.	Ketentuan untuk memperoleh diskon:

    •	Jika total belanja diatas **Rp.500.000**, maka diskon **10%**
  	
    •	Jika total belanja diatas **Rp.300.000**, maka diskon **8%**
  	
    •	Jika total belanja diatas **Rp.200.000**, maka diskon **5%**

# Method yang digunakan

1.	`Transcaction()`
   
    Membuat kelas transaksi untuk menghimpun data transaksi dan membuat fungsi/method sehingga menghasilkan objek

2.	`tambah_barang()` (self, nama_barang, jumlah_barang, harga_barang)
   
  	Metode ini digunakan untuk memasukkan barang ke daftar barang belanja.

3.	`update_nama_barang()` (self, nama_barang, nama_barang_baru)

  	Metode ini digunakan untuk merubah nama barang yang sudah ada dalam daftar barang belanja.

4.	`update_jumlah_barang()` (self, nama_barang, jumlah_barang_baru)

  	Metode ini digunakan untuk merubah jumlah barang berdasarkan nama barang yang ada didalam daftar barang belanja.

5.	`update_harga_barang()` (self,nama_barang,jumlah_barang_baru)

  	Metode ini digunakan untuk merubah harga barang berdasarkan nama barang yang ada didalam daftar barang belanja.

6.	`hapus_barang()` (self,nama_barang)

  	Metode ini digunakan untuk menghapus salah satu barang yang diinginkan berdasarkan nama barang yang ada didalam     `daftar barang belanja

7.	`reset_transaction()`

   	Metode ini digunakan untuk menghapus semua barang didalam daftar barang belanjaan.

8.	`cek_order()`

   	Metode ini digunakan untuk memastikan data yang diinputkan sudah benar atau belum.

9.	`total_belanja()`

   	Metode ini digunakan untuk menghitung total harga dari daftar barang belanja customer.

# FLOWCHART
<p>
<img align="center" src="flowchart.jpg" width="800" height="1200" />
</p>

# ALUR PROGRAM
1.	Customer membuat ID transaksi dengan membuat objek dari class trnsct_123 = Transaction()
   
2.	Customer memasukkan nama barang, jumlah, barang, dan harga barang
   
3.	kemudian dicek apakah ada kesalahan inputan, jika ada kesalahan inputan tapi tidak ingin menghapus barangnya,maka customer dapat melakukan salah satu dari method dibawah:
  	
        o	update nama barang dengan method update_nama_barang()
  	
        o	update jumlah barang dengan method update_jumlah_barang()
  	
        o	update harga barang dengan method update_harga_barang()
  	
4.	Jika customer ingin membatalkan salah satu barang, customer dapat menghapus salah satu barang dengan method
hapus_barang, ketika menghapus salah satu item maka jumlah barang dan harga barang ikut terhapus.

6.	Jika customer ingin menghapus semua barang di daftar barang, yaitu menggunakan method reset_transaction()
   
7.	Apabila customer sudah selesai belanja online, tapi masih ragu apakah inputannya sudah benar atau belum, maka
customer dapat menggunakan method cek_order dan mengeluarkan pesan "pemesanan sudah benar" jika tidak ada kesalahan input. Jika ada kesalahan input maka mengeluarkan pesan "terdapat kesalahan input data.
  	
8.	Setelah melakukan pengecekan, customer dapat menghitung total belanja dengan method total_belanja() dengan           ketentuan:
   
        o	jika total belanja > 500_000 maka dapat diskon 10%
  	
        o	jika total belanja > 300_000 maka dapat diskon 8%
  	
        o	jika total belanja > 200_000 maka dapat diskon 5%

# TEST CASE
# TEST 1
Customer ingin menambahkan dua 4 barang baru dengan method tambah_barang(). Barang yang diinputkan:

nama barang: apel, jumlah: 20, harga: 3000
nama barang: jambu, jumlah: 25, harga: 2500
nama barang: mangga, jumlah: 25, harga: 5000
nama barang: jeruk, jumlah: 33, harga: 3500 Expected Output:

<p>
<img align="center" src="method tambah_barang.png" width="600" height="300" />
</p>

# TEST 2
Customer ingin mengubah nama barang apel menjadi duku dengan method update_nama_barang(). Expected Output:

<p>
<img align="center" src="method update_nama_barang.png" width="600" height="300" />
</p>

# TEST 3
Customer ingin mengubah jumlah barang mangga menjadi 17 buah dengan method update_jumlah_barang(). Expected Output:
<p>
<img align="center" src="method update_jumlah_barang.png" width="600" height="300" />
</p>

# TEST 4
Customer ingin mengubah harga barang jambu menjadi 3000 dengan method update_harga_barang(). Expected Output:
<p>
<img align="center" src="method update_harga_barang.png" width="600" height="300" />
</p>

# TEST 5
Customer ingin menghapus barang duku dengan method hapus_barang(). Expected Output:
<p>
<img align="center" src="method hapus_barang.png" width="600" height="300" />
</p>

# TEST 6
Customer ingin menghitung barang total belanja dengan method total_belanja(). Expected Output:
<p>
<img align="center" src="method total_belanja.png" width="600" height="300" />
</p>

# TEST 7
Customer ingin mengecek belanjaan dengan method cek_order(). Expected Output:
<p>
<img align="center" src="method_cek_order.png" width="600" height="300" />
</p>

# TEST 8
Customer ingin menghapus seluruh barang dengan method reset_transaction(). Expected Output:
<p>
<img align="center" src="method reset_transaction.png" width="600" height="300" />
</p>

# SARAN PENGEMBANGAN
Saran pengembangan selanjutnya, program ini dapat ditambahkan fitur-fitur yang user friendly, dapat menghitung jika ada pajak transaksi, dapat membuat history transaksi, cek stok barang, serta menyimpan data-data transaksi kedalam database.
