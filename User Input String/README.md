# User Input String

Kemungkinan bisa menggunakan operator ekstrasi >> di cin untuk menyimpan sebuah string yang dimasukkan oleh pengguna.

```cpp
string firstName;
cout << "Type your first name: ";
cin >> firstName; // Mendapatkan input user 
cout << "Your name is: " << firstName;

// maka output yang muncul adalah
// Type your first name: John
// Your name is: John
```

Namun kode diatas bukanlah kode yang tepat. Walaupun bisa menangkap sebuah input dari user, namun kode diatas kuran tepat. Karena, salah satu kelemakan `cin` adalah memperlakukan sebuah spasi, tab, dll sebagai penutup sebuah karater, yang berarti bahwa itu hanya dapat menyimpan satu kata. Jadi diatas kita meninputkan `John` maka itu akan berhasil, tetapi misal kita akan menginputkan `John Cena` maka `cin` hanya akan menyimpan kata pertama yaitu `John`, dan kata `Cena` diabaikan. Shingga variable `firstName` hnya akan berisi `John`. 

Itu kenapa, ketika bekerja dengan string, kita ditawarkan menggunakan fungsi `getline()` untuk membaca sebuah baris dari sebuah text. Dan membutuhkan `cin` sebagai parameter pertama, dan variable string untuk parameter kedua.

```cpp
string fullName;
cout << "Type your full name: ";
getline (cin, fullName);
cout << "Your name is: " << fullName;

// Type your full name: John Doe
// Your name is: John Doe
```