# Dart Programming

Dart adalah bahasa pemrograman modern yang dikembangkan oleh Google (dirancang oleh Lars Bak dan Kasper Lund). Dart bersifat open source dan banyak dipakai untuk mengembangkan aplikasi mobile, web, server, desktop dan perangkat Internet of Things (IoT). Dart adalah bahasa pemrograman berorientasi objek yang secara sintaksis mirip dengan bahasa C yang membuatnya mudah dipelajari jika kamu lebih suka C atau Java sebagai bahasa pemrograman.

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

> $ merupakan **interpolation** di mana kita bisa memasukkan nilai dari variabel atau expression ke dalam string. konsep ini dikenal dengan nama **String Interpolation**

contoh lain penerapan **String interpolation**
```
void main(){
  print('2 + 4 = ${2 + 4}');
  //jika ingin menampilkan dollar sebagai mata uang
  print('harganya \$50');
  //cara lain
  print(r'harganya $50');
  /*
   Huruf ‘r’ sebelum String akan memberitahu Dart untuk menganggap String sebagai raw, yang berarti akan mengabaikan interpolation.
   */
  
}
/* Outputnya :
2 + 4 = 6
harganya $50
harganya $50 */
```

### Aturan dalam penamaan variabel :
1. Karakter pertama harus berupa huruf, bisa juga pake underscore ( _ )
2. Tidak boleh diawali angka
3. Tidak boleh menggunakan karakter spesial seperti $ # @ & dan lain-lain
4. Tidak boleh menggunakan spasi
5. Jangan menggunakan keyword sebagai nama variabel seperti **print**,**true**,**false**,**final**,**import** dan lain-lain

### Tipe data yang digunakan di dart :
- Integer
- Double
- String
- Boolean
- List *daftar nilai* -> \[10,20,30] atau \["kijang","rusa","beruang"]
- Map *pasangan key-value* -> {"nama":"fiki","umur":20}
- dynamic *tipe data apapun*

**catatan :**
Dart mendukung *type inference*. artinya ketika mendeklarasikan variabel dengan var, 
Dart akan secara otomatis menentukan tipe datanya. Misalnya :

```
var nama = 'Fiki Dedi';  // String
var umur = 20;          // integers
```

Compiler akan tahu bahwa variabel nama memiliki nilai berupa **String** atau teks 
dan variabel umur bernilai angka atau **integer** meskipun kita tidak mendefinisikannya secara eksplisit.

Kamu bisa mendeklarasikan tipe data variabel secara eksplisit untuk menghindari kebingungan dan memudahkan proses debuggin dengan cara berikut

```
String nama = 'Fiki Dedi';  // String
int umur = 20;          // integers
```

contoh kode program berdasarkan tipe datanya
```
void main(){
  //tipe data integer
  int umur = 18;
  
  //tipe data double (desimal)
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

Berikut contoh kode konversi tipe data
```
void main(){
  // String -> int
  var nilai = int.parse('100');
  
  // String -> double
  var nilaidesimal = double.parse('12.5');
  
  // int -> String
  var nilai2 = 20.toString();
  
  // double -> String
  var nilaiphi = 3.14159.toStringAsFixed(2); // String nilaiphi = '3.14'
  
  print(nilai);
  print(nilaidesimal);
  print(nilai2);
  print(nilaiphi);
  
}

```

### Operator di dart
Ada beberapa jenis operator yaitu :
1. Operator Aritmatika
2. Operator Perbandingan
3. Operator Logika

#### Operator Aritmatika
Operator ini digunakan untuk melakukan perhitungan aritmatika seperti penjumlahan, pengurangan, perkalian, pembagian, etc

| Operator | Fungsi |
| ----------- | ----------- |
| + | Penjumlahan |
| - | Pengurangan |
| * | Perkalian |
| / | Pembagian |
| % | Modulo atau sisa hasil bagi |

> Catatan : Operator aritmatika pada pemrograman memiliki aturan yang sama dengan matematika, di mana perkalian dan pembagian akan didahulukan sebelum penjumlahan atau pengurangan.

contoh kode :
```
void main(){
  print(50 + 2);   // 52
  print(50 - 2);   // 48
  print(50 * 2);   // 100
  print(50 / 2);   // 25
  print(50 % 2);   // 0
}
```

dart juga menggunakan konsep increment (x++) dan decrement (b--)

contoh kode :
```
  var a = 16, b = 15;
  a++; //artinya a = a + 1
  b--; //artinya b = b -1
  print(a); // output = 17
  print(b); // output = 14
  
  a+=5;
  print(a); // output = 22
  
  a*=2;
  print(a); //output = 32
```

#### Operator Perbandingan

| Operator | Fungsi |
| ----------- | ----------- |
| == | sama dengan |
| != | tidak sama dengan |
| > | lebih dari |
| < | kurang dari |
| >= | lebih dari sama dengan |
| <= | kurang dari sama dengan |

Contoh penerapan kode :

```
void main(){
  if (10 > 2) {
    print('Benar gan');
  } else {
    print('Salah gan');
  }
}
```

#### Operator Logika

| Operator | Fungsi |
| ----------- | ----------- |
| && | AND |
| \|\| | OR |
| ! | NOT |

contoh kode :
```
void main(){
  //contoh and
  if (10 > 2 && 2 != 2) {
    print('Benar gan');
  } else {
    print('Salah gan');
  }
  //outputnya salah gan
  
  //contoh or
  if (10 > 2 || 2 != 2) {
    print('Benar gan');
  } else {
    print('Salah gan');
  }
  //outputnya benar gan
  
  //contoh not
   if (10 != 0) {
    print('Benar gan');
  } else {
    print('Salah gan');
  }
  //outputnya benar gan
}
```
