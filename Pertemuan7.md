Berikut adalah materi perkuliahan mengenai **Pengenalan Teknik Percabangan** dalam Algoritma Pemrograman yang mencakup beberapa topik terkait seperti penggunaan percabangan `if`, `if else`, `nested if`, dan `switch`.

---

### **1. Pengenalan Teknik Percabangan**

**Definisi Percabangan:**
Percabangan adalah salah satu teknik dasar dalam pemrograman yang memungkinkan eksekusi program untuk memilih salah satu dari beberapa jalur berdasarkan kondisi tertentu. Dengan percabangan, program dapat mengarahkan alur eksekusi ke bagian lain, sesuai dengan hasil evaluasi kondisi yang diberikan.

**Tujuan Percabangan:**
- Menangani kondisi yang berbeda dalam program.
- Memberikan kontrol atas eksekusi kode program berdasarkan nilai atau kondisi yang berbeda.

### **2. Penggunaan Percabangan `if`**

Percabangan `if` adalah pernyataan yang digunakan untuk memeriksa suatu kondisi. Jika kondisi tersebut benar (true), maka blok kode yang terkait akan dieksekusi.

**Sintaks `if`:**
```python
if kondisi:
    # blok kode yang dijalankan jika kondisi benar
```

**Contoh:**
```python
x = 10
if x > 5:
    print("x lebih besar dari 5")
```

**Penjelasan:**
- Jika `x` lebih besar dari 5, maka program akan mencetak "x lebih besar dari 5".

### **3. Penggunaan Percabangan `if else`**

Percabangan `if else` digunakan untuk memilih salah satu dari dua jalur eksekusi. Jika kondisi pertama benar (true), maka blok kode setelah `if` yang dijalankan. Jika kondisi tersebut salah (false), maka blok kode setelah `else` yang dijalankan.

**Sintaks `if else`:**
```python
if kondisi:
    # blok kode yang dijalankan jika kondisi benar
else:
    # blok kode yang dijalankan jika kondisi salah
```

**Contoh:**
```python
x = 3
if x > 5:
    print("x lebih besar dari 5")
else:
    print("x tidak lebih besar dari 5")
```

**Penjelasan:**
- Karena `x` tidak lebih besar dari 5, program akan mencetak "x tidak lebih besar dari 5".

### **4. Penggunaan Nested `if`**

**Nested `if`** adalah penggunaan pernyataan `if` di dalam pernyataan `if` lainnya. Hal ini memungkinkan untuk memeriksa kondisi lebih lanjut setelah kondisi pertama dipenuhi.

**Sintaks Nested `if`:**
```python
if kondisi1:
    if kondisi2:
        # blok kode yang dijalankan jika kondisi1 dan kondisi2 benar
```

**Contoh:**
```python
x = 10
y = 20
if x > 5:
    if y > 15:
        print("x lebih besar dari 5 dan y lebih besar dari 15")
```

**Penjelasan:**
- Program pertama-tama memeriksa apakah `x` lebih besar dari 5. Jika benar, program akan melanjutkan untuk memeriksa apakah `y` lebih besar dari 15.

### **5. Penggunaan `switch`**

Pada bahasa pemrograman tertentu (seperti C, Java, atau JavaScript), **`switch`** adalah alternatif untuk menggunakan beberapa pernyataan `if else` yang dapat membuat kode lebih jelas dan mudah dibaca. `switch` digunakan untuk membandingkan nilai variabel dengan beberapa pilihan yang ada, dan menjalankan blok kode yang sesuai dengan nilai tersebut.

**Sintaks `switch`:**
```c
switch (ekspresi) {
    case nilai1:
        // blok kode jika ekspresi sama dengan nilai1
        break;
    case nilai2:
        // blok kode jika ekspresi sama dengan nilai2
        break;
    default:
        // blok kode jika ekspresi tidak cocok dengan nilai yang ada
}
```

**Contoh:**
```c
int hari = 3;
switch (hari) {
    case 1:
        printf("Senin");
        break;
    case 2:
        printf("Selasa");
        break;
    case 3:
        printf("Rabu");
        break;
    default:
        printf("Hari tidak valid");
}
```

**Penjelasan:**
- Program akan mencetak "Rabu" karena nilai `hari` adalah 3.

### **Kesimpulan dan Perbandingan Percabangan:**

| Jenis Percabangan    | Deskripsi                                           | Kapan Digunakan                              |
|----------------------|-----------------------------------------------------|----------------------------------------------|
| `if`                 | Mengeksekusi blok kode jika kondisi benar           | Ketika hanya ada satu kondisi yang perlu dicek. |
| `if else`            | Mengeksekusi dua blok kode, tergantung kondisi      | Ketika ada dua jalur yang bisa dipilih berdasarkan kondisi. |
| Nested `if`          | Menggunakan `if` di dalam `if` untuk kondisi bertingkat | Ketika ada kondisi yang lebih spesifik atau bertingkat. |
| `switch`             | Membandingkan nilai satu variabel dengan beberapa pilihan | Untuk memilih antara banyak pilihan berdasarkan satu nilai variabel. |

---

### **Latihan Soal:**
1. Buat program yang meminta input angka dari pengguna dan mengecek apakah angka tersebut positif, negatif, atau nol.
2. Buat program dengan menggunakan `switch` untuk mencetak nama bulan berdasarkan nomor bulan (1-12).

--- 

Materi di atas memberikan pemahaman dasar tentang percabangan dalam pemrograman. Pastikan untuk mempraktekkan setiap teknik dengan membuat kode dan menjalankannya agar lebih menguasai konsep ini.


---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)