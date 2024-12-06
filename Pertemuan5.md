Berikut adalah materi perkuliahan untuk topik **"Konsep Tipe Data String, Operator Tipe Data String, dan Fungsi String pada Python"** dalam mata kuliah Algoritma Pemrograman:

---

## **Materi Perkuliahan: Tipe Data String pada Python**

### 1. **Konsep Tipe Data String**
Tipe data **string** adalah salah satu tipe data dasar yang digunakan untuk menyimpan sekumpulan karakter. Di Python, string dapat berupa satu karakter, satu kata, atau kalimat panjang. String dikelilingi oleh tanda kutip tunggal (`'`) atau tanda kutip ganda (`"`), dan Python memperlakukan keduanya secara identik.

#### Contoh:
```python
# Menggunakan tanda kutip tunggal
s = 'Hello, World!'

# Menggunakan tanda kutip ganda
s2 = "Python Programming"

# String dengan tanda kutip tripel (untuk teks multi-baris)
s3 = '''Ini adalah
contoh string
multi-baris.'''
```

#### Karakter dalam String
- Setiap karakter dalam string diindeks mulai dari 0, dan indeks negatif dimulai dari -1 (dari belakang).
- String adalah **immutable**, artinya setelah string dibuat, kita tidak dapat mengubah karakter-karakter di dalamnya.

#### Contoh Indeks:
```python
s = "Hello"
print(s[0])  # H
print(s[-1])  # o
```

### 2. **Operator Tipe Data String**
Tipe data string mendukung berbagai operator untuk manipulasi string.

#### a. **Operator Penambahan (Concatenation)**
Operator `+` digunakan untuk menggabungkan dua string menjadi satu string.

```python
s1 = "Hello"
s2 = "World"
s3 = s1 + " " + s2  # Gabung dengan spasi
print(s3)  # Output: Hello World
```

#### b. **Operator Perkalian (Repetition)**
Operator `*` digunakan untuk mengulang string sejumlah n kali.

```python
s = "Python"
print(s * 3)  # Output: PythonPythonPython
```

#### c. **Operator Pengindeksan dan Pemotongan (Slicing)**
Operator `[]` digunakan untuk mengakses karakter berdasarkan indeks atau untuk melakukan pemotongan (slicing).

```python
s = "Python"
print(s[0])  # Output: P (mengambil karakter pertama)
print(s[1:4])  # Output: yth (karakter dari indeks 1 hingga 3)
print(s[:3])  # Output: Pyt (karakter dari awal hingga indeks 2)
print(s[3:])  # Output: hon (karakter dari indeks 3 hingga akhir)
```

#### d. **Operator In dan Not In**
Operator `in` digunakan untuk memeriksa apakah suatu substring ada dalam string, sedangkan `not in` digunakan untuk memeriksa kebalikannya.

```python
s = "Hello, World!"
print("Hello" in s)  # Output: True
print("Python" not in s)  # Output: True
```

### 3. **Fungsi String pada Python**
Python menyediakan berbagai fungsi built-in untuk bekerja dengan string. Berikut adalah beberapa fungsi string yang sering digunakan.

#### a. **`len()`**
Fungsi ini digunakan untuk menghitung panjang string (jumlah karakter dalam string).

```python
s = "Hello, World!"
print(len(s))  # Output: 13
```

#### b. **`upper()` dan `lower()`**
Fungsi ini digunakan untuk mengubah semua karakter dalam string menjadi huruf besar (`upper()`) atau huruf kecil (`lower()`).

```python
s = "Hello"
print(s.upper())  # Output: HELLO
print(s.lower())  # Output: hello
```

#### c. **`strip()`**
Fungsi ini digunakan untuk menghapus karakter spasi (atau karakter lain yang ditentukan) dari awal dan akhir string.

```python
s = "   Hello   "
print(s.strip())  # Output: Hello
```

#### d. **`replace()`**
Fungsi ini digunakan untuk mengganti bagian tertentu dari string dengan substring yang baru.

```python
s = "Hello, World!"
print(s.replace("World", "Python"))  # Output: Hello, Python!
```

#### e. **`split()`**
Fungsi ini digunakan untuk memecah string menjadi sebuah list berdasarkan pemisah yang diberikan (default adalah spasi).

```python
s = "Python is awesome"
print(s.split())  # Output: ['Python', 'is', 'awesome']
```

#### f. **`find()`**
Fungsi ini digunakan untuk mencari posisi pertama dari substring dalam string. Jika substring tidak ditemukan, fungsi ini akan mengembalikan nilai `-1`.

```python
s = "Hello, World!"
xprint(s.find("World"))  # Output: 7
print(s.find("Python"))  # Output: -1
```

#### g. **`join()`**
Fungsi ini digunakan untuk menggabungkan elemen-elemen dalam iterable (seperti list) menjadi satu string dengan pemisah yang ditentukan.

```python
words = ["Hello", "World", "Python"]
print(" ".join(words))  # Output: Hello World Python
```

#### h. **`count()`**
Fungsi ini digunakan untuk menghitung jumlah kemunculan substring dalam string.

```python
s = "Hello, Hello, Hello"
print(s.count("Hello"))  # Output: 3
```

#### i. **`isalnum()`, `isalpha()`, `isdigit()`**
- **`isalnum()`**: Memeriksa apakah string hanya mengandung alfanumerik (huruf dan angka).
- **`isalpha()`**: Memeriksa apakah string hanya mengandung huruf.
- **`isdigit()`**: Memeriksa apakah string hanya mengandung angka.

```python
s = "123abc"
print(s.isalnum())  # Output: True
print(s.isalpha())  # Output: False
print(s.isdigit())  # Output: False
```

---

### 4. **Latihan dan Tugas**
- **Latihan 1**: Buatlah program yang meminta input nama pengguna dan mengubahnya menjadi format judul (menggunakan fungsi `title()`).
- **Latihan 2**: Buatlah fungsi yang menerima sebuah kalimat dan menghitung berapa banyak kata "Python" yang muncul dalam kalimat tersebut.
- **Tugas**: Buatlah sebuah program yang menggabungkan dua string dengan format tertentu, misalnya menggabungkan nama depan dan nama belakang dan mencetaknya dalam format "Nama Lengkap: [Nama Depan] [Nama Belakang]".

---

Dengan materi di atas, mahasiswa diharapkan dapat memahami konsep dasar string dalam Python, serta menguasai berbagai operator dan fungsi yang sering digunakan untuk manipulasi string.

---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)