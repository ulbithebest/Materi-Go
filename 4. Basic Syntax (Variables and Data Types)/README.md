## Sintaks Dasar: Variabel dan Tipe Data

Berikut ini adalah program sederhana untuk mendeklarasikan variabel dan tipe data di Go:

## Variabel
- **Deklarasi Biasa**: Menggunakan `var`.
- **Deklarasi Cepat**: Menggunakan `:=`.

Contoh:
```go
var nama string = "Budi"
umur := 20
```
## Tipe Data 
- **String**: `string`
- **Integer**: `int`, `int8`, `int16`, `int32`, `int64`
- **Floating-point**: `float32`, `float64`
- **Boolean**: `bool`

#### 1. String
Berikut merupakan contoh penggunaan dari String
```go
package main

import "fmt"

func main() {
    // Deklarasi String
    var firstName string = "John"       // Deklarasi dengan var
    lastName := "Doe"                   // Deklarasi cepat
    fullName := firstName + " " + lastName // Menggabungkan string

    // Output
    fmt.Println("Full Name:", fullName) // Output: Full Name: John Doe

    // Panjang String
    fmt.Println("Length of fullName:", len(fullName)) // Output panjang string

    // Akses karakter dalam string
    fmt.Println("First letter of fullName:", string(fullName[0]))
}
```
 Output:
 
![alt text](https://github.com/ghaidafasya24/img/blob/main/penggunaan%20string.png?raw=true)

#### 2. Integer
Berikut merupakan contoh penggunaan dari Integer
 ```go
package main

import "fmt"

func main() {
    // Deklarasi Integer
    var age int = 25                    // Integer default
    var smallNumber int8 = 100          // Integer 8-bit
    var mediumNumber int16 = 1000       // Integer 16-bit
    var largeNumber int64 = 1000000000  // Integer 64-bit

    // Output
    fmt.Printf("Age: %d\nSmall: %d\nMedium: %d\nLarge: %d\n", age, smallNumber, mediumNumber, largeNumber)

    // Operasi Matematika
    total := int(smallNumber) + age // Konversi tipe data
    fmt.Println("Total (smallNumber + age):", total)

    // Modulus
    fmt.Println("Modulus (age %% 7):", age%7)
}
```
 Output:
 
![alt text](https://github.com/ghaidafasya24/img/blob/main/penggunaan_int.png?raw=true)

#### 3. Floating-poin
Berikut merupakan contoh penggunaan dari Float
```go
package main

import "fmt"

func main() {
    // Deklarasi Floating-point
    var pi float32 = 3.14159   // Floating-point 32-bit
    var gravity float64 = 9.81 // Floating-point 64-bit

    // Output
    fmt.Printf("Pi: %.2f\nGravity: %.2f\n", pi, gravity)

    // Operasi Matematika
    radius := 5.0
    area := pi * float32(radius*radius) // Konversi tipe data
    fmt.Printf("Area of circle: %.2f\n", area)

    // Pembagian Floating-point
    result := gravity / 2
    fmt.Printf("Gravity / 2: %.2f\n", result)
}
```
Output:

![alt text](https://github.com/ghaidafasya24/img/blob/main/penggunaan%20float.png?raw=true)

#### 4. Boolean
Berikut merupakan contoh penggunaan dari Boolean
```go
package main

import "fmt"

func main() {
    var isGoFun bool = true
    fmt.Println(isGoFun) // Output: true
}
```
Output:
 
![alt text](https://github.com/ghaidafasya24/img/blob/main/penggunaan%20bool.png?raw=true)
