# Labpy08
# Praktikum 8
# Nama : Feby Putri Khurunnisa
# Kelas: TI 24 A2
# Nim  : 312410245 
Buat program sederhana dengan mengaplikasikan penggunaan class. Buatlah
class untuk menampilkan daftar nilai mahasiswa, dengan ketentuan:

• Method tambah() untuk menambah data

• Method tampilkan() untuk menampilkan data

• Method hapus(nama) untuk menghapus data berdasarkan nama

• Method ubah(nama) untuk mengubah data berdasarkan nama

![Screenshot (64)](https://github.com/user-attachments/assets/3604e9dd-824d-4fcd-a5a0-259a751d4075)
![Screenshot (63)](https://github.com/user-attachments/assets/5b7c1b12-859a-47be-bac4-2c8ca7edf288)
# Hasil Run

![Screenshot (66)](https://github.com/user-attachments/assets/5bcb1f0e-916d-4ad0-8d52-d91c81241809)
# Penjelasan
 1.  Import dan Definisi Class
        
class Mahasiswa:: Ini mendefinisikan sebuah class bernama Mahasiswa.
def __init__(self):: Ini adalah constructor dari class yang akan dipanggil saat kita membuat objek dari class ini.
self.daftar_mahasiswa = []: Di dalam constructor, kita mendeklarasikan atribut daftar_mahasiswa yang merupakan list kosong. List ini akan digunakan untuk menyimpan data mahasiswa dalam bentuk dictionary.

 2. Method tambah()

def tambah(self, nama, nilai):: Ini adalah method untuk menambahkan data mahasiswa baru. Method ini menerima dua parameter: nama dan nilai.
self.daftar_mahasiswa.append({'nama': nama, 'nilai': nilai}): Kita menambahkan dictionary baru ke dalam list daftar_mahasiswa, di mana dictionary tersebut berisi nama dan nilai mahasiswa.
print(...): Menampilkan pesan bahwa data mahasiswa berhasil ditambahkan.

 3. Method tampilkan()

def tampilkan(self):: Method ini digunakan untuk menampilkan semua data mahasiswa.
if not self.daftar_mahasiswa:: Memeriksa apakah daftar mahasiswa kosong. Jika kosong, akan menampilkan pesan dan keluar dari method.
for index, mahasiswa in enumerate(self.daftar_mahasiswa, start=1):: Menggunakan enumerate untuk mendapatkan indeks dan data mahasiswa. start=1 membuat indeks mulai dari 1.
print(...): Menampilkan nama dan nilai setiap mahasiswa dalam daftar.

 4. Method hapus()

def hapus(self, nama):: Method ini digunakan untuk menghapus data mahasiswa berdasarkan nama.
for mahasiswa in self.daftar_mahasiswa:: Melakukan iterasi pada setiap mahasiswa dalam daftar.
if mahasiswa['nama'] == nama:: Memeriksa apakah nama mahasiswa yang sedang diperiksa sama dengan nama yang ingin dihapus.
self.daftar_mahasiswa.remove(mahasiswa): Menghapus mahasiswa dari daftar jika ditemukan.
print(...): Menampilkan pesan bahwa data mahasiswa berhasil dihapus atau tidak ditemukan.

 5. Method ubah()

def ubah(self, nama, nilai_baru):: Method ini digunakan untuk mengubah nilai mahasiswa berdasarkan nama.
for mahasiswa in self.daftar_mahasiswa:: Melakukan iterasi pada setiap mahasiswa dalam daftar.
if mahasiswa['nama'] == nama:: Memeriksa apakah nama mahasiswa yang sedang diperiksa sama dengan nama yang ingin diubah.
mahasiswa['nilai'] = nilai_baru: Mengubah nilai mahasiswa jika ditemukan.
print(...): Menampilkan pesan bahwa data mahasiswa berhasil diubah atau tidak ditemukan.

# Diagram class

# Flowchart
![flwchrt labpy08](https://github.com/user-attachments/assets/5225095d-2756-4590-b83c-76028d4432a7)

