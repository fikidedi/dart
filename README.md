# Dart Programming

Dart adalah bahasa pemrograman modern yang dikembangkan oleh Google (dirancang oleh Lars Bak dan Kasper Lund). Dart bersifat open source dan banyak dipakai untuk mengembangkan aplikasi mobile, web, server, desktop dan perangkat Internet of Things (IoT). Dart adalah bahasa pemrograman berorientasi objek yang secara sintaksis mirip dengan bahasa C yang membuatnya mudah dipelajari jika Anda lebih suka C atau Java sebagai bahasa pemrograman.

## Editor Online
[Dartpad](https://dartpad.dartlang.org/)

## List Belajar Dart
1. Sintak Dasar (Hello World, Komentar)
```
/* 
 * ini adalah fungsi main. fungsi yang akan dijalankan pertama kali
 * ketika program dijalankan
*/
main(){
  //tampilkan tulisan hello world ke layar
  print("Hello World");
}
```

2. Variabel dan Tipe Data
```
void main(){
  var nama = "Andika";
  var umur = 18;
  print("Nama saya ${nama} berusia ${umur} tahun");
}
```
> Catatan : Dart menganut konsep case sensitive, artinya abc berbeda dengan Abc
Aturan dalam penamaan variabel :
1. Karakter pertama harus berupa huruf, bisa juga pake underscore ( _ )
2. Tidak boleh diawali angka
3. Tidak boleh menggunakan karakter spesial seperti $ # @ & dan lain-lain
4. Tidak boleh menggunakan spasi
5. Jangan menggunakan keyword sebagai nama variabel

3. Operator
