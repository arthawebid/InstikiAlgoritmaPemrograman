Berikut adalah materi perkuliahan algoritma pemrograman dengan topik **Pengenalan Array 1 Dimensi**, **Indeks dan Value Array 1 Dimensi**, serta **Mengakses & Mengisi Array 1 Dimensi**:

---

## **Pengenalan Array 1 Dimensi**

### 1. **Pengertian Array**

Array adalah struktur data yang digunakan untuk menyimpan sekumpulan nilai dengan tipe data yang sama. Elemen-elemen dalam array disusun secara berurutan dan masing-masing elemen memiliki indeks yang unik. Array 1 dimensi berarti array yang hanya memiliki satu baris atau satu deretan elemen.

Contoh: 
- Jika kita ingin menyimpan 5 angka dalam satu variabel, kita bisa menggunakan array untuk menyimpannya.

### 2. **Struktur Array 1 Dimensi**
Array 1 dimensi dapat dianggap sebagai kumpulan data yang disusun secara linear (seperti daftar) dalam memori. Setiap elemen dalam array memiliki posisi atau indeks tertentu.

Contoh deklarasi array dalam beberapa bahasa pemrograman:
- **Java**:
  ```java
  int[] array = new int[5];
  ```
- **C++**:
  ```cpp
  int array[5];
  ```
- **Python** (menggunakan list):
  ```python
  array = [0, 0, 0, 0, 0]
  ```

### 3. **Karakteristik Array**
- **Ukuran Tetap**: Setelah deklarasi, ukuran array tidak dapat diubah.
- **Elemen Bertipe Sama**: Semua elemen dalam array memiliki tipe data yang sama.
- **Urutan Indeks**: Elemen array diakses berdasarkan indeksnya.

---

## **Indeks dan Value Array 1 Dimensi**

### 1. **Indeks Array**

Indeks adalah posisi elemen dalam array. Indeks array dimulai dari angka 0. Misalnya, array yang berisi 5 elemen, elemen pertama memiliki indeks 0, elemen kedua memiliki indeks 1, dan seterusnya.

Contoh:
- **Array**: `array = [10, 20, 30, 40, 50]`
- **Indeks**: 0  1  2  3  4

### 2. **Value Array**

Value atau nilai adalah data yang disimpan dalam elemen array. Setiap elemen array menyimpan nilai yang dapat berupa angka, karakter, atau tipe data lainnya.

Contoh:
- Pada array `array = [10, 20, 30, 40, 50]`, nilai (value) dari elemen dengan indeks 0 adalah `10`, nilai dari indeks 1 adalah `20`, dan seterusnya.

---

## **Mengakses & Mengisi Array 1 Dimensi**

### 1. **Mengakses Elemen Array**

Mengakses elemen array dilakukan dengan menyebutkan nama array diikuti oleh indeks yang ingin diakses dalam tanda kurung siku `[]`.

Contoh:
- Untuk mengakses elemen pertama (dengan indeks 0) dari array `array = [10, 20, 30, 40, 50]`:
  - **Java**:
    ```java
    int value = array[0]; // value = 10
    ```
  - **C++**:
    ```cpp
    int value = array[0]; // value = 10
    ```
  - **Python**:
    ```python
    value = array[0] # value = 10
    ```

### 2. **Mengisi Array**

Array dapat diisi dengan cara menetapkan nilai-nilai ke dalam elemen array dengan menggunakan indeks.

#### Cara Mengisi Elemen Array:
- **Java**:
  ```java
  array[0] = 10; // Mengisi elemen pertama dengan nilai 10
  array[1] = 20; // Mengisi elemen kedua dengan nilai 20
  ```
- **C++**:
  ```cpp
  array[0] = 10; // Mengisi elemen pertama dengan nilai 10
  array[1] = 20; // Mengisi elemen kedua dengan nilai 20
  ```
- **Python**:
  ```python
  array[0] = 10  # Mengisi elemen pertama dengan nilai 10
  array[1] = 20  # Mengisi elemen kedua dengan nilai 20
  ```

### 3. **Contoh Program Pengisian dan Pengaksesan Array**

#### Contoh Program C++:
```cpp
#include <iostream>
using namespace std;

int main() {
    // Deklarasi array dengan 5 elemen
    int array[5];
    
    // Mengisi array dengan nilai
    array[0] = 10;
    array[1] = 20;
    array[2] = 30;
    array[3] = 40;
    array[4] = 50;

    // Mengakses dan menampilkan nilai array
    for (int i = 0; i < 5; i++) {
        cout << "Element ke-" << i + 1 << ": " << array[i] << endl;
    }

    return 0;
}
```

Output:
```
Element ke-1: 10
Element ke-2: 20
Element ke-3: 30
Element ke-4: 40
Element ke-5: 50
```

#### Contoh Program Python:
```python
# Deklarasi array dengan 5 elemen
array = [0, 0, 0, 0, 0]

# Mengisi array dengan nilai
array[0] = 10
array[1] = 20
array[2] = 30
array[3] = 40
array[4] = 50

# Mengakses dan menampilkan nilai array
for i in range(5):
    print(f"Element ke-{i + 1}: {array[i]}")
```

Output:
```
Element ke-1: 10
Element ke-2: 20
Element ke-3: 30
Element ke-4: 40
Element ke-5: 50
```

---

### **Kesimpulan**
- **Array 1 dimensi** adalah struktur data yang menyimpan sekumpulan data dengan tipe yang sama dalam urutan yang berkelanjutan.
- **Indeks** dimulai dari 0, dan setiap elemen array dapat diakses dengan indeksnya.
- **Value** adalah nilai yang disimpan dalam array dan dapat diubah atau diakses menggunakan indeks.
- Untuk mengakses atau mengisi array, kita menggunakan indeks yang sesuai dengan posisi elemen dalam array tersebut.

Dengan pemahaman ini, Anda dapat mulai memanipulasi array untuk berbagai kebutuhan dalam algoritma pemrograman.


---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)