===================================================
PROGRAM FUZZY LOGIC UNTUK MEMILIH 5 RESTORAN TERBAIK
===================================================

Nama        : Maria Nathasya Desfera Pangestu (2211104008)
Nama        : Lintang Suminar Tyas Wening (2211104009)
Kelas       : SE0601
Mata Kuliah : Kecerdasan Buatan

----------------------------------
DESKRIPSI PROGRAM
----------------------------------
Program ini dibuat untuk menentukan 5 restoran terbaik berdasarkan dua kriteria utama:
1. Pelayanan (Servis)
2. Harga

Penilaian dilakukan menggunakan metode Logika Fuzzy (Fuzzy Logic), yang terdiri dari:
- Fuzzifikasi (membership)
- Inferensi (Metode Inferensi Mamdani dengan aturan if-then)
- Defuzzifikasi (perhitungan skor)
Hasil akhir adalah skor kelayakan dan keterangan kualitas setiap restoran.

----------------------------------
KOMPONEN FILE YANG DIBUTUHKAN
----------------------------------
Pastikan dalam satu folder terdapat file berikut:
1. fuzzy_restoran.py              => file utama program Python
2. restoran.xlsx                  => file Excel input berisi data restoran
3. Readme.txt                     => file penjelasan mengenai program ini
4. peringkat.xlsx                 => file hasil output yang ditampilkan di Excel


----------------------------------
CARA MENJALANKAN PROGRAM
----------------------------------
1. Pastikan Python sudah terinstal di komputer Anda.
2. Pastikan library `openpyxl` sudah terinstal.
   Jika belum, jalankan perintah berikut di terminal:
   pip install openpyxl

3. Jalankan program dengan perintah:
   python program_fuzzy_restoran.py

4. Hasil akan ditampilkan di layar dan juga disimpan di file:
   - peringkat.xlsx

----------------------------------
OUTPUT YANG DIHASILKAN: peringkat.xlsx
----------------------------------
File ini akan berisi 5 restoran dengan skor tertinggi, seperti contoh:

| ID          | Pelayanan | Harga  | Skor           | Keterangan Kualitas  |
|-------------|-----------|--------|----------------|----------------------|
| 23          | 77        | 22825  | 85.00          | Sangat Baik          |
| 33          | 73        | 24704  | 85.00          | Sangat Baik          |
| 66          | 80        | 20052  | 85.00          | Sangat Baik          |
| 69          | 85        | 24551  | 85.00          | Sangat Baik          |
| 79          | 92        | 22360  | 85.00          | Sangat Baik          |

----------------------------------
CATATAN TAMBAHAN
----------------------------------
- Pastikan data dalam file `restoran.xlsx` sesuai format.
- Jika skor total nol (tidak ada keanggotaan fuzzy), maka skor kelayakan = 0.
