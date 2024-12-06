Berikut adalah materi perkuliahan untuk topik **Algoritma Pemrograman** dengan pembahasan **Deklarasi Fungsi**, **Parameter Fungsi**, **Deklarasi Sintaks**, dan **Pemanggilan Fungsi**. Materi ini dapat digunakan sebagai bahan ajar untuk mahasiswa yang mempelajari dasar-dasar algoritma pemrograman.

---

## Materi Perkuliahan: Algoritma Pemrograman

### 1. **Deklarasi Fungsi**
Fungsi adalah blok kode yang dirancang untuk melaksanakan tugas tertentu, dan dapat dipanggil berulang kali dari berbagai bagian dalam program. Fungsi memungkinkan kita untuk mengorganisasi dan menyusun program menjadi bagian-bagian kecil yang dapat dikelola.

#### Struktur Deklarasi Fungsi
Deklarasi fungsi terdiri dari:
- **Tipe Kembalian**: Tipe data yang dikembalikan oleh fungsi setelah eksekusi selesai. Jika fungsi tidak mengembalikan nilai, kita menggunakan tipe `void` (untuk bahasa C/C++) atau `None` (untuk Python).
- **Nama Fungsi**: Nama yang digunakan untuk memanggil fungsi.
- **Parameter Fungsi**: (Opsional) Daftar variabel yang diteruskan ke dalam fungsi ketika dipanggil.
- **Body Fungsi**: Bagian di dalam fungsi yang berisi kode yang akan dijalankan saat fungsi dipanggil.

#### Contoh Deklarasi Fungsi

**Bahasa C:**

```c
#include <stdio.h>

// Deklarasi fungsi
int tambah(int a, int b) {
    return a + b; // Mengembalikan hasil penjumlahan
}

int main() {
    int hasil = tambah(3, 4); // Memanggil fungsi
    printf("Hasil: %d\n", hasil);
    return 0;
}
```

**Bahasa Python:**

```python
# Deklarasi fungsi
def tambah(a, b):
    return a + b  # Mengembalikan hasil penjumlahan

hasil = tambah(3, 4)  # Memanggil fungsi
print("Hasil:", hasil)
```

### 2. **Parameter Fungsi**
Parameter adalah variabel yang diterima oleh fungsi saat fungsi dipanggil. Parameter memungkinkan kita untuk mengirimkan data ke dalam fungsi agar dapat diproses.

#### Jenis Parameter:
- **Parameter Posisional**: Parameter yang diberikan urutan tertentu saat fungsi dipanggil.
- **Parameter Default**: Parameter yang memiliki nilai default jika tidak diberikan nilai saat pemanggilan fungsi.
- **Parameter Variabel**: Parameter yang dapat menampung sejumlah argumen, misalnya menggunakan tanda `*args` di Python.

#### Contoh Penggunaan Parameter

**Bahasa C:**

```c
#include <stdio.h>

// Fungsi dengan parameter
void cetakSalam(char nama[]) {
    printf("Hallo, %s!\n", nama);  // Menampilkan pesan
}

int main() {
    cetakSalam("Andi");  // Memanggil fungsi dengan parameter
    return 0;
}
```

**Bahasa Python:**

```python
# Fungsi dengan parameter
def cetak_salam(nama):
    print(f"Hallo, {nama}!")  # Menampilkan pesan

cetak_salam("Andi")  # Memanggil fungsi dengan parameter
```

### 3. **Deklarasi Sintaks**
Sintaks adalah aturan atau struktur penulisan kode dalam bahasa pemrograman tertentu. Fungsi harus dideklarasikan sesuai dengan sintaks yang benar agar dapat dipanggil dan dijalankan dengan sukses.

#### Sintaks Umum Deklarasi Fungsi:
- **Bahasa C/C++**: Tipe Kembalian + Nama Fungsi + Parameter
  ```c
  <tipe_kembalian> <nama_fungsi>(<parameter>) { ... }
  ```
- **Bahasa Python**: `def` + Nama Fungsi + Parameter
  ```python
  def <nama_fungsi>(<parameter>):
      # kode
  ```

Contoh Sintaks:

**Bahasa C:**

```c
int tambah(int a, int b);  // Deklarasi fungsi
```

**Bahasa Python:**

```python
def tambah(a, b):  # Deklarasi fungsi
    return a + b
```

### 4. **Pemanggilan Fungsi**
Pemanggilan fungsi adalah langkah untuk menjalankan fungsi yang telah dideklarasikan. Fungsi dapat dipanggil dengan cara menyebutkan nama fungsi dan memberikan argumen yang sesuai dengan parameter yang diterima.

#### Cara Memanggil Fungsi
- Pada pemrograman prosedural, fungsi dapat dipanggil di mana saja dalam kode setelah deklarasi fungsi.
- Pada pemrograman berorientasi objek, fungsi sering dipanggil dengan menggunakan objek atau instansiasi kelas.

#### Contoh Pemanggilan Fungsi

**Bahasa C:**

```c
#include <stdio.h>

// Fungsi untuk menambah dua angka
int tambah(int a, int b) {
    return a + b;
}

int main() {
    int hasil = tambah(5, 7);  // Pemanggilan fungsi
    printf("Hasil penjumlahan: %d\n", hasil);
    return 0;
}
```

**Bahasa Python:**

```python
# Fungsi untuk menambah dua angka
def tambah(a, b):
    return a + b

hasil = tambah(5, 7)  # Pemanggilan fungsi
print("Hasil penjumlahan:", hasil)
```

### Penjelasan Pemanggilan Fungsi:
1. **Fungsi dengan Argumen Posisional**: Argumen yang dikirimkan ke fungsi sesuai dengan urutan parameter yang ada.
   - **C**: `tambah(5, 7)`
   - **Python**: `tambah(5, 7)`

2. **Fungsi dengan Nilai Kembalian**: Fungsi yang mengembalikan nilai setelah dieksekusi, yang dapat disimpan dalam variabel.
   - **C**: `int hasil = tambah(5, 7);`
   - **Python**: `hasil = tambah(5, 7)`

### Latihan
1. **Latihan 1**: Buat fungsi yang menerima dua bilangan bulat dan mengembalikan hasil perkalian kedua bilangan tersebut. Kemudian panggil fungsi tersebut dalam `main`.
2. **Latihan 2**: Buat fungsi yang menerima dua bilangan bulat dan mengembalikan nilai terbesar dari kedua bilangan tersebut.

---

Materi ini memberikan gambaran dasar tentang deklarasi fungsi, parameter fungsi, dan cara memanggil fungsi dalam program. Fungsi adalah bagian penting dalam membuat program yang lebih modular dan efisien.

---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)