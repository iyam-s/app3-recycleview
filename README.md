# Pengenalan recycler view 
Tugas pengenalan recyclerview

# Apa itu recycler view ?
RecyclerView adalah komponen dalam Android yang dirancang untuk menampilkan kumpulan data dalam jumlah besar secara lebih efisien dan responsif. 

RecyclerView juga fleksibel karena memungkinkan developer untuk:
Menentukan tata letak item (dengan LayoutManager seperti Linear, Grid, atau Staggered),
Menambahkan animasi transisi antar item,
Menyisipkan fitur interaktif seperti klik atau swipe pada item.
Secara keseluruhan, RecyclerView meningkatkan performa, daya tanggap (responsiveness), dan efisiensi konsumsi daya aplikasi, terutama saat berhadapan dengan data dalam jumlah besar yang ditampilkan secara dinamis.

## 👥 Tim
-Madina al aliyy f.s (23)
-Mayang Aura Chandra (24)
-M. Nauval Irkhamsyah (27)

## 📱 Fitur
Create – Menambahkan data baru
Read – Membaca atau menampilkan data
Update – Mengubah data yang sudah ada
Delete – Menghapus data

## 🔧 Teknologi
- Kotlin
- Android Studio
- Git + GitHub

## 📸 Penjelasan code dan screenshot
![1](https://github.com/user-attachments/assets/37e4b043-0c18-4840-b0dd-f02b64790049)
![2](https://github.com/user-attachments/assets/109c813f-12dc-4259-bdba-2ffd67ecbbb1)
![3](https://github.com/user-attachments/assets/b6522759-5fe3-48de-9424-ccda576b555b)
![4](https://github.com/user-attachments/assets/a0c6a405-26c2-465e-bd36-dbed74c917f2)

Kode ini adalah bagian dari adapter RecyclerView di Android, yang digunakan untuk menampilkan dan mengelola daftar data siswa. Fungsinya adalah untuk:
Menampilkan daftar siswa
1. Setiap siswa ditampilkan dalam bentuk kartu/item berisi:
Nama
NIS
Kelas
Tombol Edit dan Hapus

2. Mengedit data siswa
Saat tombol Edit ditekan:
Muncul dialog input berisi data siswa yang bisa diubah.
Setelah disimpan, data akan diperbarui di daftar.

3. Menghapus data siswa
Saat tombol Hapus ditekan:
Muncul dialog konfirmasi.
Jika disetujui, data siswa akan dihapus dari daftar.

4. Mencari siswa (Filter)
Pengguna bisa mencari siswa berdasarkan:
Nama
NIS
Kelas

Hasil pencarian akan langsung diperbarui di tampilan daftar

<img width="576" height="255" alt="Screenshot 2025-08-07 112907" src="https://github.com/user-attachments/assets/2e3ce638-1f4f-4b84-9c1f-57a004b68e25" />
data class: digunakan untuk menyimpan data. Kotlin secara otomatis membuatkan method seperti toString(), equals(), hashCode(), dan copy() untuk memudahkan pengelolaan data.
Student: adalah nama kelasnya.
val nama, nis, kelas: adalah properti dari objek Student, masing-masing menyimpan nama siswa, NIS (Nomor Induk Siswa), dan kelasnya.

<img width="1171" height="723" alt="Screenshot 2025-08-07 130045" src="https://github.com/user-attachments/assets/424a8d87-196d-41b3-a6df-ccba9e4917f7" />
<img width="1072" height="401" alt="Screenshot 2025-08-07 130051" src="https://github.com/user-attachments/assets/719b86b1-1f95-444c-9dce-454f3dc2f404" />
Kode ini digunakan untuk menampilkan data lengkap siswa saat pengguna memilih salah satu dari daftar siswa yang ada.

<img width="1060" height="720" alt="Screenshot 2025-08-07 130245" src="https://github.com/user-attachments/assets/c3f8213b-957d-4058-ac07-d8f65d0b81b8" />
<img width="1099" height="691" alt="Screenshot 2025-08-07 130300" src="https://github.com/user-attachments/assets/af72adec-1683-4598-835e-f212c688c24c" />
<img width="1044" height="313" alt="Screenshot 2025-08-07 130306" src="https://github.com/user-attachments/assets/cf82c43d-c160-4fd2-80be-0bb76d609811" />
Kode ini membentuk antarmuka utama aplikasi daftar siswa dengan fitur:
Tampilan dinamis melalui RecyclerView
Pencarian data siswa
Menambahkan siswa baru
Navigasi ke detail siswa (kalau di dalam StudentAdapter ada intent ke DetailActivity)

<img width="919" height="664" alt="Screenshot 2025-08-07 130717" src="https://github.com/user-attachments/assets/2a89e180-4b1e-4fd7-a4a3-852aee07b980" />
<img width="671" height="747" alt="Screenshot 2025-08-07 130728" src="https://github.com/user-attachments/assets/f1938ee9-394c-406c-a753-91023180cfb5" />
<img width="670" height="311" alt="Screenshot 2025-08-07 130734" src="https://github.com/user-attachments/assets/de752076-1252-4d17-bae6-efc8ac76a5c5" />
Fungsi Layout Ini:
Menampilkan:
Judul “Biodata Siswa”
Gambar ikon siswa (fotosiswa)
3 informasi penting:
Nama
NIS
Kelas
Data tersebut ditampilkan dalam bentuk TextView, dan nilainya diatur melalui kode Kotlin di DetailActivity.

Penjelasan fungsi beberapa komponen :

LinearLayout: Sebagai wadah utama yang menata elemen-elemen secara vertikal.
TextView (judul): Menampilkan teks "Biodata Siswa" sebagai judul utama di bagian atas.
ImageView: Menampilkan gambar siswa dari sumber drawable (@drawable/fotosiswa) di tengah tampilan.
TextView dengan id tvNama: Menampilkan nama siswa.
TextView dengan id tvNis: Menampilkan Nomor Induk Siswa (NIS).
TextView dengan id tvKelas: Menampilkan kelas dari siswa tersebut.

<img width="1081" height="621" alt="Screenshot 2025-08-07 131032" src="https://github.com/user-attachments/assets/38a35645-3e69-4419-b3fa-01ad66f103c3" />
<img width="1081" height="621" alt="Screenshot 2025-08-07 131032" src="https://github.com/user-attachments/assets/91d8ea07-54dc-4c42-a6b3-5b77885d341c" />
Fungsi Layout Ini:

Menampilkan tampilan utama yang terdiri dari:
Tombol “Tambah Siswa”
Search bar untuk mencari siswa berdasarkan nama/NIS/kelas.
RecyclerView untuk menampilkan daftar siswa secara vertikal.

beberapa  fungsi komponen dan fungsinya :

ConstraintLayout	Layout fleksibel untuk mengatur posisi elemen dengan constraint (kait antar elemen).
Button id=btnTambah	Saat diklik, akan memunculkan form dialog untuk menambahkan data siswa baru.
SearchView id=searchView	Untuk mengetik kata kunci dan mencari siswa secara realtime.
RecyclerView id=recyclerView	Tempat menampilkan daftar siswa secara scrollable. Setiap item ditampilkan lewat StudentAdapter.

<img width="888" height="674" alt="Screenshot 2025-08-07 131816" src="https://github.com/user-attachments/assets/337a6ae7-437f-486d-9d6e-0d6b5650073d" />
<img width="888" height="674" alt="Screenshot 2025-08-07 131816" src="https://github.com/user-attachments/assets/b9b54797-f865-4bf6-9d88-fb9ad7469917" />

LinearLayout: Berfungsi sebagai wadah utama dengan orientasi vertikal, sehingga komponen di dalamnya disusun dari atas ke bawah dan diberi padding 20dp.
EditText dengan id edtNama: Digunakan untuk memasukkan nama siswa. InputType disetel ke textPersonName agar sesuai untuk nama orang.
EditText dengan id edtNis: Digunakan untuk memasukkan Nomor Induk Siswa (NIS). InputType disetel ke number agar hanya bisa menerima angka.
EditText dengan id edtKelas: Digunakan untuk memasukkan kelas siswa. InputType disetel ke text untuk teks bebas.

<img width="1081" height="690" alt="Screenshot 2025-08-07 131942" src="https://github.com/user-attachments/assets/0171441a-1729-4cd6-9fb3-8de0d3a0251d" />
<img width="758" height="680" alt="Screenshot 2025-08-07 132006" src="https://github.com/user-attachments/assets/f42c3289-5cc7-4cde-b437-542e9b3819db" />
<img width="689" height="577" alt="Screenshot 2025-08-07 132017" src="https://github.com/user-attachments/assets/6e35bc8a-fa9c-4994-8ac6-e7d51c16fc59" />
<img width="725" height="765" alt="Screenshot 2025-08-07 132024" src="https://github.com/user-attachments/assets/55454cf1-6a84-477f-90bc-6cd46de670f6" />

CardView: Membungkus seluruh item agar tampil seperti kartu dengan sudut membulat (cardCornerRadius) dan bayangan (cardElevation), memberi tampilan elegan dan terpisah antar data siswa.
LinearLayout (utama): Menyusun semua komponen di dalam kartu secara vertikal dan memberikan padding agar isi tidak menempel langsung ke tepi kartu.
ImageView: Menampilkan ikon atau foto siswa dengan ukuran 48x48dp di sebelah kiri.
TextView tvNama: Menampilkan nama siswa dalam huruf tebal dan ukuran lebih besar (18sp).
TextView tvNis: Menampilkan Nomor Induk Siswa (NIS) dengan ukuran teks 14sp dan warna abu-abu gelap.
TextView tvKelas: Menampilkan kelas siswa dengan ukuran teks 14sp dan warna abu-abu lebih terang.
Button btnEdit: Tombol untuk mengedit data siswa.
Button btnHapus: Tombol untuk menghapus data siswa. Warna teks disesuaikan agar kontras dengan latar.


# Kesimpulan
dari semua kode diatas dapat diambil kesimpulan:
Di halaman utama, ada tombol tambah untuk memasukkan data siswa baru, kolom pencarian untuk mencari nama siswa secara cepat, dan daftar siswa yang ditampilkan lewat RecyclerView. Setiap data siswa ditampilkan dalam bentuk kartu yang memuat foto, nama, NIS, dan kelas, lengkap dengan tombol edit dan hapus di bagian bawahnya. Ketika salah satu siswa dipilih, akan muncul halaman detail yang menampilkan informasi lengkap siswa tersebut.
Semua tampilan dibuat dengan rapi dan responsif, agar pengalaman pengguna jadi lebih nyaman dan aplikasi bisa dipakai dengan lancar di berbagai ukuran layar. Dengan kata lain, ini adalah aplikasi pendataan siswa sederhana tapi fungsional, cocok untuk digunakan di lingkungan sekolah atau pendidikan.
