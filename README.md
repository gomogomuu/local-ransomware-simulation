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

   ##  Step-by-Step Verification Procedure

## cara nya:


1. **Buka CMD di Direktori:** Buka folder proyek di File Explorer, ketik `cmd` pada *address bar* di atas, lalu tekan **Enter**.
2. **Kunci File (Enkripsi):** Jalankan perintah `malware.exe encrypt test.txt` untuk mengunci file menjadi `test.txt.locked` (isi teks hancur).
3. **Buka File (Dekripsi):** Jalankan perintah `malware.exe decrypt test.txt.locked` untuk memulihkan file teks kembali ke kondisi semula.
