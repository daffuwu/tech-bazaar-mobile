# Tech Bazaar
- [Tugas 7](#tugas-7)

## Tugas 7
### Jelaskan apa yang dimaksud dengan *stateless widget* dan *stateful widget*, dan jelaskan perbedaan dari keduanya

- *Stateless widget* adalah *widget* yang *state* / keadaannya tidak dapat berubah.
- *Stateful widget* adalah *widget* yang dinamis, *state* / keadaannya dapat berubah.

Jika pengguna berinteraksi dengan suatu *widget* yang *stateless*, maka *widget* tersebut tidak akan berubah. Sedangkan jika *widget* tersebut *stateful*, maka *widget* tersebut akan berubah.

### Sebutkan widget apa saja yang kamu gunakan pada proyek ini dan jelaskan fungsinya

- Widget yang berupa teks biasa, seperti judul "Tech Bazaar" serta informasi NPM, kelas, dan nama. 
- Widget yang berupa tombol "Lihat Daftar Produk", "Tambah Produk", dan "Logout" yang akan memberikan pesan ke layar jika ditekan.

### Apa fungsi dari `setState()`? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
Fungsi `setState()` berfungsi untuk memberi tahu *framework* bahwa ada perubahaan *state* (keadaan) dari suatu *widget*. Salah satu variabel yang dapat terdampak dengan fungsi tersebut adalah variabel yang menampilkan *counter* pada layar web. Jika tombol yang terhubung dengan *event handler* counter ditekan, counter akan diperbarui di layar.

### Jelaskan perbedaan antara `const` dengan `final`
Dalam flutter dart `const` dan `final` hampir sama, yaitu untuk mendeklarasi variabel yang nilainya tidak dapat diubah. Namun `final` dapat diisi untuk dengan `DateTime.now()`, sedang `const` tidak bisa. Lebih tepatnya `const` harus diisi oleh nilai yang diketahui sangat **waktu *compile***, sedangkan nilai yang terisi pada `final` dapat diketahui setelah *compile*, yaitu ketika **waktu *running***.

### Jelaskan bagaimana cara kamu mengimplementasikan *checklist-checklist* di atas

1. Membuat sebuah program Flutter baru dengan tema E-Commerce yang sesuai dengan tugas-tugas sebelumnya.
    - Menjalankan perintah `flutter create tech_bazaar` untuk membuat aplikasi Flutter baru.
    -  Membuat berkas [`menu.dart`](lib/menu.dart) untuk menampilkan menu halamam web.

2. Membuat tiga tombol sederhana dengan ikon dan teks
    - Buat seluruh *widget* pada [`menu.dart`](lib/menu.dart) menjadi *stateless*. 
    - Buat *class* `ItemCard` untuk mendefinisikan objek tombol yang akan menampilkan pesan pada layar jika ditekan.
    - Buat *class* `ItemHomepage` untuk desain bentuk tombol.
    - Pada *class* `MyHomePage` tambahkan seluruh widget tombol yang diinginkan.
