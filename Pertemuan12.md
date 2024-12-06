Berikut adalah materi perkuliahan Algoritma Pemrograman yang membahas penggunaan perulangan `while` dan `do...while`:

---

### **Materi Perkuliahan: Algoritma Pemrograman**
### **Topik: Penggunaan Perulangan `while` dan `do...while`**

#### **1. Pengertian Perulangan (Looping)**

Perulangan atau looping dalam pemrograman adalah suatu cara untuk menjalankan sebuah blok kode berulang kali berdasarkan kondisi tertentu. Perulangan berguna untuk menghindari pengulangan kode secara manual dan memungkinkan program melakukan tugas yang sama secara efisien.

Terdapat beberapa jenis perulangan dalam pemrograman, di antaranya adalah:
- **Perulangan `for`** 
- **Perulangan `while`**
- **Perulangan `do...while`**

Pada materi kali ini, kita akan fokus pada perulangan `while` dan `do...while`.

---

### **2. Perulangan `while`**

Perulangan `while` digunakan untuk menjalankan suatu blok kode selama kondisi tertentu bernilai benar (true). Struktur dasar perulangan `while` adalah:

```cpp
while (kondisi) {
    // blok kode yang akan diulang
}
```

**Penjelasan:**
- **Kondisi:** merupakan ekspresi yang dievaluasi sebelum setiap iterasi.
- **Blok kode:** kode yang akan dieksekusi selama kondisi bernilai benar.

**Proses eksekusi perulangan `while`:**
1. Mengevaluasi kondisi.
2. Jika kondisi bernilai **true**, blok kode dieksekusi.
3. Setelah eksekusi, kembali ke langkah pertama, mengevaluasi kondisi.
4. Jika kondisi bernilai **false**, perulangan berhenti.

**Contoh Penggunaan `while`:**

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    while (i <= 5) {
        cout << "Perulangan ke-" << i << endl;
        i++; // Increment i agar tidak terjadi perulangan tanpa henti
    }
    return 0;
}
```

**Penjelasan:**
- Perulangan dimulai dengan `i = 1` dan selama `i <= 5`, program akan mencetak "Perulangan ke-x".
- Setelah mencetak, nilai `i` akan ditambah 1 (increment).
- Ketika `i` menjadi 6, kondisi `i <= 5` menjadi false dan perulangan berhenti.

---

### **3. Perulangan `do...while`**

Perulangan `do...while` mirip dengan `while`, namun perbedaannya adalah bahwa perulangan ini selalu menjalankan blok kode setidaknya sekali, meskipun kondisi awal bernilai false. Ini karena kondisi baru dievaluasi setelah eksekusi blok kode.

Struktur dasar perulangan `do...while` adalah:

```cpp
do {
    // blok kode yang akan diulang
} while (kondisi);
```

**Penjelasan:**
- **Blok kode**: kode yang akan dieksekusi terlebih dahulu.
- **Kondisi**: kondisi yang diperiksa setelah blok kode dieksekusi.
- **Perulangan berhenti** jika kondisi bernilai false.

**Proses eksekusi perulangan `do...while`:**
1. Menjalankan blok kode setidaknya satu kali.
2. Mengevaluasi kondisi setelah eksekusi blok kode.
3. Jika kondisi bernilai true, kembali ke langkah pertama.
4. Jika kondisi bernilai false, perulangan berhenti.

**Contoh Penggunaan `do...while`:**

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    do {
        cout << "Perulangan ke-" << i << endl;
        i++; // Increment i
    } while (i <= 5);
    return 0;
}
```

**Penjelasan:**
- Blok kode di dalam `do` akan dieksekusi terlebih dahulu.
- Setelah itu, kondisi `i <= 5` akan dievaluasi.
- Perulangan akan terus terjadi selama kondisi bernilai true, dan berhenti jika kondisi menjadi false.

---

### **4. Perbandingan `while` dan `do...while`**

| **Fitur**            | **Perulangan `while`**                          | **Perulangan `do...while`**                    |
|----------------------|-------------------------------------------------|------------------------------------------------|
| **Eksekusi pertama** | Kondisi diperiksa sebelum eksekusi pertama.     | Blok kode dieksekusi terlebih dahulu, baru kondisi diperiksa. |
| **Keuntungan**       | Berguna jika kita tidak tahu berapa kali perulangan diperlukan, dan perulangan hanya dilakukan jika kondisi awal benar. | Berguna jika kita perlu menjalankan blok kode setidaknya sekali, bahkan jika kondisi awal salah. |
| **Kondisi**          | Perulangan berhenti jika kondisi awal tidak terpenuhi. | Perulangan akan selalu dilakukan sekali, bahkan jika kondisi awal salah. |

---

### **5. Kasus Penggunaan `while` dan `do...while`**

- **Perulangan `while`** cocok digunakan jika kita ingin perulangan hanya dilakukan ketika kondisi awal sudah benar.
  
  **Contoh:**
  - Menunggu input dari pengguna sampai pengguna memberikan input yang valid.
  
- **Perulangan `do...while`** cocok digunakan ketika kita ingin memastikan bahwa suatu aksi dilakukan setidaknya sekali, misalnya:
  
  **Contoh:**
  - Menampilkan menu dan meminta pilihan pengguna setidaknya satu kali, meskipun pada awalnya pilihan bisa salah.

---

### **6. Kesalahan Umum dalam Penggunaan Perulangan**

- **Infinite Loop (Perulangan Tak Terbatas):** 
  Kesalahan yang sering terjadi adalah tidak memperbarui kondisi di dalam perulangan, sehingga kondisi selalu bernilai true dan perulangan berjalan terus menerus.
  
  **Contoh Kesalahan:**
  ```cpp
  int i = 1;
  while (i <= 5) {
      cout << "Perulangan ke-" << i << endl;
      // Lupa untuk menambah nilai i
  }
  ```

---

### **7. Latihan**

**Latihan 1:**  
Buat program yang meminta pengguna memasukkan angka positif. Program harus terus meminta input sampai pengguna memasukkan angka negatif menggunakan perulangan `while`.

**Latihan 2:**  
Buat program yang mencetak angka dari 1 hingga 10 menggunakan perulangan `do...while`.

**Latihan 3:**  
Buat program yang menampilkan menu pilihan (1. Lihat Data, 2. Input Data, 3. Keluar). Program harus terus menampilkan menu sampai pengguna memilih "Keluar" (pilihan 3), menggunakan perulangan `do...while`.

---

**Penutupan**

Perulangan adalah alat yang sangat penting dalam pemrograman untuk melakukan tugas berulang secara efisien. Dengan memahami penggunaan perulangan `while` dan `do...while`, Anda dapat membuat program yang lebih fleksibel dan dinamis.

---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)