Berikut adalah materi perkuliahan mengenai **Penggunaan Komentar, Pengenalan Input dan Output dalam Bahasa Pemrograman Python** yang dapat digunakan untuk mempelajari dasar-dasar pemrograman Python.

---

### **Materi Perkuliahan: Algoritma Pemrograman**
#### **1. Penggunaan Komentar dalam Python**

Komentar adalah teks atau informasi yang ditambahkan dalam kode program yang tidak akan dieksekusi oleh komputer. Komentar digunakan untuk memberikan penjelasan tentang bagian-bagian tertentu dari kode untuk memudahkan pembaca dalam memahami program.

##### **Jenis Komentar di Python**
- **Komentar Satu Baris**: Komentar yang hanya menjelaskan satu baris kode. Komentar ini dimulai dengan tanda `#`.
  - **Contoh**:
    ```python
    # Ini adalah komentar satu baris
    x = 10  # Menyimpan nilai 10 dalam variabel x
    ```

- **Komentar Multibaris**: Komentar yang menjelaskan beberapa baris kode sekaligus. Komentar multibaris biasanya dibungkus oleh tanda triple quote (`'''` atau `"""`).
  - **Contoh**:
    ```python
    '''
    Ini adalah komentar multibaris.
    Komentar ini dapat menjelaskan lebih dari satu baris kode.
    Biasanya digunakan untuk dokumentasi atau penjelasan panjang.
    '''
    y = 20
    ```

##### **Tujuan Penggunaan Komentar**:
- Menjelaskan kode yang kompleks atau rumit.
- Memberikan penjelasan tentang tujuan dan fungsi suatu bagian dari program.
- Membantu pengembang lain memahami kode yang ditulis.

#### **2. Pengenalan Input dan Output dalam Python**

##### **2.1. Pengenalan Output (Mencetak ke Layar)**
Output adalah proses menampilkan data dari program ke layar atau perangkat lainnya. Di Python, perintah yang digunakan untuk menampilkan informasi adalah fungsi `print()`.

- **Sintaks**:
  ```python
  print(ekspresi)
  ```
  - `ekspresi`: Teks, angka, atau data lain yang ingin ditampilkan.

- **Contoh Penggunaan `print()`**:
  ```python
  print("Halo, dunia!")  # Menampilkan teks "Halo, dunia!"
  a = 5
  b = 3
  print(a + b)  # Menampilkan hasil penjumlahan 5 + 3, yaitu 8
  ```

##### **2.2. Pengenalan Input (Memasukkan Data dari Pengguna)**
Input adalah proses untuk mendapatkan data dari pengguna. Di Python, kita menggunakan fungsi `input()` untuk membaca data yang dimasukkan oleh pengguna melalui keyboard.

- **Sintaks**:
  ```python
  variabel = input("Pesan untuk pengguna: ")
  ```
  - `Pesan untuk pengguna`: Teks yang ditampilkan untuk meminta masukan dari pengguna.

- **Contoh Penggunaan `input()`**:
  ```python
  nama = input("Masukkan nama Anda: ")  # Meminta pengguna untuk memasukkan nama
  print("Halo, " + nama + "!")  # Menampilkan nama yang dimasukkan pengguna
  ```

  **Catatan**: Fungsi `input()` selalu mengembalikan nilai dalam bentuk string (teks). Jika kita ingin memasukkan tipe data lain seperti angka, kita perlu mengkonversinya menggunakan fungsi seperti `int()` atau `float()`.

  - **Contoh konversi tipe data**:
    ```python
    umur = input("Masukkan umur Anda: ")
    umur = int(umur)  # Mengonversi input menjadi integer
    print("Umur Anda adalah:", umur)
    ```

#### **3. Contoh Program: Penggunaan Komentar, Input, dan Output**

Berikut adalah contoh program Python yang menggabungkan komentar, input, dan output:

```python
# Program untuk meminta nama dan umur pengguna

# Meminta input nama dari pengguna
nama = input("Masukkan nama Anda: ")

# Meminta input umur dari pengguna
umur = int(input("Masukkan umur Anda: "))

# Menampilkan informasi yang dimasukkan pengguna
print("Halo, " + nama + "!")
print("Anda berusia " + str(umur) + " tahun.")
```

##### **Penjelasan Program**:
1. Program ini meminta pengguna untuk memasukkan nama dan umur mereka.
2. Fungsi `input()` digunakan untuk membaca masukan dari pengguna.
3. Input umur dikonversi menjadi tipe data `int` menggunakan fungsi `int()`.
4. Output ditampilkan menggunakan fungsi `print()`, yang menggabungkan teks dengan data yang dimasukkan oleh pengguna.

---

### **Ringkasan**
1. **Komentar**: Digunakan untuk memberikan penjelasan dalam kode program, memudahkan pemahaman, dan mendokumentasikan program.
   - Komentar satu baris menggunakan tanda `#`.
   - Komentar multibaris menggunakan `'''` atau `"""`.
   
2. **Output**: Fungsi `print()` digunakan untuk menampilkan informasi ke layar.

3. **Input**: Fungsi `input()` digunakan untuk mengambil data dari pengguna. Input selalu berupa string, sehingga perlu dikonversi ke tipe data lain jika diperlukan.

---

### **Latihan**
1. Buatlah program yang meminta pengguna untuk memasukkan dua angka, kemudian menampilkan hasil penjumlahannya.
2. Tambahkan komentar yang menjelaskan langkah-langkah dalam program tersebut.
3. Ubah program tersebut agar dapat menangani pengurangan, perkalian, dan pembagian.

---

Semoga materi ini membantu memahami dasar penggunaan komentar, input, dan output dalam pemrograman Python!


---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)