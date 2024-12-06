**Materi Perkuliahan Algoritma Pemrograman: Pengenalan Teknik Perulangan & Penggunaan Perulangan `for`**

---

### **1. Pengenalan Teknik Perulangan (Looping)**
Perulangan (looping) adalah salah satu konsep dasar dalam algoritma pemrograman yang memungkinkan kita untuk menjalankan sekelompok instruksi berulang kali berdasarkan kondisi tertentu. Dengan menggunakan perulangan, kita dapat mengeksekusi blok kode secara efisien, tanpa perlu menulis ulang kode yang sama berulang-ulang.

#### **Jenis-jenis Perulangan**
Di dalam pemrograman, terdapat beberapa jenis perulangan yang umum digunakan:

1. **Perulangan `for`**  
   Digunakan ketika jumlah iterasi sudah diketahui sebelumnya, atau untuk mengulang proses sejumlah waktu tertentu.

2. **Perulangan `while`**  
   Digunakan ketika jumlah iterasi tidak diketahui sebelumnya, dan hanya akan berhenti saat kondisi yang ditentukan terpenuhi.

3. **Perulangan `do-while`**  
   Mirip dengan `while`, tetapi perulangan dimulai terlebih dahulu sebelum memeriksa kondisi, jadi setidaknya satu iterasi pasti terjadi.

Namun, pada materi ini kita akan fokus pada **perulangan `for`**.

---

### **2. Perulangan `for`**
Perulangan `for` digunakan untuk mengulang blok kode dengan jumlah iterasi yang sudah ditentukan. Struktur umum dari perulangan `for` adalah sebagai berikut:

```python
for variabel in range(start, stop, step):
    # Blok kode yang akan diulang
```

- **start**: Nilai awal dari variabel loop. (opsional, default adalah 0)
- **stop**: Batas akhir loop (nilai ini tidak akan diproses, hanya sampai sebelum nilai ini tercapai).
- **step**: Langkah kenaikan untuk variabel loop. (opsional, default adalah 1)

#### **Contoh Penggunaan Perulangan `for`:**
1. **Mencetak Angka 1 sampai 5**
   
   ```python
   for i in range(1, 6):
       print(i)
   ```

   **Penjelasan**:
   - `range(1, 6)` berarti variabel `i` dimulai dari 1 hingga 5 (6 tidak termasuk).
   - Program ini akan mencetak angka 1 sampai 5.

   **Output**:
   ```
   1
   2
   3
   4
   5
   ```

2. **Mencetak Angka Genap dari 0 hingga 10**
   
   ```python
   for i in range(0, 11, 2):
       print(i)
   ```

   **Penjelasan**:
   - `range(0, 11, 2)` berarti variabel `i` dimulai dari 0 dan naik 2 setiap kali (menampilkan angka genap).
   - Program ini akan mencetak angka genap dari 0 hingga 10.

   **Output**:
   ```
   0
   2
   4
   6
   8
   10
   ```

3. **Menggunakan Perulangan `for` untuk Menghitung Total Nilai dalam List**
   
   ```python
   numbers = [10, 20, 30, 40, 50]
   total = 0

   for num in numbers:
       total += num

   print("Total nilai:", total)
   ```

   **Penjelasan**:
   - Dalam contoh ini, program menggunakan perulangan `for` untuk menjumlahkan nilai dalam list `numbers`.
   - Setiap elemen dalam list akan ditambahkan ke variabel `total`.
   
   **Output**:
   ```
   Total nilai: 150
   ```

#### **Pentingnya Perulangan `for`**
- **Efisiensi**: Dengan perulangan `for`, kita dapat mengulang sebuah proses sebanyak yang kita inginkan tanpa menulis kode yang berulang-ulang.
- **Kemudahan dalam pengolahan data**: Misalnya dalam pengolahan array atau list, perulangan `for` sangat membantu untuk memproses setiap elemen secara otomatis.

---

### **3. Studi Kasus**
Berikut ini adalah beberapa contoh soal yang menggunakan perulangan `for`:

#### **Soal 1**: Menampilkan Deret Bilangan Fibonacci
Fibonacci adalah deret bilangan di mana setiap angka adalah jumlah dari dua angka sebelumnya, dimulai dengan 0 dan 1. Misalnya: 0, 1, 1, 2, 3, 5, 8, 13, dst.

Buatlah program untuk menampilkan deret Fibonacci sebanyak `n` angka.

```python
n = int(input("Masukkan jumlah angka Fibonacci: "))
a, b = 0, 1

for _ in range(n):
    print(a, end=" ")
    a, b = b, a + b
```

**Penjelasan**:
- Program ini akan mencetak deret Fibonacci sebanyak `n` angka.
- Variabel `a` dan `b` adalah dua angka yang dimulai dengan 0 dan 1, yang kemudian diperbarui dengan cara `a, b = b, a + b`.

#### **Soal 2**: Menentukan Bilangan Prima
Tulislah program yang dapat memeriksa apakah sebuah angka adalah bilangan prima atau bukan.

```python
number = int(input("Masukkan angka: "))
is_prime = True

for i in range(2, number):
    if number % i == 0:
        is_prime = False
        break

if is_prime and number > 1:
    print(number, "adalah bilangan prima.")
else:
    print(number, "bukan bilangan prima.")
```

**Penjelasan**:
- Program ini memeriksa apakah angka yang dimasukkan habis dibagi dengan angka lain selain 1 dan dirinya sendiri.
- Jika angka tersebut dapat dibagi oleh angka lain, maka angka tersebut bukan bilangan prima.

---

### **4. Praktikum**
Sebagai tugas praktikum, mahasiswa dapat diminta untuk mengimplementasikan beberapa contoh soal berikut menggunakan perulangan `for`:

1. Menampilkan deret angka ganjil dari 1 hingga 20.
2. Menghitung jumlah semua angka dalam list yang diberikan oleh pengguna.
3. Menampilkan pola bintang segitiga terbalik, misalnya:
   ```
   *****
   ****
   ***
   **
   *
   ```

---

### **5. Kesimpulan**
Perulangan `for` adalah alat yang sangat berguna dalam pemrograman, terutama saat kita membutuhkan pengulangan yang terstruktur. Dengan menggunakan perulangan ini, kita dapat menghemat waktu dan menulis kode yang lebih efisien. Sebagai tambahan, penting bagi mahasiswa untuk berlatih dengan berbagai contoh agar lebih memahami cara kerja perulangan dalam algoritma pemrograman.

---

**Referensi**:
1. "Python Programming: An Introduction to Computer Science" oleh John Zelle.
2. Dokumentasi Python: https://docs.python.org/3/

---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)