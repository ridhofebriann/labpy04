# labpy04
Nama        : M.Ridho Febrian <p>

Kelas       : TI.24.A.5 <p>

Nim         : 312410500 <p>

Mata kuliah : Bahasa Pemrograman <p>

# penjelasan flowchart Praktikum 4 

1. Mulai

Penjelasan: Ini adalah titik awal dari alur program. Program dimulai di sini.

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw1.png?raw=true)

2. Input Data

Penjelasan: Program meminta pengguna untuk memasukkan data berikut:

NIM: Nomor Induk Mahasiswa

Nama: Nama Mahasiswa

Nilai Tugas: Nilai tugas dalam rentang 0-100

Nilai UTS: Nilai Ujian Tengah Semester dalam rentang 0-100

Nilai UAS: Nilai Ujian Akhir Semester dalam rentang 0-100

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw2.png?raw=true)

3. Validasi Input

Penjelasan: Program memvalidasi input dengan langkah-langkah berikut:

Memastikan bahwa NIM dan Nama tidak kosong.

Memastikan bahwa nilai Tugas, UTS, dan UAS berada dalam rentang 0-100.

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw3.png?raw=true)

Output:

Jika input valid, alur dilanjutkan ke langkah berikutnya.

Jika input tidak valid, program kembali ke langkah Input Data.

4. Hitung Nilai Akhir

Penjelasan: Program menghitung nilai akhir mahasiswa menggunakan rumus:

Nilai Akhir = (Tugas * 0.3) + (UTS * 0.35) + (UAS * 0.35)

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw4.png?raw=true)

5. Simpan Data

Penjelasan: Program menyimpan data mahasiswa yang telah dihitung nilai akhirnya ke dalam list atau database.

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw5.png?raw=true)

6. Tanya Tambah Data

Penjelasan: Program menanyakan kepada pengguna apakah ingin menambah data mahasiswa lagi (y/t):

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw6.png?raw=true)

Jika pengguna menjawab 'y' (ya), program kembali ke langkah Input Data.

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw7.png?raw=true)

Jika pengguna menjawab 't' (tidak), program melanjutkan ke langkah Tampilkan Data.

7. Tampilkan Data

Penjelasan: Jika ada data yang telah disimpan, program menampilkan data mahasiswa tersebut dalam format tabel atau daftar yang rapi.

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw8.png?raw=true)

8. Selesai
Penjelasan: Ini adalah titik akhir dari alur program. Program berakhir di sini.

![foto](https://github.com/ridhofebriann/labpy04/blob/main/fw9.png?raw=true)

# penjelasan langkah demi langkah:

1. Mulai: Ini adalah langkah awal di mana program dimulai.

2. Input Data: Pengguna diminta untuk memasukkan NIM, Nama, Nilai Tugas, Nilai UTS, dan Nilai UAS. Data ini diinput ke dalam program untuk diproses.

3. Validasi Input: Program memeriksa apakah input data yang dimasukkan valid. Validasi mencakup pengecekan apakah NIM dan Nama tidak kosong dan apakah nilai Tugas, UTS, dan UAS berada dalam rentang 0-100.

Jika input tidak valid, program kembali meminta pengguna untuk memasukkan data yang benar.

4. Hitung Nilai Akhir: Jika input valid, program menghitung nilai akhir menggunakan rumus yang sudah ditentukan.

5. Simpan Data: Setelah nilai akhir dihitung, data mahasiswa disimpan dalam list atau database.

6. Tanya Tambah Data: Program menanyakan kepada pengguna apakah ingin menambah data mahasiswa lainnya. Jika ya, program kembali ke langkah input data. Jika tidak, lanjut ke langkah berikutnya.

7. Tampilkan Data: Program menampilkan data mahasiswa yang telah disimpan dalam format tabel yang rapi.

8. Selesai: Program selesai dan berakhir di sini.

# berikut Gambar flowchart nya:

![foto](https://github.com/ridhofebriann/labpy04/blob/main/flowchart..png?raw=true)

# penjelasan code program:

1. Definisi Fungsi

Program ini dimulai dengan mendefinisikan beberapa fungsi yang bertugas untuk memproses data dan menampilkan informasi.

a. 'hitung_nilai_akhir(tugas, uts, uas)'

  Tujuan: Menghitung nilai akhir mahasiswa berdasarkan bobot yang telah ditentukan untuk 
  setiap komponen nilai.

Parameter:

'tugas': Nilai tugas mahasiswa.

'uts': Nilai Ujian Tengah Semester (UTS).

'uas': Nilai Ujian Akhir Semester (UAS).

Proses:

Menggunakan rumus: [ \text{Nilai Akhir} = (tugas \times 0.3) + (uts \times 0.35) + (uas \times 0.35) ]

Output: Mengembalikan nilai akhir yang dihitung.

b. tampilkan_header()

Tujuan: Menampilkan header tabel yang berisi informasi kolom.

Proses:

Mencetak garis pembatas untuk tabel.

Menampilkan judul tabel "DAFTAR NILAI MAHASISWA".

Menampilkan nama kolom seperti "NO", "NAMA", "NIM", "TUGAS", "UTS", "UAS", dan "NILAI AKHIR".

Output: Tidak mengembalikan nilai, hanya mencetak ke layar.

c. 'tampilkan_data_mahasiswa(data_mahasiswa)'

Tujuan: Menampilkan data mahasiswa dalam format tabel.

Parameter:

'data_mahasiswa': List yang berisi dictionary untuk setiap mahasiswa.

Proses:

Menggunakan 'enumerate' untuk mendapatkan indeks dan data mahasiswa.

Mencetak setiap data mahasiswa dalam format yang terstruktur, dengan dua desimal untuk nilai.

Output: Tidak mengembalikan nilai, hanya mencetak ke layar.

2. Fungsi 'main()'

Fungsi ini adalah inti dari program, di mana alur utama program dijalankan.

a. Inisialisasi

List Kosong: Mendeklarasikan data_mahasiswa sebagai list kosong untuk menyimpan 'data 
mahasiswa'.

b. Loop Input Data

Loop Tak Terbatas: Program menggunakan loop 'while True' untuk terus meminta input data hingga pengguna memilih untuk berhenti.

Input Nama dan NIM:

Meminta pengguna untuk memasukkan nama mahasiswa.

Memeriksa apakah nama yang dimasukkan kosong. Jika kosong, program mencetak pesan kesalahan dan melanjutkan ke iterasi berikutnya.

Meminta pengguna untuk memasukkan NIM mahasiswa.

Memeriksa apakah NIM yang dimasukkan kosong. Jika kosong, program mencetak pesan kesalahan dan melanjutkan ke iterasi berikutnya.

c. Input Nilai

Input Nilai Tugas, UTS, dan UAS:

Meminta pengguna untuk memasukkan nilai tugas, UTS, dan UAS.

Menggunakan 'try-except' untuk menangkap kesalahan konversi nilai ke float.

Memeriksa apakah nilai berada dalam rentang 0-100. Jika tidak, program mencetak pesan kesalahan dan melanjutkan ke iterasi berikutnya.

d. Menghitung Nilai Akhir

Setelah semua input valid, program memanggil fungsi 'hitung_nilai_akhir()' dengan nilai tugas, UTS, dan UAS sebagai argumen.

Nilai akhir yang dihitung disimpan dalam variabel 'nilai_akhir'.

e. Menyimpan Data Mahasiswa

Data mahasiswa disimpan dalam dictionary dengan kunci:

'Nama': nama mahasiswa.

'NIM': NIM mahasiswa.

'Tugas': nilai tugas.

'UTS': nilai UTS.

'UAS': nilai UAS.

'Nilai Akhir': nilai akhir yang dihitung.

Dictionary tersebut ditambahkan ke list 'data_mahasiswa'.

f. Konfirmasi Tambah Data


Setelah menyimpan data, program menanyakan kepada pengguna apakah ingin menambah data lagi.

Jika pengguna menjawab 'y', loop akan dimulai lagi; jika tidak, loop akan berhenti.

3. Menampilkan Data Mahasiswa

Setelah keluar dari loop, program memeriksa apakah ada data mahasiswa yang dimasukkan.

Jika 'data_mahasiswa' tidak kosong:

Memanggil 'tampilkan_header()' untuk mencetak header tabel.

Memanggil 'tampilkan_data_mahasiswa(data _mahasiswa)' untuk mencetak semua data mahasiswa dalam 

format tabel.

Jika 'data_mahasiswa' kosong, program mencetak pesan bahwa tidak ada data mahasiswa yang 

dimasukkan.

4. Menjalankan Program

Program dijalankan dengan memanggil fungsi 'main()' jika file ini dijalankan sebagai program utama. Ini memastikan bahwa semua fungsi dan logika yang telah didefinisikan akan dieksekusi.

# Berikut foto code program python:

![foto]()

# berikut hasil code program yang sudah di jalankan:

!{foto}()




