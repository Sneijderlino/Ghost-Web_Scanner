<!-- ==================== BANNER ==================== -->
<h1 align="center">💀 Ghost Web Scanner</h1>
<h3 align="center">Tool Recon & Security Scan Web dengan aura Hacker Dark-Red</h3>
<p align="center">
  <img src="img/1.png" alt="Ghost Web Scanner Preview" width="100%" style="border-radius:12px; box-shadow:0 0 25px #ff0000;">
</p>

---

## 📋 Daftar Isi

- [Tentang](#-tentang)
- [Fitur](#-fitur)
- [Preview](#-preview)
- [Instalasi](#-instalasi)
  - [Windows](#-windows)
  - [Kali Linux / Ubuntu](#-kali-linux--ubuntu)
  - [Termux](#-termux)
- [Penggunaan](#-penggunaan)
- [Persyaratan](#-persyaratan)
- [Kontribusi](#-kontribusi)
- [Lisensi](#-lisensi)
- [Disclaimer](#-disclaimer)

---

## 👻 Tentang

`Ghost-Web-Scanner` adalah skrip Python untuk scan keamanan web dan intel pengumpulan informasi otomatis, hasil rancangan `Sneijderlino`.



> ⚠️ Hanya untuk edukasi, pengujian keamanan dan riset (ethical hacking). Jangan gunakan tanpa izin pemilik target.

---

## 🔥 Fitur

- Mendukung mode multi-platform: Windows, Kali Linux, Termux
- Auto recon: subdomain enumeration, header web server, firewall WAF basic
- Directory brute-force dari path populer (`admin`, `login`, `.env`, `wp-admin`, dll.)
- Form scanner: deteksi login form, CSRF, method GET vs POST
- Param scan: cek XSS & SQLi sederhana menggunakan payload uji
- Laporan akhir: summary target, proteksi, tech stack, score kerentanan
- UI terminal yang keren dan hacker-looking

---

## 🖼️ Preview

<p align="center">
  <img src="img/2.png" alt="Ghost Web Scanner Screenshot" width="80%" style="border-radius:12px; box-shadow: 0 0 30px #ff0000;" />
</p>


<p align="center">
  <img src="img/3.png" alt="Ghost Web Scanner Screenshot" width="80%" style="border-radius:12px; box-shadow: 0 0 30px #ff0000;" />
</p>


<p align="center">
  <img src="img/5.png" alt="Ghost Web Scanner Screenshot" width="80%" style="border-radius:12px; box-shadow: 0 0 30px #ff0000;" />
</p>

<p align="center">
  <img src="img/4.png" alt="Ghost Web Scanner Screenshot" width="80%" style="border-radius:12px; box-shadow: 0 0 30px #ff0000;" />
</p>
---

## 🛠️ Instalasi

### 🔧 Windows

1. Install Python 3.11+ dari https://www.python.org/downloads/ (pastikan centang `Add Python to PATH`).
2. Install Git: https://git-scm.com/downloads.
3. Buka Git Bash atau PowerShell.
4. Clone repo:
   ```bash
   git clone https://github.com/Sneijderlino/Ghost-Web_Scanner.git
   cd Ghost-Web-scanner
   ```
5. Install dependencies:
   ```bash
   python -m pip install -r requirements.txt
   ```
6. Jalankan:
   ```bash
   python Ghost-Web-Scanner.py
   ```

Catatan: di Windows, fitur beberapa deteksi tambahan Termux/Kali tidak tersedia (seperti `termux-battery-status`).

### 🔧 Kali Linux / Ubuntu

1. Buka terminal.
2. Clone repo:
   ```bash
   git clone https://github.com/Sneijderlino/Ghost-Web_Scanner.git
   cd Ghost-Web-scanner
   ```
3. Install Python & modul:
   ```bash
   sudo apt update && sudo apt install -y python3 python3-pip git
   python3 -m pip install --upgrade pip
   python3 -m pip install -r requirements.txt
   ```
4. Jalankan:
   ```bash
   python3 Ghost-Web-Scanner.py
   ```

### 📱 Termux (Android)

1. Install Termux dari F-Droid.
2. Update & upgrade:
   ```bash
   pkg update && pkg upgrade -y
   ```
3. Install tools dasar:
   ```bash
   pkg install -y python git clang make openssl-tool
   ```
4. Clone repo:
   ```bash
   git clone https://github.com/Sneijderlino/Ghost-Web_Scanner.git
   cd Ghost-Web-scanner
   ```
5. Install dependencies Python:
   ```bash
   pip install --upgrade pip
   pip install -r requirements.txt
   ```
6. Jalankan versi terminal:
   ```bash
   python Ghost-Web-Scanner.py
   ```

> ⚠️ Di Termux, beberapa fitur khusus (misal API khusus Android atau perangkat keras) bisa terbatas.

---

## ▶️ Penggunaan

1. Jalankan script seperti di atas.
2. Masukkan target URL (contoh `example.com` atau `http://example.com`).
3. Biarkan proses berjalan sampai selesai.
4. Baca output: subdomain ditemukan, path kuat, form dan potensi XSS / SQLi.

Contoh:

```bash
python Ghost-Web-Scanner.py
# lalu masukkan target
```

---

## ✅ Persyaratan

- Python 3.11+
- requests
- beautifulsoup4
- urllib3

File `requirements.txt` berisi paket-paket di atas.

---

## 🤝 Kontribusi

1. Fork repo
2. Buat branch baru (`git checkout -b feature/nama-fitur`)
3. Commit perubahan (`git commit -m "Tambah fitur X"`)
4. Push (`git push origin feature/nama-fitur`)
5. Buka Pull Request

Lihat `CONTRIBUTING.md` untuk detail.

---

## 📝 Lisensi

`Ghost-Web-Scanner` dilisensikan di bawah MIT License. Lihat file `LICENSE`.

---

## ⚠️ Disclaimer

Proyek ini hanya untuk edukasi dan penelitian keamanan etis. Penulis tidak bertanggung jawab atas penyalahgunaan. Pastikan Anda memiliki izin sebelum melakukan scanning pada sistem/website pihak ketiga.

---

<p align="center">⚡ Ghost Web Scanner - Stay safe, stay ethical ⚡</p>
# Ghost-Web_Scanner
