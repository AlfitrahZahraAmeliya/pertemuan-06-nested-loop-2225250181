# Pertemuan 06 Nested Loop Python

Algoritma dan Pemrograman | Pertemuan 06

Nama: Alfitrah Zahra Ameliya  
NIM: 2225250181  
Kelas: 3B  

## Tujuan

Menggunakan nested loop, pola, akumulasi, dan pencacahan.

## Cara Menjalankan

python3 tugas/tabel_perkalian_dan_statistik.py

## Algoritma Tugas 3

Program menggunakan nested loop untuk membentuk tabel perkalian dari 1 sampai `n`, menghitung jumlah setiap baris, menghitung total seluruh hasil perkalian, dan menghitung banyak hasil perkalian yang genap.

1. Membaca dan memvalidasi input `n`.
2. Menginisialisasi `total_semua = 0` dan `count_genap = 0`.
3. Menjalankan loop luar untuk nilai `i` dari 1 sampai `n`.
4. Menginisialisasi `total_baris = 0` pada setiap baris.
5. Menjalankan loop dalam untuk nilai `j` dari 1 sampai `n`.
6. Menghitung `hasil = i * j`.
7. Menambahkan `hasil` ke `total_baris` dan `total_semua`.
8. Jika `hasil` merupakan bilangan genap, maka `count_genap` ditambah 1.
9. Setelah loop dalam selesai, menampilkan `total_baris`.
10. Setelah kedua loop selesai, menampilkan `total_semua` dan `count_genap`.

Peran masing-masing bagian:

- **Loop luar (`i`)** digunakan untuk mengatur baris pada tabel.
- **Loop dalam (`j`)** digunakan untuk mengatur kolom pada setiap baris.
- **Akumulator (`total_baris` dan `total_semua`)** digunakan untuk menjumlahkan hasil perkalian.
- **Counter (`count_genap`)** digunakan untuk menghitung banyak hasil perkalian yang bernilai genap.

## Hasil Pengujian

| Input n | Hasil yang Diharapkan | Keluaran Aktual | Status |
|---|---|---|---|
| 1 | Jumlah pasangan = 1, Total seluruh hasil = 1, Banyak hasil genap = 0 | Jumlah pasangan = 1, Total seluruh hasil = 1, Banyak hasil genap = 0 | Berhasil |
| 2 | Jumlah pasangan = 4, Total seluruh hasil = 9, Banyak hasil genap = 3 | Jumlah pasangan = 4, Total seluruh hasil = 9, Banyak hasil genap = 3 | Berhasil |
| 3 | Jumlah pasangan = 9, Total seluruh hasil = 36, Banyak hasil genap = 5 | Jumlah pasangan = 9, Total seluruh hasil = 36, Banyak hasil genap = 5 | Berhasil |

## Analisis Efisiensi

Untuk input `n`, loop luar berjalan sebanyak `n` kali. Pada setiap iterasi loop luar, loop dalam juga berjalan sebanyak `n` kali.

Dengan demikian, badan loop dalam dijalankan sebanyak:

`n × n = n²`

kali.

Contohnya:

- Jika `n = 1`, badan loop dalam berjalan 1 kali.
- Jika `n = 2`, badan loop dalam berjalan 4 kali.
- Jika `n = 3`, badan loop dalam berjalan 9 kali.

Semakin besar nilai `n`, semakin banyak operasi yang dilakukan oleh nested loop.

## Refleksi

Kesalahan yang ditemukan adalah `total_baris` tidak direset pada setiap baris. Akibatnya, hasil baris sebelumnya ikut terbawa. Kesalahan diperbaiki dengan mengatur `total_baris = 0` sebelum loop dalam dimulai.