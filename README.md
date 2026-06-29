# local-ransomware-simulation

# Simulasi Malware: Local Ransomware (XOR Encryption)

Tugas Nilai Tambahan - Computer Security

## Deskripsi
Program ini adalah simulasi non-destruktif dari mekanisme kerja Ransomware yang dibuat menggunakan bahasa C++. Program mengidentifikasi file target lokal, melakukan enkripsi berbasis bitwise XOR secara simetris, dan mengubah ekstensi file menjadi `.locked`. Program ini juga menyediakan fitur dekripsi untuk mengembalikan file ke kondisi semula.

## Batasan Keamanan Sandbox
- Hanya berjalan pada file lokal yang secara eksplisit dimasukkan lewat argumen CLI.
- Tidak menyebar ke jaringan dan tidak menyentuh file sistem operasi.

## Alur Pengujian dan Penggunaan
1. Pembuatan file dummy target (`test.txt`).
2. Proses Enkripsi:
   `malware.exe encrypt test.txt`
3. Proses Dekripsi:
   `malware.exe decrypt test.txt.locked`
