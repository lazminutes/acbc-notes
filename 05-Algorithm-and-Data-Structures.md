# Pseudocode Note 1

## Deklarasi dan Assignment Variable

Tipe data pada saat melakukan deklarasi dan assignment sebuah variable harus jelas. Dua penulisan di bawah ini adalah contoh yang diharapkan.

```
// Tipe data ditentukan dari nilai yang diberikan pada variable
STORE variableName WITH <value>

// Tipe data disebutkan dengan jelas, diikuti dengan nilai yang diberikan pada variable
STORE variableName AS <data-type> WITH <value>
```

Sebuah variable dapat memiliki nilai yang ditentukan belakangan. Umumnya, penulisan ini digunakan untuk menggambarkan user input. Dua penulisan di bawah ini adalah contoh yang diharapkan.

```
// data-type dapat diisi dengan tipe data seperti STRING, NUMBER, BOOLEAN, dsb.
STORE variableName WITH ANY <data-type>

// data-type dapat diisi dengan tipe data seperti STRING, NUMBER, BOOLEAN, dsb.
STORE variableName AS <data-type> WITH ANY VALUE
```

## Reassign Variable

Nilai dari sebuah variable dapat diperbarui (reassign). Update nilai variable dapat dilakukan menggunakan keyword `SET ... WITH ...`. Berikut adalah penulisan yang diharapkan.

```
// Deklarasi dan assignment variable
STORE variableName WTIH ANY NUMBER

// Reassign variable
SET variableName WITH 10
```

## Conditional

Pseudocode conditional dapat dituliskan seperti di bawah.

```
IF statement
  ...
ELSE IF statement
  ...
ELSE
  ...
END IF
```

## Mathematical Operators

```
STORE variableName WITH ANY NUMBER

SET variableName WITH variableName PLUS 10        // penambahan
SET variableName WITH variableName MINUS 10       // pengurangan
SET variableName WITH variableName TIMES 10       // perkalian
SET variableName WITH variableName DIVIDE BY 10   // pembagian
SET variableName WITH variableName MODULUS BY 10  // modulus (sisa bagi)
```

## Comparison Operators

```
STORE variableName WITH ANY NUMBER

IF variableName MORE THAN 10             // lebih dari
  ...
ELSE IF variableName MORE THAN EQUAL 10  // lebih dari sama dengan
  ...
ELSE IF variableName LESS THAN 10        // kurang dari
  ...
ELSE IF variableName LESS THAN EQUAL 10  // kurang dari sama dengan
  ...
ELSE IF variableName EQUAL 10            // sama dengan
  ...
ELSE IF variableName NOT EQUAL 10        // tidak sama dengan
  ...
END IF
```

## Truthy dan Falsy

```
STORE variableName WITH ANY STRING

IF variableName IS TRUTHY
  ...
END IF

IF variableName IS FALSY
  ...
END IF
```

## Display

Proses menampilkan output dapat diwakili oleh keyword `DISPLAY`.

```
STORE variableName WITH ANY STRING
STORE variableName2 WITH ANY STRING


// Menampilkan nilai variableName
DISPLAY variableName

// Menampilkan nilai variableName2
DISPLAY variableName2

// Menampilkan nilai variableName dan nilai variableName2 yang digabung dengan string lain
DISPLAY "Nilai variableName" CONCAT WITH variableName CONCAT WITH "Nilai variableName2" CONCAT WITH variableName2
```

## Example 1

Buat sebuah pseudocode yang akan menampilkan pesan berdasarkan hasil pembacaan suhu tubuh seseorang. Apabila suhu tubuhnya lebih dari 36 derajat, maka pesan yang ditampilkan adalah `You are sick`. Jika tidak, maka yang ditampilkan adalah `You are healthy`.

```
STORE temprature WITH ANY NUMBER

IF temprature MORE THAN 36
  DISPLAY "You are sick"
ELSE
  DISPLAY "You are healthy"
END IF
```

## Example 2

Kembangkan kode program pada contoh sebelumnya. Apabila uang yang dimiliki orang tersebut kurang dari 1000000, maka tampilkan `You cannot do swab test`. Jika tidak, maka yang ditampilkan adalah `You should do swab test`. Pemeriksaan uang hanya dilakukan jika suhu tubuh orang tersebut lebih dari 36 derajat.

```
STORE temprature WITH ANY NUMBER
STORE money WITH ANY NUMBER

IF temprature MORE THAN 36
  DISPLAY "You are sick"
ELSE
  DISPLAY "You are healthy"
END IF

IF money LESS THAN 1000000 AND temprature MORE THAN 36
  DISPLAY "You cannot do swab test"
ELSE IF money MORE THAN EQUAL 1000000 AND temprature MORE THAN 36
  DISPLAY "You should do swab test"
END IF
```

# Pseudocode Note 2

## Switch-Case

```
SWITCH namaVariable
  CASE nilai1
    ...
  CASE nilai2
    ...
  CASE nilai3
    ...
END SWITCH
```

## For Loop

```
FOR i FROM 0 TO 9 INCREMENT BY 1
  DISPLAY 'Hello'
END FOR
```

## While Loop

```
STORE i WITH 0
WHILE i LESS THAN 10
  DISPLAY 'Hello'
  SET i WITH i PLUS 1
END WHILE
```

## Do-While Loop

```
STORE i WITH 0
DO
  DISPLAY 'Hello'
  SET i WITH i PLUS 1
WHILE i LESS THAN 10
```

## Break

```
STORE i WITH 1

WHILE i LESS THAN 100
  DISPLAY i
  IF i MODULUS BY 25 EQUAL 0
    DISPLAY 'Kelipatan 25 sudah ketemu'
    BREAK
  END IF
  SET i TO i PLUS 1
END WHILE
```

## Length and Indexing

```
STORE input WITH 'Nama saya Acong'

// Menampilkan panjang dari input
DISPLAY LENGTH OF input

// Mengakses huruf pertama pada input
DISPLAY input[0]

// Mengakses huruf terakhir pada input
DISPLAY input[LENGTH OF input]

// Mengakses huruf ke-n pada input
DISPLAY input[1] // Huruf ke 2
DISPLAY input[2] // Huruf ke 3
```

## Built-in Function

```
// Contoh Math.random
SET variableName WITH RANDOM NUMBER BETWEEN 0 AND 10

// Contoh Math.round
SET variableName WITH ROUND OF variableName

// Contoh Math.floor
SET variableName WITH ROUND DOWN OF variableName

// Contoh Math.ceil
SET variableName WITH ROUND UP OF variableName
```

Penulisan built-in function lainnya yang tidak disebutkan, bisa meniru gaya penulisan di atas.

# Pseudocode Note 3

## Function

```javascript
function penambahan(angka1, angka2) {
  let hasil = angka1 + angka2;
  return hasil
}
```

```
BEGIN penambahan
  PASS IN: angka1 AS NUMBER, angka2 AS NUMBER
  STORE hasil AS NUMBER WITH 0
  SET hasil TO angka1 PLUS angka2
  PASS OUT: hasil
END
```

## Array

### Deklarasi

```
// Deklarasi dan assignment array
STORE arr1 WITH [10, 20, 'A', 'B']
STORE arr2 AS ARRAY WITH [10, 20, 'A', 'B']
```

### Looping and Indexing

```
STORE arr WITH [10, 20, 'A', 'B']

FOR i FROM 0 TO (LENGTH OF arr MINUS 1) INCREMENT BY 1
  DISPLAY arr[i]
END FOR
```

### Push

```
STORE arr WITH []

PUSH 10 TO arr
PUSH 20 TO arr
PUSH 'A' TO arr
PUSH 'B' TO arr
```
