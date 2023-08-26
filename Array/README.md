# Array

Array digunakan untuk menyimpan banyak value dalam satu variable, daripada mendeklrasian variable terpisah untuk setiap nilai.

Untuk mendeklarasikan sebuah array, definisikan tipe variable, tentukan nama dari array dengan dikuti kurung suku `[]`. dan tentukan jumlah elemen yang harus di simpan. Jadi kita harus mendefinisikan panjang array.

```cpp
string cars[4]
```

Sekaran kita seudh mendeklarasikan sebuah variable yang menyimpan sebuah array untuk 4 string. Untuk memasukkan nilainya, kita gunakan kurung, dan pisahkan dengan koma untuk setiap nilainya

```cpp
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
```

# Mengakse element dari sebuah array

Kita bisa mengakses element array dengan merusjuk ke nomor indexnya didalam kurung siku `[]`.

```cpp
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
cout << cars[0];
// maka Outputs yang akan mucul adalah Volvo
```

# Mengubah Element Array

Untuk menguah nilai dari elemen tertentu, lihat nomor indenya

```cpp
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
cars[0]  = "Opel";
cout << cars[0];
```

# Menghilangkan Ukuran Array

di C++ kita bisa saja tidak menentukan ukuran dari array. Compiler cukup pandai untuk menentukan ukuran dari array berdasarkan jumlah nilai yang dimasukkan.

```cpp
string cars[] = {"Volvo", "BMW", "Ford"}; 
```

kode diatas sama dengan

```cpp
string cars[3] = {"Volvo", "BMW", "Ford"};
```

# Mendapatka Ukuran Array

untuk mendapatkan ukuran dari sebuah array, kita bisa gunakan operator `sizeof()`. 

```cpp
int myNumbers[5] = {10, 20, 30, 40, 50};
cout << sizeof(myNumbers);
```

maka output yang akan muncul adalah 20. Kenapa 20? bukan 5?. itu karena oeprator `sizeof()` mengembalikan ukuran suatu tipe dalam bytes.

Kita telah belajar bahwa integer itu biasaynya berukuran 4 bytes, jadi dari contoh diatas 4 bytes x 5 elements = 20 bytes.

# Looping Aarray Denan sizeof

Kadang kita menulisakn kodisi untuk melooping array dengan cara `i < 5`. Ini tidak ideal, karena dengan cara itu hanya akan bekerja utntuk array dengan specific tertentu.

Dripada menulis kode seperti 

```cpp
int myNumbers[5] = {10, 20, 30, 40, 50};
for (int i = 0; i < 5; i++) {
  cout << myNumbers[i] << "\n";
}
```

Lebih baik 

```cpp
int myNumbers[5] = {10, 20, 30, 40, 50};
for (int i = 0; i < sizeof(myNumbers) / sizeof(int); i++) {
  cout << myNumbers[i] << "\n";
}
```

# Multidimensional Arrays

Untuk mendeklarasikan sebuah multi-dimesional array, definisikan tipe variable, tentukan nama array dikuti dengan kurung siku yang menentukan berapa banyak elemen ang dimiki aray utama. dikuti oleh kurung siku lainyayang mengindikasikan berapa banyak sub array yang dimiliki.

```cpp
string letters[2][4];
```

Seperti aray biasanya, kita bisa menambahkan value dengan sebuah array literal, dipisahka dengan koma untuk setiap itemnya, didalam kurung kurawal.  Di dalam array multi-dimensional array, setiap elemen dalam sebuah array literal adalah array literal lainya.

```cpp
string letters[2][4] = {
    {"A", "B", "C", "D"},
    {"A", "B", "C", "D"}
}
```

Array bisa memiliki banyak dimensi. Semakun banyak dimensi yang dimili sebuah array. Semakin kompleks kodenya. Berikut adalh contoh array tiga dimensi.

```cpp
string latters[2][2][2] = {
    {
        {"A", "B"},
        {"C", "D"}
    },
    {
        {"E", "F"},
        {"G", "H"},
    }
}
```

