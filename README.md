# Pertemuan 06 Nested Loop Python

Nama: Alfitrah Zahra Ameliya
NIM: 2225250181
Kelas: 3B

## Tujuan

Menggunakan nested loop, pola, akumulasi, dan pencacahan.

## Cara Menjalankan

Untuk menjalankan Tugas 3, gunakan perintah:

python3 tugas/tabel_perkalian_dan_statistik.py

## Algoritma Tugas 3

Program diawali dengan menampilkan judul dan meminta pengguna memasukkan nilai n.

Jika n kurang dari atau sama dengan 0, program meminta input kembali sampai pengguna memasukkan nilai n yang positif.

Variabel total_semua digunakan sebagai akumulator untuk menghitung jumlah seluruh hasil perkalian. Variabel count_genap digunakan sebagai counter untuk menghitung banyak hasil perkalian yang bernilai genap.

Loop luar menggunakan variabel i untuk mengatur baris dari 1 sampai n. Pada setiap baris, total_baris diatur kembali menjadi 0 karena digunakan untuk menghitung jumlah hasil pada baris tersebut.

Loop dalam menggunakan variabel j untuk mengatur kolom dari 1 sampai n. Pada setiap pasangan i dan j, program menghitung hasil = i * j. Hasil tersebut ditampilkan, kemudian ditambahkan ke total_baris dan total_semua.

Jika hasil merupakan bilangan genap, count_genap bertambah satu.

Setelah loop dalam selesai, program menampilkan jumlah pada baris tersebut. Setelah seluruh loop selesai, program menampilkan total seluruh hasil dan banyak hasil genap.

## Hasil Pengujian

| Input n | Hasil yang Diharapkan | Keluaran Aktual | Status |
| 1 | Total seluruh hasil = 1, Banyak hasil genap = 0 | Total seluruh hasil = 1, Banyak hasil genap = 0 | Berhasil |
| 2 | Total seluruh hasil = 9, Banyak hasil genap = 3 | Total seluruh hasil = 9, Banyak hasil genap = 3 | Berhasil |
| 3 | Total seluruh hasil = 36, Banyak hasil genap = 5 | Total seluruh hasil = 36, Banyak hasil genap = 5 | Berhasil |

## Analisis Efisiensi

Untuk input n, loop luar berjalan sebanyak n kali dan loop dalam berjalan sebanyak n kali untuk setiap iterasi loop luar. Oleh karena itu, badan loop dalam dijalankan sebanyak n x n atau n² kali.

## Refleksi

Salah satu hal yang perlu diperhatikan dalam nested loop adalah lokasi inisialisasi variabel. total_baris harus direset pada setiap iterasi loop luar karena digunakan untuk menghitung jumlah pada setiap baris. Sebaliknya, total_semua tidak direset pada setiap baris karena digunakan untuk menghitung jumlah seluruh hasil perkalian.

Dari pengujian, program berhasil menjalankan nested loop, menghitung jumlah setiap baris, menghitung total keseluruhan, dan menghitung banyak hasil genap sesuai dengan test case yang diberikan.