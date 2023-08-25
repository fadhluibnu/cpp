# Access String

Kita bisa mengakses karatter di string dengan mengacu ke nomor indexnya didalam kurung kurawal `[]`.

Contoh

```cpp
string myString = "Hello";
cout << myString[0]; // Maka akan muncul output H
```

# Change String Character

Untuk mengubah nilai dari karaker secara spesifik di sebuah sring, merujuk ke nomor index dan gunakan petik satu.

```cpp
string myString = "Hello";
myString[0] = 'J';
cout << myString;
// Maka akan muncul Outputs Jello instead of Hello
```