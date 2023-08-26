# Structures

Structures atau bisa sebut `structs` adalah sebuah cara untuk mngelompokkkan bebrapa variabel yang serupa kedalam satu tempat. Setiap variable dalam Structure dikenal sebagai anggota dari Structure.

Tidak seperti array, sebuah Structure bisa berisi banyak tipe data yang berbeda (int, string, bool, dll).

# Membuat sebuah Structure.

UNtuk membuat sebuah structure, gunakan keyword `struct` dan  medeklarasikan setiap anggotanya didalam kurung kurawal.

Setelah deklarasi, tetapkan nama variable Structure

```cpp
struct{                 // Structure declaration
    int myNum;          // anggota 
    string myString;    // anggota
}myStructure;           // structure variable
```

# Mengakses Anggota Structure

Untuk mengakses anggota dari sebuah strcuture, gunakan titik `.`

```cpp
// membuat sebuah structure variable yang bernama myStructure
struct {
    int myNum;       
    string myString;
} myStructure;

// memasukkan value kedalam anggora dari myStructure

myStructure.myNum = 1;
myStructure.myString = "Hello World!";

// manampilkan anggota dari myStructure
cout << myStructure.myNum << "\n";
cout << myStructure.myString << "\n";
```

# Satu struktur dalam banyak variable

kita bisa menggunakan koma `,` untuk menggunakan satu structure dalam banyak variable

```cpp
struct {
    int myNum;
    string myString;
} myStruct1, myStruct2, myStruct3;
```

Berikut adalh contoh bagaimana untuk menggunakan sebuah structure dalam variable yang berbeda

```cpp
struct {
  string brand;
  string model;
  int year;
} myCar1, myCar2; // Kita bisa menambahkan banyak variable dengan memisahkan mereka dalam sebuah koma

// Memasukkan data kedalam struktur pertama yaitu myCar1
myCar1.brand = "BMW";
myCar1.model = "X5";
myCar1.year = 1999;

// Memasukkan data kedalam strukur kedua yaitu myCar2
myCar2.brand = "Ford";
myCar2.model = "Mustang";
myCar2.year = 1969;

// Memunculkan angota
cout << myCar1.brand << " " << myCar1.model << " " << myCar1.year << "\n";
cout << myCar2.brand << " " << myCar2.model << " " << myCar2.year << "\n";
```

# Named Structures

Dengan memberikan sebuah nama untuk structure, kita bisa memperlakukanya sebagai tipe data. Ini beraritu bahwa kamu bisa membuat variable dengan structure ini dimanapun dalam program kapan saja.

Untuk membuat sebuah named structure, masukkan nama dari structure dikanan setelah keyword `struct`.

```cpp
struct myDataType { // This structure is named "myDataType"
  int myNum;
  string myString;
};
```

untuk mendeklarasikan sebuah variable yang menggunakan structure, gunakan nama dari structure sebagai tipe data dari variable

```cpp
myDataType myVar;
```

# Contoh penerapan

```cpp
// Declare a structure named "car"
struct car {
  string brand;
  string model;
  int year;
};

int main() {
  // Membuat sebuah structure car dan menyimpanya dalam myCar1
  car myCar1;
  myCar1.brand = "BMW";
  myCar1.model = "X5";
  myCar1.year = 1999;

  // Membuat sebuah structure car dan menyimpanya dalam myCar2
  car myCar2;
  myCar2.brand = "Ford";
  myCar2.model = "Mustang";
  myCar2.year = 1969;
 
  // Manampilakn anggota structure
  cout << myCar1.brand << " " << myCar1.model << " " << myCar1.year << "\n";
  cout << myCar2.brand << " " << myCar2.model << " " << myCar2.year << "\n";
 
  return 0;
}
```