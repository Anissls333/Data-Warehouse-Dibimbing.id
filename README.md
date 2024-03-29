# Data Warehouse Dibimbing.id

## Tugas Phyton Part 5 - OOP
Membersihkan data `marketing_data.csv` menggunakan prinsip OOP.
Prinsip OOP yang digunakan:
- Basic OOP
- Inheritance
- Polymorphism

### Task 1: Basic OOP
Membuat class MarketingDataETL yang memiliki tiga metode: 
- extract(): akan membaca data dari sebuah file CSV (Misalkan, marketing_data.csv)
- transform(): akan melakukan pembersihan dan transformasi sederhana pada data (seperti mengubah format tanggal atau membersihkan nilai yang kosong)
- store(): akan menyimpan data yang telah ditransformasi ke dalam struktur data DataFramet.

### Task 2: Inheritance & Polymorphism
- Menggunakan inheritance untuk membuat class TargetedMarketingETL yang mewarisi dari MarketingDataETL. 
- Menambah metode segment_customers() yang mengelompokkan pelanggan berdasarkan kriteria tertentu (misalnya, pengeluaran total atau kategori produk yang dibeli).
- Demonstrasi polymorphism dengan meng-override metode transform() dalam TargetedMarketingETL untuk menambahkan logika segmentasi pelanggan ke dalam proses transformasi.

> Ini adalah kutipan.
[https://drive.google.com/file/d/13wg8hC7kpMSzNeS2c27dTKplRKkLgNfn/view?usp=drive_link](https://www.marketing_data.com)


