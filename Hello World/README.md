# Menampilkan Hello World

```cpp
#include <iostream>

using namespace std;

int main(){
    cout << "Hello World!";
    return 0;
}
```

Penjelasan

- `#include <iostream>`

    adalah header file library atau pustaka file header yang memungkinkan kita untuk bekerja dengan input dan output objects, seperti `cout` yang kita gunakan tadi

    ## Apa itu Header File Library

    Jadi di dalam bahasa C, header file ini sekumpulan fungsi yang telah di tentukan sebelumnya. Di C header file memiliki extensi `.h`, dan untuk melakukan request untuk menggunakan header file ini di proram kita yaitu dengan directive `#include`.

    Nah di C++ juga menawarkan pengguna berbagai fungsi. Dan di C++ header file bisa saja diakhiri dengan ektensi `.h`.

    Ini menawarkan fitur seperti library function, data types, macros, dll yang di impor ke dalam program dengan bantuan dari preprocessor directive `#include`. Preprocesor directives ini digunakan untuk menginstrusikan bahwa file ini perlu diproses sebelum kompilasi.

    ### Penulisan Header File 

    Kita bisa memasukkan header file di C/C++ menggunakan 2 cara, file yang sudah di definisikan yang berarti bawaan system atau file yang didefinisikan oleh user 

    - Import/Include file di direktori sistem/default

        ```cpp
        #include <filename.h>
        ```

    - Import/include file di direktori yang sama denan file saat ini

        ```cpp
        #include "filename.h"
        ```

    **Penjelasan Lebih Lanjut [Header File Library](https://www.geeksforgeeks.org/header-files-in-c-cpp-and-its-uses/)**

- `using namespace std`

    yang berarti kita bisa mengunakanan nama untuk objek dan variables dari standard library.

- `int main() {}` 

    ini namanya `function`. Kode apapun yang ada didalam kurung kurawal `{}` akan dieksekusi.

- `cout`

    sebuah object yang digunakan bersama dengan **insertion operator** `<<` untuk menampilkan output text. di ontoh itu akan menampilkan output `Hello World!`.

    ## Apa itu Insertion Operator

    Insertion operator ini dilambangkan dengan sytax `<<`. Menurut saya ini seperti Concatenation (sebuah cara untuk mengambungkan bebarapa string menjadi satu). tatapi kita tidak bisa menggunakan langsung dalam sebuah variabel.

    Bagaimana cara mengkontrol format dan bagaiamana cara membuat insertion operator di sebuah class. Insertion `<<` telah diprogram untuk semua tipe data standar di C++, dan nantinya dikirimkan ke object output seperti `cout`. 

    ### Mencoba Mengkontrol Format Output

    - `Output Width`

        Membuat output menjadi right-align atau rata kanan. Yang kita harus lakukan adalah memberikan lebar (widht) output secara spesifik untuk stipa item dengan menggunakan `setw` manipulator atau dengan memanggil fungsi `witdh`

        ```cpp
        #include <iostream>
        using namespace std;

        int main( )
        {
            double values[] = { 1.23, 35.36, 653.7, 4358.24 };
            for( int i = 0; i < 4; i++ )
            {
                cout.width(10);
                cout << values[i] << '\n';
            }
        }
        ``` 

    - `Alignment`
    - `Precision`
    - `Radix`

- `return 0`

    adalah akir dari fungsi `main`