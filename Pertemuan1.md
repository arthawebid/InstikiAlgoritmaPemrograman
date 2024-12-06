Berikut adalah materi perkuliahan tentang **Algoritma Pemrograman** dengan fokus pada **Pengenalan Algoritma**, **Pemetaan Algoritma ke dalam Bahasa Pemrograman**, dan **Pengenalan Bahasa Pemrograman Python**:

---

### **Mata Kuliah: Algoritma Pemrograman**

#### **Topik: Pengenalan Algoritma**

**Definisi Algoritma**:
Algoritma adalah sekumpulan langkah-langkah yang jelas dan terstruktur untuk menyelesaikan suatu masalah. Algoritma harus memiliki input, proses yang jelas, dan output yang diinginkan. 

**Karakteristik Algoritma**:
1. **Input**: Algoritma menerima satu atau lebih input dari luar.
2. **Output**: Algoritma menghasilkan output atau solusi terhadap masalah.
3. **Definiteness**: Setiap langkah dalam algoritma harus jelas dan tidak ambigu.
4. **Finiteness**: Algoritma harus berhenti setelah sejumlah langkah tertentu.
5. **Effectiveness**: Langkah-langkah dalam algoritma harus cukup sederhana sehingga dapat dilakukan dengan alat yang ada.

**Contoh Algoritma Sederhana**:
Algoritma untuk menjumlahkan dua angka:
1. Ambil dua angka sebagai input (misalnya `a` dan `b`).
2. Jumlahkan kedua angka: `c = a + b`.
3. Tampilkan hasil `c` sebagai output.

**Pseudocode**:
Pseudocode adalah cara untuk menggambarkan algoritma secara jelas tanpa menggunakan sintaks bahasa pemrograman tertentu. Ini adalah representasi algoritma dalam bahasa yang mudah dipahami manusia.

**Contoh Pseudocode**:
```
BEGIN
    INPUT a, b
    c = a + b
    OUTPUT c
END
```

**Diagram Alir (Flowchart)**:
Flowchart adalah diagram grafis yang menggambarkan langkah-langkah dalam suatu algoritma menggunakan simbol-simbol tertentu.
- **Oval**: menunjukkan awal dan akhir algoritma.
- **Persegi panjang**: menunjukkan langkah-langkah proses.
- **Belah ketupat**: menunjukkan keputusan atau percabangan.

---

#### **Topik: Pemetaan Algoritma ke dalam Bahasa Pemrograman**

Setelah kita memahami algoritma, langkah berikutnya adalah memetakan algoritma tersebut ke dalam bahasa pemrograman. Setiap bahasa pemrograman memiliki sintaks dan struktur yang berbeda, namun prinsip dasar dalam memetakan algoritma tetap sama.

**Langkah-langkah Pemrograman**:
1. **Definisikan Masalah**: Tentukan masalah yang akan diselesaikan.
2. **Tulis Algoritma**: Buat algoritma dalam bentuk pseudocode atau flowchart.
3. **Pilih Bahasa Pemrograman**: Tentukan bahasa pemrograman yang akan digunakan untuk implementasi.
4. **Tulis Kode**: Implementasikan algoritma dalam kode program menggunakan sintaks bahasa yang dipilih.
5. **Uji dan Debug**: Jalankan program untuk memeriksa apakah hasilnya sesuai dengan yang diinginkan, dan perbaiki jika ada kesalahan.

**Contoh Pemrograman dalam Python**:
Misalkan kita ingin menulis algoritma untuk menjumlahkan dua angka. Dalam bahasa Python, pemetaan algoritma tersebut adalah sebagai berikut:

**Pseudocode**:
```
BEGIN
    INPUT a, b
    c = a + b
    OUTPUT c
END
```

**Implementasi dalam Python**:
```python
# Mengambil input dari pengguna
a = float(input("Masukkan angka pertama: "))
b = float(input("Masukkan angka kedua: "))

# Menjumlahkan kedua angka
c = a + b

# Menampilkan hasil
print("Hasil penjumlahan: ", c)
```

---

#### **Topik: Pengenalan Bahasa Pemrograman Python**

**Apa itu Python?**
Python adalah bahasa pemrograman tingkat tinggi yang sangat populer karena sintaksnya yang sederhana dan kemampuannya untuk digunakan dalam berbagai jenis pengembangan perangkat lunak, dari pengembangan web hingga analisis data dan kecerdasan buatan (AI).

**Keunggulan Python**:
1. **Sintaks yang Sederhana**: Python mudah dibaca dan dipelajari, menjadikannya pilihan yang baik bagi pemula.
2. **Berkas Standard Library yang Luas**: Python memiliki banyak modul dan pustaka standar yang mempermudah pengembangan.
3. **Kompatibilitas yang Baik**: Python dapat berjalan di berbagai platform, seperti Windows, Linux, dan macOS.
4. **Interaktif**: Python menyediakan interpreter interaktif untuk pengujian kode secara langsung.

**Struktur Dasar Program Python**:
Berikut adalah contoh program Python yang paling dasar:

```python
# Program Python pertama
print("Hello, World!")
```

**Sintaks Dasar Python**:
1. **Variabel**:
   Di Python, kita tidak perlu mendeklarasikan tipe data secara eksplisit. Python akan menentukannya secara otomatis.
   ```python
   x = 10       # integer
   y = 3.14     # float
   name = "John"  # string
   ```

2. **Kontrol Alur (Flow Control)**:
   - **Percabangan (If-else)**:
     ```python
     if x > 5:
         print("X lebih besar dari 5")
     else:
         print("X kurang dari atau sama dengan 5")
     ```
   - **Perulangan (Looping)**:
     ```python
     # Perulangan for
     for i in range(5):
         print(i)

     # Perulangan while
     count = 0
     while count < 5:
         print(count)
         count += 1
     ```

3. **Fungsi**:
   Fungsi di Python didefinisikan dengan kata kunci `def`:
   ```python
   def tambah(a, b):
       return a + b

   hasil = tambah(3, 4)
   print(hasil)
   ```

4. **List dan Tuple**:
   - **List** adalah struktur data yang bisa berubah-ubah.
     ```python
     fruits = ["apple", "banana", "cherry"]
     fruits.append("orange")
     ```
   - **Tuple** adalah struktur data yang tidak bisa diubah (immutable).
     ```python
     coordinates = (10, 20, 30)
     ```

**Modul dan Pustaka**:
Python memiliki banyak pustaka standar untuk berbagai kebutuhan seperti matematika, manipulasi string, dan akses file. Contoh penggunaan pustaka math untuk perhitungan matematika:

```python
import math

# Menggunakan pustaka math untuk menghitung akar kuadrat
x = math.sqrt(16)
print(x)
```

---

### **Kesimpulan**

- **Algoritma** adalah langkah-langkah sistematis untuk memecahkan masalah.
- **Pemetaan algoritma ke dalam bahasa pemrograman** melibatkan penerjemahan algoritma ke dalam kode yang dapat dieksekusi oleh komputer.
- **Python** adalah bahasa pemrograman yang sangat cocok untuk pemula, dengan sintaks sederhana dan pustaka yang luas.

---

### **Tugas dan Latihan**
1. Buatlah algoritma untuk menghitung faktorial dari sebuah angka menggunakan pseudocode dan implementasikan dalam Python.
2. Implementasikan program Python yang menerima dua angka dan mencetak hasil perkalian dari kedua angka tersebut.
3. Pelajari penggunaan perulangan dan kondisi dalam Python, lalu buat program yang menentukan apakah suatu angka adalah bilangan prima.

---

Semoga materi ini bermanfaat dan memberikan pemahaman yang jelas tentang dasar-dasar algoritma dan pemrograman Python!


---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)