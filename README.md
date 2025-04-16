Kode ini mengalikan matriks A dan B dengan ukuran 5×5.

Menggunakan 3 Nested List:

* Loop i: untuk baris matriks A.
* Loop j: untuk Kolom matriks B.
* Loop k: untuk menjumlahkan hasil kali elemen A dan B.

>append()
<br>digunakan untuk menyusun list demi list ke dalam matriks hasil.

deskripsi beberapa function di code:

* >hasil = []
  <br>(Inisialisasi list kosong bernama hasil yang akan menampung matriks hasil akhir dari perkalian A × B)

* >for i in range(5):
   <br>loop pertama, berjalan sebanyak 5 kali (karena A punya 5 baris). Variabel i menunjukkan indeks baris saat ini dari matriks A.

* >baris = []
  <br>Di dalam loop baris, buat list kosong baris untuk menyimpan nilai-nilai dalam satu baris hasil.

* >for j in range(5):
  <br>Loop kedua, berjalan 5 kali juga, karena code akan menghitung nilai di setiap kolom B untuk baris A ke-i. Ini menghasilkan satu elemen dari matriks hasil per iterasi.

*  >total = 0
  <br>variabel total untuk menyimpan hasil penjumlahan dari perkalian elemen A dan B untuk posisi [i][j].

*  >for k in range(5):
            <br>total += A[i][k] * B[k][j]
  <br>Loop ketiga:

<br>k adalah indeks untuk mengakses elemen yang akan dikalikan dari baris A dan kolom B.
<br>A[i][k] adalah elemen di baris i, kolom k dari A.
<br>B[k][j] adalah elemen di baris k, kolom j dari B.
<br>Keduanya dikalikan dan dijumlahkan ke total.

* >baris.append(total)
  <br>Setelah satu elemen total selesai dihitung, tambahkan ke list baris.

* >hasil.append(baris)
  <br>Setelah satu baris lengkap (5 kolom), tambahkan ke list hasil → menjadi baris baru di matriks hasil akhir.

* >for row in hasil:
    <br>>print(row)
  <br>Loop terakhir, mencetak setiap baris dari matriks hasil ke layar agar terlihat seperti bentuk matriks.

List A : 

<br>[1, 2, 3, 4, 5],
<br>[6, 7, 8, 9, 10],
<br>[11, 12, 13, 14, 15],
<br>[16, 17, 18, 19, 20],
<br>[21, 22, 23, 24, 25]

List B :

<br>[25, 24, 23, 22, 21],
<br>[20, 19, 18, 17, 16],
<br>[15, 14, 13, 12, 11],
<br>[10, 9, 8, 7, 6],
<br>[5, 4, 3, 2, 1]


Output:

<br>[175, 160, 145, 130, 115]
<br>[550, 510, 470, 430, 390]
<br>[925, 860, 795, 730, 665]
<br>[1300, 1210, 1120, 1030, 940]
<br>[1675, 1560, 1445, 1330, 1215]

