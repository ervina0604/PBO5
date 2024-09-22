# 📚 Aplikasi CRUD dengan Java Swing dan JDBC - Pertemuan Kelima

Topik Utama: Aplikasi GUI dengan CRUD menggunakan Java Swing dan JDBC

---

## 📑 Daftar Isi
- [📝 Java Swing](https://github.com/ervina0604/PBO5/blob/main/VinaFrame.java)
- [🔗 Koneksi Database dengan JDBC](https://github.com/ervina0604/PBO5/blob/main/VinaFrame.java)
- [🛠 DbUtils: Utilitas Database](https://github.com/ervina0604/PBO5/blob/main/DbUtils.java)
- [🛠 Implementasi CRUD](https://github.com/ervina0604/PBO5/blob/main/VinaFrame.java)

---

## 📝 Java Swing
Java Swing adalah pustaka yang digunakan untuk membuat aplikasi desktop dengan antarmuka grafis yang interaktif.

### Komponen Utama:
- **JFrame** 🪟: Jendela utama aplikasi.
- **JPanel** 📦: Wadah untuk menempatkan komponen GUI lainnya.
- **JButton, JTextField, JTable**: Komponen untuk interaksi pengguna seperti tombol, input teks, dan tabel.

---

## 🔗 Koneksi Database dengan JDBC
JDBC (Java Database Connectivity) memungkinkan aplikasi Java berinteraksi dengan database. Menggunakan `DriverManager` untuk mendapatkan koneksi dan `Connection` untuk menjalankan perintah SQL.

---

## 🛠 DbUtils: Utilitas Database
Kelas `DbUtils` membantu mengonversi `ResultSet` dari database menjadi model tabel yang dapat ditampilkan di `JTable`.

### Metode `resultSetToTableModel`
- **Input**: `ResultSet rs`
- **Output**: `TableModel`

### Langkah-Langkah:
1. Ambil metadata kolom menggunakan `ResultSetMetaData`.
2. Simpan nama kolom dalam sebuah `Vector`.
3. Ambil data setiap baris dari `ResultSet` ke dalam `Vector`.
4. Kembalikan data dalam bentuk `DefaultTableModel`.

---

## 🛠 Implementasi CRUD
Berikut adalah penjelasan langkah-langkah CRUD yang diterapkan dalam aplikasi ini:

### 1. ➕ TAMBAH (Create)
Penambahan data dilakukan pada tabel **Dokter** di database `Pbo4`. Pengguna diminta untuk memasukkan informasi dokter, seperti **ID**, **nama**, **alamat**, dan **email**. Setelah data dimasukkan, pengguna dapat memilih untuk menambah dokter lain atau menyelesaikan proses. Semua data yang ditambahkan akan disimpan dengan aman menggunakan perintah `commit`.

### 2. 🔍 TAMPIL (Read)
Menu **Tampil Data** berfungsi untuk menampilkan semua informasi dokter yang tersimpan di tabel **Dokter**. Pengguna dapat memverifikasi bahwa data yang ditampilkan sesuai dengan input yang telah dimasukkan.

### 3. ❌ HAPUS (Delete)
Untuk menghapus data, pengguna diminta memasukkan **ID dokter** yang ingin dihapus. Setelah penghapusan, sistem akan mengonfirmasi keberhasilan proses. Jika **ID dokter** tidak ditemukan, sistem akan memberi tahu pengguna. Pengguna dapat memverifikasi penghapusan dengan kembali ke menu **Tampil Data**.

### 4. ✏️ UPDATE (Update)
Pengguna dapat memperbarui informasi dokter dengan memilih **ID dokter** yang akan diubah, lalu memasukkan informasi baru seperti **nama**, **alamat**, dan **email**. Setelah perubahan dilakukan, pengguna bisa melihat hasilnya melalui menu **Tampil Data** untuk memastikan pembaruan berhasil.

---

### 🚀 Selamat Belajar dan Menerapkan Java Swing serta JDBC dalam Pengembangan Aplikasi! 💻
