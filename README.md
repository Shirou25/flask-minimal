# flask-minimal

Proyek awal Flask yang minimalis untuk membantu Anda dengan cepat membangun aplikasi web yang bersih, sederhana, dan efisien. Proyek ini dirancang agar tetap ringan dan fokus pada produktivitas, dengan seluruh kode berada di satu file (app.py), dilengkapi dengan struktur template dasar dan aset statis.

## Fitur
- Aplikasi Flask dalam satu file (app.py) untuk kemudahan dan produktivitas maksimal.
- Struktur template HTML dasar dengan gaya dan JavaScript minimal.
- Setup proyek yang sederhana dan intuitif tanpa kompleksitas berlebihan.
- Mudah disesuaikan untuk pengembangan aplikasi web secara cepat.

Prasyarat
Sebelum memulai, pastikan Anda memiliki:

Akses ke instance EC2 Ubuntu.
Python 3 dan pip terinstal.
Akses root atau sudo ke server.

## Persiapan
```bash
sudo apt update
sudo apt install python3 python3-venv python3-pip -y
```

## Instalasi

1. Clone repositori:
   ```bash
   git clone https://github.com/yourusername/flask-minimal.git
   cd flask-minimal
   ```

2. Buat virtual environment (disarankan):
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Instal semua dependensi yang dibutuhkan:
   ```bash
   pip install -r requirements.txt
   ```

4. Jalankan aplikasi:
   ```bash
   python app.py
   ```

Aplikasi Flask akan berjalan, dan Anda bisa mengaksesnya melalui browser dengan membuka alamat: http://localhost:5000

## Usage

Menjalankan Aplikasi Flask Secara Otomatis Saat Reboot dengan systemd
Untuk memastikan aplikasi Flask Anda berjalan otomatis saat instance EC2 Ubuntu di-reboot, ikuti langkah-langkah berikut:

1. Buat File Service systemd
   Buat file service:
   sudo nano /etc/systemd/system/flask-app.service
   Tambahkan konfigurasi berikut:
   
   [Unit]
Description=Aplikasi Flask Minimal
After=network.target

[Service]
User=ubuntu
WorkingDirectory=/home/ubuntu/flask-minimal
Environment="PATH=/home/ubuntu/flask-minimal/venv/bin"
ExecStart=/home/ubuntu/flask-minimal/venv/bin/python app.py
Restart=always

[Install]
WantedBy=multi-user.target

