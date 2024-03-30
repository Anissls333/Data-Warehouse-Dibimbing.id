# Tugas Phyton Part 5 - OOP
Membersihkan data `marketing_data.csv` menggunakan prinsip OOP.
Prinsip OOP yang digunakan:
- Basic OOP
- Inheritance
- Polymorphism

## Class
Pada github kali ini terdiri dari 2 kelas di Phyton:
1. `MarketingDataETL`
2. `TargetedMarketingETL`

### `MarketingDataETL`
Kelas `MarketingDataETL` merupakan alat untuk mengekstrak, mentransformasi, dan menyimpan data pemasaran dari sebuah file CSV. Prosedur:
1. Inisialisasi processor
2. **extract()** : mengekstraksi data.
3. **transform()** : melakukan transformasi data seperti penghapusan baris kosong, pengubahan format tanggal, pengurutan berdasarkan ID pelanggan.
4. **store()** : menyimpan data yang telah ditransformasi ke dalam struktur data DataFrame atau ke dalam file CSV baru.

Setelah proses ekstraksi, transformasi, dan penyimpanan, data yang telah diproses akan memiliki 4 kolom data:
1. **customer_id** (ID pelanggang) yang telah diurutkan secara ascending (kecil ke besar)
2. **purchase_date** (tanggal pembelian) yang telah diubah format tanggalnya menjadi YYYY-MM-DD
3. **product_category** (kategori produk)
4. **amount_spent** (jumlah yang dihabiskan)
   
### `TargetedMarketingETL`
Kelas `TargetedMarketingETL` merupakan turunan dari kelas `MarketingDataETL` yang ditambahkan dengan kemampuan untuk melakukan segmentasi pelanggan berdasarkan kriteria tertentu. Kelas ini dapat melakukan operasi ekstraksi, transformasi, dan penyimpanan data seperti kelas induknya, namun juga mampu melakukan segmentasi pelanggan sesuai dengan kriteria yang ditentukan.

Kelas `TargetedMarketingETL` memiliki metode tambahan sebagai berikut:
- **segment_customers(criteria)**: Metode ini memungkinkan untuk melakukan segmentasi pelanggan berdasarkan kriteria tertentu, seperti total pengeluaran atau kategori produk yang dibeli.
  
Metode **transform()** juga di-override untuk menambahkan logika tambahan terkait segmentasi pelanggan.

Data yang dihasilkan akan memperlihatkan total pengeluaran setiap pelanggan, memungkinkan untuk pemahaman yang lebih baik tentang pola pembelian pelanggan.
