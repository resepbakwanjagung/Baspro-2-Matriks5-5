Kode ini mengalikan matriks A dan B dengan ukuran 5×5.

Menggunakan 3 Nested List:

Loop i: untuk baris matriks A.
Loop j: untuk Kolom matriks B.
Loop k: untuk menjumlahkan hasil kali elemen A dan B.

append() digunakan untuk menyusun list demi list ke dalam matriks hasil.

deskripsi beberapa function di code:

* hasil = []
  (Inisialisasi list kosong bernama hasil yang akan menampung matriks hasil akhir dari perkalian A × B)

* for i in range(5):
   loop pertama, berjalan sebanyak 5 kali (karena A punya 5 baris). Variabel i menunjukkan indeks baris saat ini dari matriks A.

* baris = []
  Di dalam loop baris, buat list kosong baris untuk menyimpan nilai-nilai dalam satu baris hasil.

* for j in range(5):
  Loop kedua, berjalan 5 kali juga, karena code akan menghitung nilai di setiap kolom B untuk baris A ke-i. Ini menghasilkan satu elemen dari matriks hasil per iterasi.

*  total = 0
  variabel total untuk menyimpan hasil penjumlahan dari perkalian elemen A dan B untuk posisi [i][j].

*  for k in range(5):
            total += A[i][k] * B[k][j]
  Loop ketiga:

> k adalah indeks untuk mengakses elemen yang akan dikalikan dari baris A dan kolom B.
> A[i][k] adalah elemen di baris i, kolom k dari A.
> B[k][j] adalah elemen di baris k, kolom j dari B.
> Keduanya dikalikan dan dijumlahkan ke total.

* baris.append(total)
  Setelah satu elemen total selesai dihitung, tambahkan ke list baris.

* hasil.append(baris)
  Setelah satu baris lengkap (5 kolom), tambahkan ke list hasil → menjadi baris baru di matriks hasil akhir.

* for row in hasil:
    print(row)
  Loop terakhir, mencetak setiap baris dari matriks hasil ke layar agar terlihat seperti bentuk matriks.

  
