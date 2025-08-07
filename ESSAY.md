# 📊 Struktur Data – Studi Kasus & Analisis

## 📌 1. Apa Itu Struktur Data?

Struktur data adalah cara menyimpan dan mengorganisir data agar dapat digunakan secara efisien. Struktur data sangat penting dalam pemrograman karena menentukan bagaimana data diakses dan dimodifikasi.

---

## 🎯 2. Kegunaan Struktur Data

- ✅ **Mengelola Data Secara Efisien**  
  Menyimpan dan mengambil data dengan cepat dan hemat memori.

- ✅ **Meningkatkan Performa Aplikasi**  
  Algoritma bekerja lebih efisien ketika menggunakan struktur data yang tepat.

- ✅ **Menyelesaikan Masalah Kompleks**  
  Misalnya pencarian data, pengurutan, dan navigasi antar objek (seperti graf atau tree).

---

## 🧩 3. Jenis-Jenis Struktur Data

| Jenis        | Penjelasan |
|--------------|------------|
| **Array**     | Kumpulan data bertipe sama yang disimpan secara berurutan. |
| **Stack**     | LIFO (Last In First Out), elemen terakhir yang masuk akan keluar pertama. |
| **Queue**     | FIFO (First In First Out), elemen pertama yang masuk akan keluar pertama. |
| **Linked List** | Elemen saling terhubung menggunakan pointer/referensi. |
| **Tree**      | Struktur hierarki seperti pohon, terdiri dari root dan cabang. |
| **Graph**     | Kumpulan node yang saling terhubung, cocok untuk merepresentasikan jaringan. |
| **Hash Table**| Menyimpan data menggunakan pasangan key-value dengan hashing. |

---

## 📚 4. Apa Itu Array dan Kegunaannya?

**Array** adalah struktur data yang menyimpan elemen bertipe sama dalam satu variabel menggunakan indeks.  
🔧 **Kegunaan**:
- Menyimpan banyak data secara berurutan.
- Mengakses data menggunakan indeks secara langsung dan cepat.

---

## 🧪 5. Contoh Array

### PHP:
``php
$buah = ["apel", "jeruk", "mangga"];
echo $buah[1]; // Output: jeruk
let angka = [10, 20, 30];
console.log(angka[2]); // Output: 30


6. Contoh Penerapan Struktur Data
✅ PHP (Array dan Stack):
php
Salin
Edit
<?php
$menu = ["Nasi Goreng", "Sate", "Mie Ayam"];
foreach ($menu as $m) {
    echo $m . "\n";
}

$stack = [];
array_push($stack, "Satu");
array_push($stack, "Dua");
echo array_pop($stack); // Output: Dua
?>
✅ Python (Queue dan Tree):
python
Salin
Edit
from collections import deque

# Queue
queue = deque(["A", "B", "C"])
print(queue.popleft())  # Output: A

# Tree
class Node:
    def __init__(self, data):
        self.data = data
        self.children = []

root = Node("Root")
root.children.append(Node("Left"))
root.children.append(Node("Right"))

for child in root.children:
    print(child.data)
