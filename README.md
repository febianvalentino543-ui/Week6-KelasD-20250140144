<img width="3000" height="1702" alt="image" src="https://github.com/user-attachments/assets/6ccf9d20-c562-4ba1-a69d-a4f74a587b33" />

# Praktikum JavaScript: DOM, Event Handling, Fetch API, dan Validasi Input
 
Repositori ini berisi hasil praktikum **Pemrograman Web** yang membahas dasar-dasar JavaScript untuk membangun website yang dinamis dan interaktif.
 
| Keterangan | Detail |
| --- | --- |
| **Mata Kuliah** | Praktikum Pemrograman Web |
| **Kelas** | D |
| **Topik** | JavaScript DOM, Event Handling, Fetch API, dan Validasi Input |
 
---
 
## 📚 Materi Praktikum
 
### 1. DOM Selector dan Manipulasi
 
Mempelajari cara memilih dan memanipulasi elemen HTML menggunakan JavaScript melalui **Document Object Model (DOM)**.
 
**Materi yang dipelajari:**
 
- Memilih elemen HTML menggunakan `getElementById()`, `querySelector()`, dan `querySelectorAll()`.
- Mengubah konten elemen menggunakan `textContent` dan `innerHTML`.
- Mengubah atribut dan style elemen HTML.
- Menambahkan, menghapus, dan memodifikasi elemen secara dinamis.
- Memahami hubungan antara HTML, CSS, dan JavaScript.
---
 
### 2. Event Handling
 
Mempelajari cara menangani interaksi pengguna pada halaman web menggunakan JavaScript.
 
**Materi yang dipelajari:**
 
- Menggunakan `addEventListener()` untuk menangani event.
- Menangani event seperti `click`, `input`, `change`, dan `submit`.
- Mengambil nilai input dari pengguna.
- Menggunakan `preventDefault()` untuk mencegah perilaku default form.
- Memperbarui tampilan halaman berdasarkan interaksi pengguna.
---
 
### 3. Fetch API
 
Mempelajari cara mengambil data dari API eksternal menggunakan **Fetch API** dengan sumber data dari **DummyJSON**.
 
**API yang digunakan:** [https://dummyjson.com/products](https://dummyjson.com/products)
 
**Materi yang dipelajari:**
 
- Mengirim permintaan HTTP menggunakan `fetch()`.
- Mengolah respons API menjadi format JSON menggunakan `response.json()`.
- Menampilkan data produk secara dinamis pada halaman web.
- Menggunakan `Promise` dan `async/await`.
- Menangani kesalahan ketika permintaan API gagal.
**Contoh implementasi:**
 
```javascript
async function getProducts() {
  try {
    const response = await fetch(
      "https://dummyjson.com/products"
    );
 
    if (!response.ok) {
      throw new Error("Gagal mengambil data produk");
    }
 
    const data = await response.json();
    console.log(data.products);
  } catch (error) {
    console.error("Terjadi kesalahan:", error);
  }
}
 
getProducts();
```
 
---

<img width="2996" height="1698" alt="image" src="https://github.com/user-attachments/assets/a7e2fe4e-7279-4e62-9e51-260e56912a64" />

<img width="3000" height="1706" alt="Screenshot 2026-10-25 141542" src="https://github.com/user-attachments/assets/59b95a75-4f70-46b9-a237-b374268c0477" />

### 4. Validasi Input
 
Mempelajari cara melakukan validasi data yang dimasukkan pengguna sebelum diproses oleh aplikasi.
 
Pada praktikum ini, validasi diterapkan pada form **Caption Produk** yang memiliki input nama produk, harga, pilihan template caption, tombol untuk membuat caption, dan area hasil caption.
 
**Validasi yang diterapkan:**
 
- Nama produk wajib diisi.
- Nama produk minimal terdiri dari 5 karakter.
- Harga produk wajib diisi dan harus berupa angka.
- Harga produk minimal Rp1.000.
- Template caption dipilih sesuai kebutuhan.
- Caption dibuat berdasarkan data produk, harga, dan template yang dipilih.
- Hasil caption ditampilkan pada halaman setelah input memenuhi ketentuan.
**Tujuan validasi:**
 
- Mencegah data kosong atau tidak sesuai ketentuan.
- Memberikan pesan kesalahan yang informatif kepada pengguna.
- Meningkatkan kualitas data yang diproses.
- Membuat form lebih interaktif dan mudah digunakan.
---
 
## 🛠️ Teknologi yang Digunakan
 
| Teknologi | Kegunaan |
| --- | --- |
| **HTML5** | Membangun struktur halaman web. |
| **CSS3** | Mengatur tampilan dan desain halaman. |
| **JavaScript** | Mengelola DOM, event, pengambilan data API, dan validasi form. |
| **Fetch API** | Mengambil data produk dari layanan eksternal. |
| **DummyJSON** | Menyediakan data produk untuk latihan penggunaan API. |
 
---
 
## 📝 Kesimpulan
 
Melalui praktikum ini, saya mempelajari dasar-dasar JavaScript untuk membangun website yang lebih dinamis dan interaktif. Materi **DOM Selector dan Manipulasi** membantu saya mengelola elemen halaman, **Event Handling** memungkinkan halaman merespons tindakan pengguna, **Fetch API** digunakan untuk mengambil data produk dari DummyJSON, sedangkan **Validasi Input** membantu memastikan data yang dimasukkan sesuai dengan ketentuan sebelum diproses.
 
Praktikum ini menjadi dasar untuk memahami pengembangan aplikasi web yang lebih kompleks dengan JavaScript.
