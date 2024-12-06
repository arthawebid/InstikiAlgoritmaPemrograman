Berikut adalah materi perkuliahan tentang penggunaan perulangan `while` dan `do...while` dalam pemrograman Python:

---

## **Materi Perkuliahan: Penggunaan Perulangan `while` dan `do...while` pada Python**

### **1. Pengertian Perulangan**
Perulangan (loop) adalah salah satu struktur kontrol dalam pemrograman yang digunakan untuk menjalankan suatu blok kode secara berulang-ulang, dengan syarat tertentu yang ditentukan oleh kondisi.

Ada beberapa jenis perulangan yang digunakan dalam Python, di antaranya:
- `while`
- `for`
- `do...while` (tidak ada secara langsung dalam Python, tetapi bisa disimulasikan)

---

### **2. Perulangan `while`**
Perulangan `while` digunakan untuk menjalankan blok kode selama suatu kondisi bernilai `True`. Setelah kondisi menjadi `False`, perulangan akan berhenti.

#### **Sintaks Perulangan `while`**
```python
while kondisi:
    # blok kode yang dijalankan selama kondisi True
```

- **Kondisi** adalah ekspresi yang akan diuji setiap kali sebelum perulangan dimulai.
- **Blok kode** adalah sekumpulan pernyataan yang akan dijalankan selama kondisi bernilai `True`.

#### **Contoh Program Perulangan `while`**
```python
# Program menghitung angka 1 sampai 5 menggunakan while
i = 1
while i <= 5:
    print(i)
    i += 1  # Increment i, supaya perulangan tidak berlangsung selamanya
```
**Penjelasan:**
- Perulangan dimulai dengan nilai `i = 1`.
- Setiap kali perulangan dijalankan, nilai `i` akan dicetak dan kemudian ditambah 1.
- Perulangan berhenti ketika nilai `i` lebih besar dari 5.

#### **Kasus Umum Penggunaan `while`**
- **Menerima input pengguna**: Membaca input hingga pengguna memberikan input yang valid.
- **Pengulangan dengan batas yang tidak tetap**: Saat jumlah pengulangan bergantung pada kondisi yang dinamis.

---

### **3. Perulangan `do...while` dalam Python**
Python tidak memiliki struktur perulangan `do...while` seperti bahasa pemrograman lainnya (misalnya C, Java). Namun, kita bisa mensimulasikan perilaku `do...while` dengan menggunakan perulangan `while` dan memeriksa kondisi setelah blok kode dijalankan setidaknya satu kali.

#### **Simulasi Perulangan `do...while`**
Dalam perulangan `do...while`, blok kode selalu dijalankan sekali sebelum memeriksa kondisi. Kita bisa menggunakan perulangan `while` untuk meniru perilaku ini.

#### **Sintaks Simulasi `do...while`**
```python
while True:
    # blok kode yang dijalankan
    if not kondisi:
        break
```

#### **Contoh Program Simulasi `do...while`**
```python
# Program menghitung angka 1 sampai 5 menggunakan simulasi do...while
i = 1
while True:
    print(i)
    i += 1
    if i > 5:
        break
```
**Penjelasan:**
- Perulangan selalu dimulai terlebih dahulu, lalu kondisi diperiksa setelah eksekusi blok kode.
- Jika kondisi `i > 5` terpenuhi, perulangan dihentikan dengan menggunakan `break`.

#### **Kasus Umum Penggunaan Simulasi `do...while`**
- **Memastikan suatu aksi terjadi minimal sekali**: Misalnya, membaca input pengguna sampai mereka memberikan input yang benar.
  
---

### **4. Perbedaan antara `while` dan `do...while`**
- **`while`**: Mengevaluasi kondisi terlebih dahulu sebelum menjalankan blok kode. Jika kondisi `False` di awal, blok kode tidak dijalankan sama sekali.
- **`do...while`**: Menjalankan blok kode terlebih dahulu, baru kemudian mengevaluasi kondisi untuk iterasi berikutnya. Di Python, ini disimulasikan dengan `while True` dan perintah `break`.

---

### **5. Studi Kasus**
#### **a. Menghitung Jumlah Angka Positif**
Menggunakan perulangan `while` untuk menghitung jumlah angka positif yang dimasukkan oleh pengguna.

```python
jumlah = 0
while True:
    angka = int(input("Masukkan angka positif (0 untuk berhenti): "))
    if angka == 0:
        break
    if angka > 0:
        jumlah += angka
print("Jumlah total angka positif:", jumlah)
```
**Penjelasan:**
- Program terus meminta input dari pengguna hingga mereka memasukkan angka 0.
- Setiap angka positif yang dimasukkan akan dijumlahkan.

#### **b. Simulasi Menu Pilihan Pengguna**
Menggunakan simulasi perulangan `do...while` untuk memastikan menu selalu muncul setidaknya sekali.

```python
while True:
    print("Menu:")
    print("1. Pilihan 1")
    print("2. Pilihan 2")
    print("3. Keluar")
    pilihan = int(input("Pilih menu (1/2/3): "))
    if pilihan == 3:
        print("Keluar dari program.")
        break
    elif pilihan == 1:
        print("Pilihan 1 dipilih")
    elif pilihan == 2:
        print("Pilihan 2 dipilih")
    else:
        print("Pilihan tidak valid")
```
**Penjelasan:**
- Menu akan selalu tampil setidaknya sekali dan memeriksa pilihan pengguna.
- Program akan berhenti jika pengguna memilih `3` untuk keluar.

---

### **6. Kesimpulan**
- **`while`** digunakan untuk perulangan yang bergantung pada kondisi yang diuji sebelum setiap iterasi.
- **Simulasi `do...while`** di Python dapat dilakukan dengan `while True` dan `break` untuk memastikan blok kode dijalankan minimal sekali.
- Kedua struktur ini penting untuk digunakan dalam pemrograman ketika kita ingin mengontrol alur program berdasarkan kondisi yang dinamis.

---

### **Latihan**
1. Buat program yang meminta pengguna untuk memasukkan angka hingga mereka memasukkan angka negatif. Program harus menghitung jumlah angka positif yang dimasukkan.
2. Modifikasi program simulasi menu pilihan agar dapat menampilkan menu baru setelah pilihan dieksekusi, dan dapat menangani input yang salah dengan memberikan pesan error.

---

---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)