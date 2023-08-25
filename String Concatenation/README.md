# String Concatenation

operator `+` bisa digunakan antar string untuk menjumlahkan guna membuat string baru. Ini dinamakan `concatenation`

Berikut adalah contohnya

```cpp
string firstName = "John";
string lastName = "Doe";
string fullName = firstName + " " + lastName;
cout << fullName;
```

## Append

Sebuah string di C++ sebenarnya adalah sebuah object, yang berisi fungsi yang dapat melakukan operasi tetentu pada string. Sebagai contoh, kita bisa melakukan concatenate string dengan `append()`

```cpp
string firstName = "John ";
string lastName = "Doe";
string fullName = firstName.append(lastName);
cout << fullName;
```