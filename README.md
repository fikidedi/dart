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
  //beri tanda $ jika dimasukkan dalam petik
  print("Nama saya $nama berusia $umur tahun");
  print(nama);
  print(umur);
}
```
> Catatan : Dart menganut konsep case sensitive, artinya abc berbeda dengan Abc

### Aturan dalam penamaan variabel :
1. Karakter pertama harus berupa huruf, bisa juga pake underscore ( _ )
2. Tidak boleh diawali angka
3. Tidak boleh menggunakan karakter spesial seperti $ # @ & dan lain-lain
4. Tidak boleh menggunakan spasi
5. Jangan menggunakan keyword sebagai nama variabel seperti **print**,**true**,**false**,**final**,**import** dan lain-lain

### Tipe data yang sering digunakan di dart :
- (Number)
  - Integer
  - Double
- String
- Boolean
- List
- Map

**catatan :**
Dart mendukung *type inference*. artinya ketika mendeklarasikan variabel dengan var, 
Dart akan secara otomatis menentukan tipe datanya. Misalnya :

```
var nama = 'Fiki Dedi';  // String
var umur = 20;          // integers
```

Compiler akan tahu bahwa variabel nama memiliki nilai berupa String atau teks 
dan variabel umur bernilai angka atau integer meskipun kita tidak mendefinisikannya secara eksplisit.

```
void main(){
  //tipe data integer
  int umur = 18;
  
  //tipe data double
  double phi = 3.14;
  
  //tipe data string
  var pesan = "Selamat datang";
  //String pesan = "Selamat datang";
  
  //tipe data boolean
  bool isValid = true;
  
  //list
  var angka = [1,2,3,4,5];
  
  //map
  var makanan = {'Bakso':10000,'Mie Ayam':12000};
  
  print(umur);
  print(phi);
  print(pesan);
  print(isValid);
  print(angka);
  print(makanan);

}
```
