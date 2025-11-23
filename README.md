# CRUD-kampus-simple
📘 ABS Kampus Simple – REST API Flask

Proyek ABS Kampus Simple adalah aplikasi REST API berbasis Flask yang digunakan untuk mengelola data Mahasiswa, Kelas, dan Mata Kuliah dalam sistem akademik sederhana.
Struktur API dibuat modular menggunakan folder handler untuk setiap entitas, sehingga mudah dikembangkan dan dipelihara.

🚀 Fitur Utama
✅ Mahasiswa

Get all mahasiswa

Get single mahasiswa

Insert mahasiswa

Update mahasiswa

Delete mahasiswa

✅ Kelas

Get all kelas

Insert kelas

Update kelas

Delete kelas

✅ Mata Kuliah

Get all mata kuliah

Insert mata kuliah

Update mata kuliah

Delete mata kuliah

📂 Struktur Folder
ABS_kampus_simple/
│── main.py
│── mahasiswa/
│   └── handler.py
│── kelas/
│   └── handler.py
│── matakuliah/
│   └── handler.py
│── .venv/ (virtual environment)

🛠️ Teknologi yang Digunakan

Python 3.11

Flask

Virtual Environment (.venv)

Modul custom handler (Mahasiswa, Kelas, Mata Kuliah)

📦 Cara Instalasi & Menjalankan Aplikasi
1. Aktifkan Virtual Environment

Jika menggunakan Windows PowerShell:

.venv\Scripts\activate

2. Install Dependencies

Jika ada file requirements.txt, jalankan:

pip install -r requirements.txt


Kalau belum ada, minimal install Flask:

pip install flask

3. Jalankan Aplikasi

Pastikan kamu sedang berada di folder project:

python main.py


API akan berjalan di:

http://127.0.0.1:5000

🌐 Daftar Endpoint
📍 Mahasiswa
Method	Endpoint	Deskripsi
GET	/mahasiswa/get-all	Ambil semua data mahasiswa
GET	/mahasiswa/get-single	Ambil satu mahasiswa
POST	/mahasiswa/post	Tambah mahasiswa
POST	/mahasiswa/update	Update mahasiswa
POST	/mahasiswa/delete	Hapus mahasiswa
📍 Kelas
Method	Endpoint
GET	/kelas/get-all
POST	/kelas/post
POST	/kelas/update
POST	/kelas/delete
📍 Mata Kuliah
Method	Endpoint
GET	/matakuliah/get-all
POST	/matakuliah/post
POST	/matakuliah/update
POST	/matakuliah/delete
📝 Catatan

Semua endpoint POST menerima data melalui JSON.

Project berjalan menggunakan Flask built-in server (development mode).

Folder .venv sebaiknya tidak diupload ke GitHub (gunakan .gitignore).
