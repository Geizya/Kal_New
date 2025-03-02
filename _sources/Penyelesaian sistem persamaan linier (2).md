---
title: Penyelesaian sistem persamaan linier

---

# Penyelesaian sistem persamaan linier 
## operasi baris elementer 
operasi baris elementer(OBE)operasi yang dilakukan pada baris suatu matriks untuk mengubahnya menjadi bentuk yang lebih sederhana. OBE dapat digunakan untuk menyelesaikan sistem persamaan linear (SPL) dan menentukan invers matriks. 

ciri ciri obe:
1.Mengubah Matriks Tanpa Mengubah Solusi Sistem
2.Dapat Dibalik (Inversibel)
3.Matriks Tidak Kehilangan Struktur

jenis obe:
1.Pertukaran Baris dengan Menukar posisi dua baris dalam matriks.
2.Pengalian Baris dengan Mengalikan setiap elemen dalam suatu baris dengan konstanta non-nol.
3.Penjumlahan Baris yaitu Menambahkan kelipatan dari satu baris ke baris lainnya.

## eliminasi gaus 
Eliminasi Gauss yaitu metode yang digunakan untuk menyelesaikan sistem persamaan linier.dengan metode ini untuk mengubah sistem persamaan linier menjadi bentuk yang lebih sederhana/dalam bentuk matriks eselon baris sehingga dapat ditemukan solusinya dengan lebih mudah.Metode eliminasi Gauss dilakukan melalui serangkaian operasi baris elementer pada matriks koefisien dari sistem persamaan linier.


### contoh soal 1 

selesaikan dengan menggunakan eliminasi gauss
$$
\begin{array}{cc}
x_1+2x_2+3x_3z&=6\\
2x_1+4_2+6x_12&=4\\
x_3-x_24&=2
\end{array}
$$

Selesaikan dengan menggunakan eliminasi Gauss
$$
\begin{array}{cc}
x_1+2x_2+3x_3&=6\\
2x_1+4x_2+6x_3&=12\\
x_2+x_3&=2
\end{array}
$$
jawab:
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
2 & 4 & 6 & | &12\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 0 & 0 & | &0\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
x_2+x_3 = 2\\
x_2 = 2 - x_3\\
\end{array}
$$
$$
\begin{array}{cc}
x_1+2x_2+3x_3 = 6\\
x_2 = 2 - x_3 \\
\end{array}
$$
$$
\begin{array}{cc}
x_1 + 2(2-x_3)+3x_3 = 6\\
x_1 + 4-2x_3+3x_3 = 6\\
x_1+4+x_3\\
x_1=2-x_3
\end{array}
$$
$$
\begin{array}{cc}
x_1 = 2-x_3\\
x_2=2-x_3\\
x_3=x_3
\end{array}
$$
jadi hanya ada satu variabel maka sistem memiliki, tak hingga banyak solusi


### contoh soal 2 

$$
\begin{array}{cc}
x_1+x_2+x_3&=3\\
2x_1+2x_3&=5\\
x_1+2x_2&=3
\end{array}
$$
jawab: 
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
2 & 0 & 2 & | &5\\
1 & 2 & 0 & | &3\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 1 & -1& | &0\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 0 & -1 & | &-1/2\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
-x_3=-1/2\\
x_3=1/2
\end{array}
$$
$$
\begin{array}{cc}
-2x_2=-1\\
x_2=1/2
\end{array}
$$
$$
\begin{array}{cc}
x_1+x_2+x_3=3\\
x_1+1/2+1/2=3\\
x_1+1=3\\
x_1=2
\end{array}
$$
hasil akhirnya adalah:
$$
\begin{array}{cc}
(x_1+x_2+x_3)=(2,1/2,1/2)
\end{array}
$$
jadi, sistem ini memiliki solusi tunggal.


### contoh soal 3

$$
\begin{array}{cc}
2x_1+2x_2&=4\\
x_1+x_2&=2
\end{array}
$$
jawab:
$$
\begin{bmatrix}
2 & 2 &  | &4\\
1 & 1 &  | &2\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 &  | &2\\
1 & 1 &  | &2\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
x_1+x_2=2\\
x_1=2-x_2\\
x_2=x_2
\end{array}
$$
$$
\begin{array}{cc}
(x_1,x_2)=(2-x_2,x_2)
\end{array}
$$
$$
\begin{array}{cc}
jika(x_2=0),maka((x_1,x_2)=(2,0))\\
jika(x_2=1),maka((x_1,x_2)=(1,1))\\
jika(x_2=2),maka((x_1,x_2)=(0,2))
\end{array}
$$
maka sistem ini memiliki tak hingga banyak solusi.

### contoh soal 4

$$
\begin{array}{cc}
x_1+x_2&=5\\
x_1+2x_3&=6
\end{array}
$$
jawab:
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 2 &| &6\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 1 &| &1\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
x_2=1\\
x_1+1=5\\
x_1=4
\end{array}
$$
jadi:
$$
\begin{array}{cc}
(x_1,x_2)=(4,1)
\end{array}
$$
maka, sistem ini memiliki solusi tunggal.