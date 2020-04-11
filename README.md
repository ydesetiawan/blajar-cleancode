
# BLajar Clean Code

Saya barusan selesai membaca buku  _“Clean Code”_  karangan dari sang profesor  _“Robert C. Martin”_  yang dikenal dengan sebutan  _“Uncle Bob”_. Buku ini sangat direkomendasikan bagi setiap programmer, karena akan membuka wawasan kita untuk menulis code dengan baik.

![](https://miro.medium.com/max/1408/1*Gu59ODHVL0uehLyEEiLJGQ.jpeg)

Ditulisan kali ini saya akan rangkum point point penting yung diambil dari buku tersebut. Saya tulis dengan Bahasa Indo-English.

Untuk memahami lebih detail mengenai  _“Clean Code”_  kalian bisa googling atau baca sendiri buku ini ya… :)

> “Jika kalian belajar sesuatu, kita harus tulis dan share. Biar gak lupa” :)

Yuk monggo disimak…

# Seperti apa sih Clean Code itu?

-   **_It should be elegant_** _—_ Clean code itu kalau kita baca menyenangkan dan mudah dipahami.
-   **_Clean code is focused_** _—_ Setiap function, setiap class, setiap module menggambarkan satu tujuan.
-   **_Clean code can be read, and enhanced by a developer other than its original author_**

Kalau kata  [“Kent Beck”](https://en.wikipedia.org/wiki/Kent_Beck)  — _a design is simple if it follows these rules (in order of importance:_

-   **_Runs all the tests_**
-   **_Contains no duplication_**
-   **_Expresses the intent of the programmer_**
-   **_Minimizes the number of classes and methods —_** Lebih sedikit code lebih baik.

# Bagaimana sih kita menulis clean code yang baik itu?

## **Mengikuti Universal Principle**

Supaya code kita bisa dikatakan clean code ada beberapa prinsip prinsip dalam dunia pemrograman yang harus kita ikuti dan sudah terbukti banyak digunakan dikalangan profesional, Meliputi :

-   [**_DRY Principle_**](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) **_(Don’t Repeat Yourself) —_**  Menghindari duplication code dimana mana.
-   [**_SOLID Principle_**](https://en.wikipedia.org/wiki/SOLID) **_—_**Software design yang membuat code mudah dimengerti, flexible dan mudah dimaintenance.
-   **_Design Pattern —_**  Silahkan baca di tulisan saya sebelumnya  [**_disini_**](https://medium.com/@ydesetiawan/design-pattern-ah-gak-penting-433f1b977c0a)
-   [**_Test-Driven Development (TDD)_**](https://en.wikipedia.org/wiki/Test-driven_development) **_—_** Keep your test code as clean as production code.

## Meaningful Names

> Choosing good names takes time but saves more than it takes.The name of a variable, function, or class, should answer all the big questions.

Yang harus kita perhatikan ketika membuat nama yaitu :

-   **_Class Names —_**  Setiap class dan object harus pakai kata benda (noun). ex : Account, Product.
-   **_Method Names_  —** Setiap method harus pakai kata kerja (verb). ex : saveAccount, transferProduct.
-   **_Pick One Word per Concept —_**  Pilih satu kata untuk satu abstract konsep dan pertahankan. ex: Account**Controller**, Product**Controller.**

## Functions

> _A Function should do one thing only and do it_ **_really_** _well_

-   **_Avoid passing boolean into a function_ —**  karena function tersebut memiliki if statement yang akan melakukan lebih dari satu hal.
-   **_Functions should either do something or answer something, but not both. —_** Ini memastikan suatu fungsi tidak memiliki efek samping tersembunyi. Sebagai contoh, sebuah function bernama isHoliday() seharusnya hanya return boolean dan tidak melakukan operasi lain.
-   **_Prefer Exceptions to return Error Codes and extract error handling_**  `try catch`  **_into their own function._**
-   **_The Code should always be separated with blank lines to club logical blocks together_**. — Think of different lines of code as thoughts  and then always think of organizing similar thoughts together
-   **_Each function should read like a newspaper._**  — Every function’s implementation follows its call and has less vertical density code.
-   **_Don’t return null_**

## Object and data structures

-   **_Variables should be private —_** jadi kita dapat mengubah type atau implementasinya saat diperlukan. Tidak perlu menambahkan getter / setter ke setiap variabel untuk mengeksposnya sebagai publik.
-   **Hiding implementation by abstractions. —**  We do not want to expose details of data but rather express data as  **abstract terms.**

## Exception handling

-   Try and extract  `try catch`  blocks into separate well-named functions. Having them mixed with other code just confuses the structure of the program. This is in line with the ‘Function should do one thing’ rule. Error handling is one thing.
-   Prefer returning Exceptions instead of Error Codes.
-   Each exception that you throw should provide enough context to determine the source and location of an error.

## Variables

-   Variables should be declared as close to their usage as possible.
-   Keep variables private and only expose  **necessary** interactions as well defined  **abstractions.** Avoid senseless getters and setters which expose all variables unnecessarily.

## Comments

> The only truly good comment is the comment you found a way  **not to write**.

-   Don’t use a comment when you can use a  **well-named**  Function or a Variable
-   Any comment which forces you to look into another module for meaning has failed miserably in communicating and is not worth it at all.

> **“Don’t comment bad code, rewrite it”**
> 
> — Brian W. Kernighan and P. J. Plaugher

mungkin ini saja point point penting yang saya bisa ambil dari buku nya “Uncle Bob” mengenai clean code.

Jika ada pertanyaan atau feedback tolong comment saja di kolom komentar!

Jika kalian setuju dan tertarik mengenai tulisan saya, dengan senang hati boleh di share kok:)
