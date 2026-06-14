Nama : Zafran Woro Ahza
NIM  : 442023611048

![Screenshot](images/1.jpeg)
![Screenshot](images/2.jpeg)
![Screenshot](images/3.jpeg)
![Screenshot](images/4.jpeg)

Penjelasan singkat mengenai mengapa operasi database harus menggunakan fungsi suspend dan dijalankan melalui Dispatchers.IO. :
suspend itu berfungsi agar operasi database tidak memblokir UI thread. Fungsi bisa dijeda tanpa membekukan aplikasi

Dispatchers.IO berfungsi karena Room Database adalah operasi I/O (baca/tulis ke storage). IO dispatcher punya thread pool khusus yang dioptimalkan untuk ini, sehingga Main Thread tetap bebas untuk mengurus tampilan