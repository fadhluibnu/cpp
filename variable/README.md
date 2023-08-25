# Variable

Variable adalah kontainer yang membungkus nilai.

Ada bebrapa tipe data yang ada di variable dan kita harus mendefinisikan dengan keyword yang berbeda juga, Contoh :

- `int`

    Meyimpan integer, tanpa adanya desimal. Seperti 123 atau -123.

- `double`

    Menyimpan angka floating atau desimal. Seperti 19.99 or -19.99

- `char`

    Menyimpan karakter tunggal seperti `a` atau `B`. Untuk mendefinisikan nilai Char kita gunakan petik satu `'..'`.

- `string`

    Menyimpan text seperti `"Hello World"`. Untuk mendefinisikan Nilai String kita gunakan petik dua `".."`.

- `bool`

    Menyimpan nilai dengan dua keadaan yaitu true atau false

## Mendeklarasikan Variabel

Untuk membuat sebuah variabel, tentukan jenisnya adn masukkan nilainya

```
type variableName = value
```
Dimana untuk `type` adalah salah satu tipe data dari C++ seperti `int` dan variableName adalah nama dari variable seperti x atau myName. Tanda sama dengan digunakan untuk memasukkan nilai ke variable.

Berikut adalah syntax untuk membuat variable yang menyimpan number.

```cpp
int myNum = 15;
cout << myNum;
```

Berikut adalah implementasi dari semua tipe variable

```cpp
int myNum = 15;
double myFloatNum = 5.99;
char test = 'F';
string myText = "Hello";
bool myBoolean = true;
cout << "My Num : " << myNum << endl ;
cout << "My Float : " << myFloatNum << endl ;
cout << "My Char : " << test << endl ;
cout << "My String : " << myText << endl ;
cout << "My Boolean : " << myBoolean << endl ;
```

# Mendeklarasikan Banyak Variable 

## Mendeklarasikan banyak Variable

Untuk mendeklarasikan lebih dari satu variable dari tipe yang sama, gunakan coma untuk memisahkan daftar/list

contoh

```cpp
int x = 5, y = 6, z = 50;
```

Jadi kita bisa mendeklarasikan variable tanpa mengulan ulang menuliskan keyword yang sama.

## Satu Nilai/Value untuk Banyak Variable

Kita juga bisa memasukkan value yang sama untuk banyak variable dalam satu baris.

contoh

```cpp
int x, y, z;
x = y = z = 50;
cout << x + y + z;
```

# Rule For Naming Variables

Variable C++ harus di diidentifikasikan dengan nama yang unik. Keunikan nama ini dipanggil indefiers. 

Ada bebrapa persnyaratan untuk mendefinisikan nama di variable C++

- Bisa berisi huruf, angka dan garis bawah
- Harus dimulai dengan huruf atau garis bawah
- Case Senstive 
- Tidak boleh berisi spasi atau special character seperti !, #, %, dll
- Kata kata yang mengandun keyword di C++ seperti `int`


# Constant Variable

Kondisi dimana kita tidak ingin value dari variable kita diubah dengan kata lain variabel kita tidak bisa diubah setelah kita tetapkan nilai pertama kali atau bisa disebut read-only. Untuk membuat constant variable kita bisa gunakan `const` keyword.

contoh

```cpp
const int myNum = 15 // variabel ini telah didevinisikan dengan nilai 15
myNum = 10 //ini akan menyebabkan error
```

Jadi variable dengan nama myNum diinisialisasi dengan value `15`. Setelah itu di line selanjutnya kita mencoba mengubah value myNum dari `15` menjadi `10`. Tindakan ini akan menyebabkan error karena variable myNum adalah variable constant yang artinya setelah variabel myNum diberikan sebuah nilai, maka kita tidak bisa mengubah nilai tersebut.