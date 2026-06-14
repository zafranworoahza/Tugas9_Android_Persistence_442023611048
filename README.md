Nama : Zafran Woro Ahza
NIM  : 442023611048

![1.jpeg](../../../../1.jpeg)
![2.jpeg](../../../../2.jpeg)
![3.jpeg](../../../../3.jpeg)
![4.png](../../../../4.png)

Penjelasan singkat mengenai mengapa operasi database harus menggunakan fungsi suspend dan dijalankan melalui Dispatchers.IO. :
suspend itu berfungsi agar operasi database tidak memblokir UI thread. Fungsi bisa dijeda tanpa membekukan aplikasi

Dispatchers.IO berfungsi karena Room Database adalah operasi I/O (baca/tulis ke storage). IO dispatcher punya thread pool khusus yang dioptimalkan untuk ini, sehingga Main Thread tetap bebas untuk mengurus tampilan