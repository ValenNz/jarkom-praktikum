# Laporan Praktikum Jaringan Komputer - Modul 1
## Running Modul (Rules & Tools Setup)

### Identitas Praktikan
| Item | Keterangan |
|------|------------|
| **Nama** | [Isi Nama Lengkap Anda] |
| **NIM** | [Isi NIM Anda] |
| **Kelas** | [Isi Kelas Praktikum Anda] |
| **Tanggal** | [Isi Tanggal Praktikum] |
| **Asisten** | [Isi Nama Asisten jika ada] |

---

## 1. Tujuan Praktikum
Berdasarkan modul praktikum Jaringan Komputer Semester Genap 2025/2026, tujuan dari Modul 1 adalah:
1. Mahasiswa mengetahui aturan dan sistem pelaksanaan praktikum.
2. Mahasiswa mengetahui tools yang akan digunakan dan memastikan tools berfungsi dengan baik selama pelaksanaan praktikum.

---

## 2. Persiapan Tools
Sebelum memulai praktikum, dilakukan pengecekan dan instalasi tools yang wajib digunakan selama 16 pertemuan ke depan.

### 2.1 Wireshark
Wireshark adalah aplikasi packet sniffer yang digunakan untuk menganalisis protokol jaringan.
- **Status:** Terinstall ✅
- **Versi:** [Isi Versi Wireshark Anda, misal: 4.0.3]
- **Link Download:** [www.wireshark.org](http://www.wireshark.org/)

### 2.2 Python
Python digunakan untuk modul Socket Programming.
- **Status:** Terinstall ✅
- **Versi:** [Isi Versi Python Anda, misal: 3.11.0]
- **Link Download:** [www.python.org](https://www.python.org/downloads/)

---

## 3. Langkah Kerja
Berikut adalah langkah-langkah yang dilakukan selama praktikum Modul 1:

1. **Briefing Aturan Praktikum**
   - Mendengarkan penjelasan asisten mengenai tata tertib laboratorium (TULT Lantai 6 & 7).
   - Memahami sistem penilaian, kehadiran (minimal 75%), dan sanksi pelanggaran.
   - Memahami alur 16 modul praktikum hingga Tugas Besar.

2. **Pengecekan Tools**
   - Memastikan Wireshark dan Python sudah terinstall di komputer laboratorium/personal.
   - Melakukan update jika diperlukan.

3. **Test Run Wireshark**
   - Mengunduh file `soal1.pcap` dari LMS kelas praktikum.
   - Membuka aplikasi Wireshark.
   - Melakukan open file `soal1.pcap` melalui menu `File > Open`.
   - Mengamati fitur dasar Wireshark (Packet List, Packet Details, Packet Bytes).

---

## 4. Hasil dan Pembahasan

### 4.1 Tampilan Awal Wireshark
Berikut adalah tampilan awal Wireshark sebelum membuka file trace. Terlihat daftar interface jaringan yang tersedia.

![Tampilan Awal Wireshark](images/wireshark_home.png)
*Gambar 1: Tampilan awal Wireshark saat pertama kali dibuka.*

### 4.2 Membuka File soal1.pcap
File `soal1.pcap` berhasil dibuka. Berikut adalah tangkapan layar saat file trace dimuat ke dalam Wireshark.

![Membuka soal1.pcap](images/wireshark_soal1.png)
*Gambar 2: Tampilan Wireshark setelah membuka file soal1.pcap dari LMS.*

### 4.3 Analisis Singkat Paket
Pada file `soal1.pcap`, dapat dilihat beberapa protokol yang tertangkap. Berikut adalah detail salah satu paket yang dipilih (misalnya paket HTTP atau TCP pertama).

![Detail Paket](images/wireshark_detail.png)
*Gambar 3: Detail paket pada jendela Packet Details.*

### 4.4 Verifikasi Python
Berikut adalah tangkapan layar Command Prompt/Terminal saat mengecek versi Python untuk memastikan tools siap digunakan pada modul selanjutnya (Modul 7 & 9).

![Cek Python](images/python_version.png)
*Gambar 4: Verifikasi instalasi Python melalui command line.*

---

## 5. Kesimpulan
Berdasarkan praktikum Modul 1 ini, dapat disimpulkan bahwa:
1. Praktikan telah memahami aturan main, sistem penilaian, dan sanksi yang berlaku di Laboratorium Informatika Universitas Telkom.
2. Tools utama yaitu **Wireshark** dan **Python** telah berhasil diinstall dan berfungsi dengan baik.
3. Praktikan mampu membuka file trace (`.pcap`) dan memahami antarmuka dasar Wireshark yang akan digunakan pada modul-modul selanjutnya (HTTP, DNS, TCP, dll).
4. Kesiapan tools ini sangat penting untuk kelancaran praktikum hingga penyusunan Tugas Besar.

---

## 6. Lampiran
- File `soal1.pcap` (Jika diizinkan untuk dilampirkan).
- Dokumentasi foto saat praktikum (Opsional).
