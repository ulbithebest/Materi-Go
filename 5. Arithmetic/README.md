# Materi Aritmatika dan Bangun Datar di Go

Aritmatika adalah operasi dasar dalam matematika yang mencakup penjumlahan, pengurangan, perkalian, pembagian, dan lainnya. Dalam materi ini, kita akan membahas:
1. Dasar Operasi Aritmatika.
2. Rumus-rumus luas bangun datar: Persegi, Persegi Panjang, Segitiga, dan Lingkaran.

---

## **Materi Awal: Dasar Operasi Aritmatika**

### Operasi Dasar:
- **Penjumlahan** (`+`)
- **Pengurangan** (`-`)
- **Perkalian** (`*`)
- **Pembagian** (`/`)
- **Modulus** (`%`) (khusus bilangan bulat)

### Kode Contoh:
```go
package main

import "fmt"

func main() {
    a := 10
    b := 3

    fmt.Println("Penjumlahan:", a+b)
    fmt.Println("Pengurangan:", a-b)
    fmt.Println("Perkalian:", a*b)
    fmt.Println("Pembagian:", a/b)
    fmt.Println("Modulus:", a%b)
}
```
Output:
 
![alt text](https://github.com/ghaidafasya24/img/blob/main/aritmatika.png?raw=true)

## **Materi Lanjutan: Rumus Luas Bangun Datar**

Berikut adalah program untuk menghitung luas bangun datar menggunakan operasi aritmatika.

### 1. Luas Persegi

**Rumus : L=s×s**

### Contoh Kode:
```go
package main

import "fmt"

func main() {
    var sisi float64
    fmt.Print("Masukkan panjang sisi: ")
    fmt.Scan(&sisi)

    luas := sisi * sisi
    fmt.Printf("Luas persegi adalah: %.2f\n", luas)
}
```

Output:

Kita masukkan panjang sisinya terlebih dahulu, sebagai contoh:

![alt text](https://github.com/ghaidafasya24/img/blob/main/persegi1.png?raw=true)

Berikut merupakan hasil dari luas persegi:

![alt text](https://github.com/ghaidafasya24/img/blob/main/persegi2.png?raw=true)


### 2. Luas Persegi Panjang

**Rumus : L=p×l**

### Contoh Kode:
```go
package main

import "fmt"

func main() {
    var panjang, lebar float64
    fmt.Print("Masukkan panjang: ")
    fmt.Scan(&panjang)
    fmt.Print("Masukkan lebar: ")
    fmt.Scan(&lebar)

    luas := panjang * lebar
    fmt.Printf("Luas persegi panjang adalah: %.2f\n", luas)
}
```

Output:

Kita masukan terlebih dahulu panjang dan lebarnya, sebagai contoh:

![alt text](https://github.com/ghaidafasya24/img/blob/main/persegipanjang1.png?raw=true)

Berikut merupakan luas persegi panjangnya:

![alt text](https://github.com/ghaidafasya24/img/blob/main/persegipanjang2.png?raw=true)


### 3. Luas Lingkaran

**Rumus : L=π×r×r**
Catatan: π ≈ 3.14

### Contoh Kode:
```go
package main

import "fmt"

func main() {
    const pi = 3.14
    var radius float64
    fmt.Print("Masukkan jari-jari: ")
    fmt.Scan(&radius)

    luas := pi * radius * radius
    fmt.Printf("Luas lingkaran adalah: %.2f\n", luas)
}
```

Output:

![alt text](https://github.com/ghaidafasya24/img/blob/main/lingkaran1.png?raw=true)

![alt text](https://github.com/ghaidafasya24/img/blob/main/lingkaran2.png?raw=true)

## **Kesimpulan**

- Operasi aritmatika di Go sangat sederhana dan mendukung berbagai perhitungan matematika.
- Dengan pemahaman dasar, kita dapat menghitung luas berbagai bangun datar seperti persegi, persegi panjang dan    lingkaran.
- Anda dapat mengembangkan materi ini untuk mendukung bangun datar lainnya atau menambahkan validasi input.
