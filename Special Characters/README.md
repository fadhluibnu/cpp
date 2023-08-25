# Special Character

Dikarenakan string harus ditulis dengan petik, Jadi jika  tidak di tulis dalam sebuah petik maka C++ akan salah paham terhadap string tersebut dan akan membuat sebuah error

```cpp
string txt = "We are the so-called "Vikings" from the north.";
```

Contoh diatas akan memuculkan sebuah error karena `Vikings` tidak berada dalam sebuah tanda petik. solusi untuk menghindari masalah ini adalah mengunakan **backslash escape character**

```cpp
string txt = "We are the so-called \"Vikings\" from the north.";
```

Backslash escape character `\` mengubah karater khusus menjadi karater string

Escape character | Result | Description
--- | --- | --- |
`\'` | `'` | Single quote
`\"` | `"` | Double quote
`\\` | `\` | Backslash
`\n` | New Line	
`\t` | Tab