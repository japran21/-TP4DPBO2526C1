# -TP4DPBO2526C1

# JANJI
Saya Muhammad Ilal Zhafran dengan NIM 2502623 mengerjakan Tugas Praktikum 4 pada Mata Kuliah Desain dan Pemrograman Berorientasi Objek (DPBO) untuk keberkahan-Nya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin

# STRUKTUR
<img width="475" height="932" alt="image" src="https://github.com/user-attachments/assets/745846a5-b96d-4739-a33d-2f07ce1d9af4" />

# ALUR PROGRAM
### 1. Add (Tambah Data)
engguna mengisi `ID`, `Nama`, `Tahun Lahir`, memilih `Kategori` pada dropdown, dan memilih `Jenis Kelamin` menggunakan radio button.
Pengguna menekan tombol *Add*. Sistem melakukan validasi:
  * Kolom tidak boleh kosong.
  * Kategori harus dipilih secara valid.
  * Tahun lahir harus berupa angka yang valid (rentang tahun wajar).
* Data disimpan ke dalam `ArrayList<Person>`, tabel langsung ter-refresh, dan muncul pesan notifikasi *"Data berhasil ditambahkan!"*. Form otomatis dibersihkan (*clear*).
  ### 2. Read (Tampilkan & Pilih Data)
* Data ditampilkan dalam bentuk `JTable` melalui `DefaultTableModel`.
* Saat pengguna **mengklik salah satu baris tabel**:
  * Seluruh data pada baris tersebut otomatis mengisi kolom-kolom input form.
  * Tombol **Add** berubah menjadi **Update**.
  * Tombol **Delete** yang awalnya tersembunyi menjadi muncul/tampak.

### 3. Update (Ubah Data)
* Setelah memilih baris data dari tabel, pengguna dapat mengedit data pada form.
* Pengguna menekan tombol **Update**.
* Sistem memvalidasi input, memperbarui data pada list, me-refresh tabel, menampilkan dialog notifikasi *"Data berhasil diubah!"*, dan mereset form.

### 4. Delete dengan Confirmation Prompt (Hapus Data)
* Saat data dipilih dan tombol **Delete** ditekan, program **tidak langsung menghapus data**, melainkan memunculkan dialog konfirmasi:
  > *"Apakah Anda yakin ingin menghapus data ini?"* dengan tombol **Yes** dan **No**.
* **Jika Yes:** Data dihapus dari list dan tabel, muncul pesan konfirmasi *"Data berhasil dihapus!"*, dan form dibersihkan.
* **Jika No:** Penghapusan dibatalkan dan data tetap aman.

### 5. Cancel / Clear Form
* Tombol **Cancel** dapat ditekan kapan saja untuk mengosongkan input form, mengembalikan tombol ke mode **Add**, dan menyembunyikan tombol **Delete**.

# DOKUMENTASI
### JAVA
| Fitur CRUD | Keterangan | Gambar |
|---|---|---|
| **ADD** | Menambahkan data member gym baru lewat form | <img width="897" height="452" alt="Add3" src="https://github.com/user-attachments/assets/e7ade42a-0c3a-44e1-9fb1-1ee680450274" /><img width="892" height="782" alt="Add2" src="https://github.com/user-attachments/assets/daae88a9-11db-4200-96f9-bc7526dab6b1" /><img width="897" height="776" alt="Add" src="https://github.com/user-attachments/assets/2a8070a0-8ee5-471f-a2ae-631a733cb3ab" />|
| **Update** | Mengubah data berdasarkan baris yang diklik | <img width="900" height="547" alt="Update1" src="https://github.com/user-attachments/assets/e75fa886-8271-49ab-bf20-74950fd5729f" /><img width="905" height="487" alt="update2" src="https://github.com/user-attachments/assets/609b7df2-2513-4a5f-8b86-e3159465952b" />|
| **Delete** | Menghapus data dengan pop-up konfirmasi | <img width="902" height="775" alt="delete1" src="https://github.com/user-attachments/assets/96a2d02b-9de6-4827-99cd-c25227029927" /><img width="892" height="567" alt="delete2" src="https://github.com/user-attachments/assets/a11975ce-0052-43e4-aeb9-a397f252120c" /><img width="905" height="565" alt="delete3" src="https://github.com/user-attachments/assets/77fba0db-3e13-48d2-ba81-a23d6291efae" /><img width="901" height="491" alt="delete4" src="https://github.com/user-attachments/assets/77da4488-e6a2-4b2a-a630-ad950a7a66a4" />|
