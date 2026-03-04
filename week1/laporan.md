```markdown
# Modul 2: PENGENALAN TOOLS

## Tujuan Praktikum
1. Mahasiswa dapat melakukan instalasi tool yang digunakan (Wireshark)
2. Mahasiswa dapat menggunakan tool (Wireshark) untuk menangkap dan mengidentifikasi paket data

## 2.1 Pengantar

Pemahaman seseorang tentang protokol jaringan seringkali dapat diperdalam dengan cara "melihat protokol dalam melakukan tindakan" dan juga "mencoba eksplorasi protokol", mengamati urutan pesan yang saling bertukar antara 2 entitas, menyelidiki detail dari operasi protokol, dan sebab protokol melakukan tindakan tertentu lalu mengamati tindakan-tindakan tersebut serta konsekuensinya.

Pada praktikum jaringan komputer ini, kita akan menggunakan **Wireshark** untuk menjalankan berbagai aplikasi jaringan dalam skenario yang berbeda menggunakan komputer sendiri. Wireshark merupakan aplikasi untuk mengamati pesan yang bertukar antara entitas protokol yang disebut dengan **Packet Sniffer**.

### Struktur Packet Sniffer

Packet Sniffer terdiri dari dua bagian utama:
- **Packet Capture Library**: Menerima salinan dari setiap frame link layer yang dikirim/diterima oleh komputer
- **Packet Analyzer**: Menampilkan isi dari semua bidang dalam pesan protokol

## 2.2 Wireshark

Wireshark adalah penganalisa protokol jaringan gratis yang berjalan di komputer Windows, Mac, dan Linux/Unix. Wireshark memiliki fungsionalitas yang kaya yang mencakup kemampuan untuk menganalisis ratusan protokol, dan antarmuka pengguna yang dirancang dengan baik.

### Instalasi Wireshark

Untuk menginstal Wireshark:
1. Kunjungi http://www.wireshark.org/download.html
2. Unduh dan instal binary Wireshark sesuai sistem operasi Anda
3. Perangkat lunak libpcap/WinPcap akan diinstal otomatis jika belum ada

## 2.3 Menjalankan Wireshark

Saat Anda menjalankan program Wireshark, Anda akan mendapatkan tampilan awal seperti berikut:

### Tampilan Awal Wireshark

![Tampilan Awal Wireshark](screenshot1.png)

**Keterangan:**
- Di bagian **Capture**, terdapat daftar **interfaces** yang tersedia
- Interface yang tersedia tergantung pada koneksi jaringan komputer Anda (Wi-Fi, Ethernet, dll)
- Klik dua kali pada interface yang ingin digunakan untuk memulai capture paket

### Komponen Antarmuka Wireshark

Antarmuka Wireshark memiliki lima komponen utama:

1. **Command Menu**: Menu pull-down standar yang terletak di bagian atas jendela Wireshark
   - Menu **File**: Untuk menyimpan/membuka data paket
   - Menu **Capture**: Untuk memulai/menghentikan pengambilan paket

2. **Packet-Listing Window**: Menampilkan ringkasan satu baris untuk setiap paket yang diambil
   - Nomor paket
   - Sumber dan alamat tujuan
   - Jenis protokol
   - Informasi khusus protokol

3. **Packet-Header Details Window**: Memberikan rincian tentang paket yang dipilih
   - Informasi frame Ethernet
   - Datagram IP
   - Segmen TCP/UDP
   - Protokol tingkat tertinggi (HTTP, DNS, dll)

4. **Packet-Contents Window**: Menampilkan seluruh isi frame yang diambil dalam format ASCII dan heksadesimal

5. **Packet Display Filter Field**: Bidang untuk memasukkan filter protokol atau informasi lain

## 2.4 Menggunakan Wireshark Untuk Test Run

### Langkah-Langkah Test Run

1. **Jalankan browser web** Anda

2. **Jalankan Wireshark** - Anda akan melihat jendela seperti di atas

3. **Mulai pengambilan paket**:
   - Pilih menu **Capture** → **Interfaces**
   - Pilih interface yang aktif (Wi-Fi atau Ethernet)
   - Klik **Start** untuk memulai capture

4. **Generate traffic jaringan**:
   - Buka browser
   - Kunjungi URL: http://gaia.cs.umass.edu/wireshark-labs/INTRO-wireshark-file1.html
   - Browser akan menghubungi server HTTP dan bertukar pesan HTTP

5. **Hentikan capture**:
   - Klik tombol **Stop** (kotak merah) atau
   - Pilih menu **Capture** → **Stop**

### Hasil Capture Paket

Setelah melakukan capture, tampilan Wireshark akan terlihat seperti berikut:

![Wireshark Window Saat dan Setelah Capture](screenshot2.png)

**Keterangan Gambar:**
- **Panel Atas**: Menampilkan daftar semua paket yang tertangkap
- **Panel Tengah**: Menampilkan detail header dari paket yang dipilih
- **Panel Bawah**: Menampilkan isi paket dalam format hex dan ASCII

### Filter Paket HTTP

Untuk menampilkan hanya paket HTTP:
1. Ketik **"http"** (huruf kecil) di kolom **Display Filter**
2. Tekan **Enter** atau klik **Apply**
3. Hanya paket HTTP yang akan ditampilkan

### Analisis Paket HTTP GET

Setelah menerapkan filter HTTP, Anda dapat melihat:
- Pesan **HTTP GET** yang dikirim dari komputer ke server
- Pesan **HTTP Response** dari server ke komputer
- Detail protokol yang dapat diperluas/ditutup dengan klik tanda **+/-**

## Tugas Praktikum

1. Instal Wireshark di komputer Anda
2. Jalankan Wireshark dan lakukan capture paket
3. Kunjungi website sederhana untuk generate traffic
4. Terapkan filter untuk melihat paket HTTP
5. Identifikasi dan catat informasi berikut:
   - Alamat IP sumber dan tujuan
   - Protokol yang digunakan
   - Informasi header HTTP

## Kesimpulan

Wireshark adalah tool yang sangat powerful untuk:
- Menganalisis lalu lintas jaringan
- Troubleshooting masalah jaringan
- Mempelajari cara kerja protokol jaringan
- Keamanan jaringan

Dengan memahami cara menggunakan Wireshark, mahasiswa dapat melihat secara langsung bagaimana protokol jaringan berkomunikasi dan bertukar pesan.

## Referensi

- Wireshark Official Website: http://www.wireshark.org/
- Wireshark User Guide: http://www.wireshark.org/docs/wsug_html_chunked/
- Wireshark FAQ: http://www.wireshark.org/faq.html

---

**Catatan**: Pastikan untuk menyimpan screenshot hasil praktikum Anda sebagai bukti pelaksanaan modul ini.
```