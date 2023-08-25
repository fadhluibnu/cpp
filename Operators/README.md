# Operators

Operators diunakan untuk melakukan operasi di variable dan value.

Berikut adalah contoh penggunaan operator `+` untuk menambahakan dua value.

```cpp
int x = 100 +50;
```

Selain bisa manambahakan value dengan value. Operator + juga bisa menambahakan variable dengan value. atau variable dengan variable.

```cpp
int sum1 = 100 + 50;        // 150 (100 + 50)
int sum2 = sum1 + 250;      // 400 (150 + 250)
int sum3 = sum2 + sum2;     // 800 (400 + 400)
```

# Operator Aritmatika

Operator aritmatika digunakan untuk melakukan operasi matematika umum.

Operator | Name | Deskripsi | Contoh
--- | --- | --- | --- |
`+` | Tambahan | Menambahkan Dua Nilai | x + y
`-` | Pengurangan | Mengurangi satu nilai dari nilai lainya | x - y
`-` | Multiplacation | Mengalikan Dua Nilai | x * y
`/` | Pembagian | Membagikan satu value oleh value lainya | x / y
`%` | Modulus | Mengembalikan sisa bagi | x % y
`++` | Increment | Meningkatkan value variable sebanyak 1 | ++y
`++` | Decrement | Menrunkan value variable sebanyak 1 | --y

# Operator Penugasan (Assignment)

Operator Penugasan digunakan untk memasukkan value kedalam variable.

Berikut adalah contoh penggunaan operator penugasan yaitu `=` yng digunakan untuk memasukkan value 10 kedalam variable x

```cpp
int x = 10;
```

Berikut adalah daftar operator penugasan

Operator | Contoh | Sama Dengan
--- | --- | --- | 
`=` | x = 5 | x = 5
`+=` | x += 3 | x = x + 3	
`-=` | x -= 3 | x = x - 3	
`*=` | x *= 3 | x = x * 3	
`/=` | x /= 3 | x = x / 3	
`%=` | x %= 3 | x = x % 3	
`&=` | x &= 3 | x = x & 3	
`|=` | `x |= 3` | `x = x | 3`
`^=` | x ^= 3 | x = x ^ 3	
`>>=` | x >>= 3 | x = x >> 3	
`<<=` | x <<= 3 | x = x << 3

# Comparison Operator

Comparison operator atau operator pembanding digunakan untuk membandingkan dua nilai (atau variable). Ini sangat penting pada pemrograman, karena itu membantu kita untuk menemukan jawaban dan membuat keputusan.

Nilai yang dikembaikan dari sebuah perbandingan salah yaitu true `1` atau false `0`. Nilai ini dikenal sebagai nilai boolean.

Berikut adalah contoh menggunakan lebih besar dari untuk mencaritahu apakah 5 lebih besar dari 3

```cpp
int x = 5;
int y = 3;
cout << (x > y); //ini akan mengembalikan 1 (true) karena 5 lebih besar dari 3
```

Berikut adalah daftar dari operator perbandingan

Operator | Nama | Contoh
--- | --- | --- | 
`==` | Equal to | x == y	
`!=` | Not equal | x != y	
`>` | Greater than | x > y	
`<` | Less than | x < y	
`>=` | Greater than or equal to | x >= y	
`<=` | Less than or equal to | x <= y

# Logicial Operator

Sama seperti comparison operators, logicial operator atau operator logika juga mengembalikan true `1` atau false `0`

Operator logika digunakan untuk menentukan logika antar variabel atau nilai

Operator | Nama | Deskripsi | Contoh
--- | --- | --- | --- |
`&&` | Logical and Returns true if both statements are true | x < 5 &&  x < 10	
`||` | Logical or Returns true if one of the statements is true | `x < 5 || x < 4`	
`!` | Logical not Reverse the result, returns false if the result is true | !(x < 5 && x < 10)