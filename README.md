# self-cashier-sederhana
# Latar Belakang Masalah
Andi adalah seorang pemilik supermarket. Beliau ingin memperbaiki proses bisnis di supermarket miliknya, yaitu dengan membuat sistem kasir self-service agar customer bisa langsung menginputkan barang yang dibelinya saat ingin melakukan pembayaran secara mandiri. Hal ini dilakukan agar customer yang berada di luar kota juga bisa membeli barang dari supermarket tersebut.

Untuk memecahkan masalah tersebut adalah dengan membuat program Cashier Self-Service untuk memperbaiki proses bisnis di supermarket milik Andi.

# Objective
Tujuan dari pembuatan projek ini adalah membuat sistem kasir self-service yang dapat melakukan beberapa metode yaitu:

Customer dapat menginput barang, jumlah barang, dan juga harga barang dengan metode tambah_barang.
Jika customer salah input, ia dapat mengubah salah satu inputanya:
mengubah nama barang dengan metode update_nama_barang.
mengubah jumlah barang dengan metode update_jumlah_barang.
mengubah harga barang dengan metode update_harga_barang.
Jika customer ingin menghapus salah satu barang dari daftar barang belanjanya, dapat menggunakan metode hapus_barang.
Jika customer ingin menghapus semua barang dari daftar belanjanya, dapat menggunakan metode reset_transaction.
Sebelum dapat menghitung total belanjanya, isi dari daftar belanja customer dicek dulu dengan metode cek_order. Metode ini mengecek apakah ada inputan yang masih salah pada daftar barang belanja customer.
Sistem dapat menghitung semua total belanja dan juga diskon yang didapatkannya dengan metode total_belanja.
Ketentuan untuk memperoleh diskon:
Jika total belanja diatas Rp.500.000, maka diskon 10%
Jika total belanja diatas Rp.300.000, maka diskon 8%
Jika total belanja diatas Rp.200.000, maka diskon 5%
# Method yang digunakan
tambah_barang()
Metode ini digunakan untuk memasukkan barang ke daftar barang belanja.

update_nama_barang()
Metode ini digunakan untuk merubah nama barang yang sudah ada dalam daftar barang belanja.

update_jumlah_barang()
Metode ini digunakan untuk merubah jumlah barang berdasarkan nama barang yang ada didalam daftar barang belanja.

update_harga_barang()
Metode ini digunakan untuk merubah harga barang berdasarkan nama barang yang ada didalam daftar barang belanja.

hapus_barang()
Metode ini digunakan untuk menghapus salah satu barang yang diinginkan berdasarkan nama barang yang ada didalam daftar barang belanja

reset_transaction()
Metode ini digunakan untuk menghapus semua barang didalam daftar barang belanjaan.

cek_order()
Metode ini digunakan untuk memastikan data yang diinputkan sudah benar atau belum.

total_belanja()

Metode ini digunakan untuk menghitung total harga dari daftar barang belanja customer.
<p>
<img align="center" src="flowchart.jpg" width="800" height="1200" />
</p>
