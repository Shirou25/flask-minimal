# flask-minimal

Proyek awal Flask yang minimalis untuk membantu Anda dengan cepat membangun aplikasi web yang bersih, sederhana, dan efisien. Proyek ini dirancang agar tetap ringan dan fokus pada produktivitas, dengan seluruh kode berada di satu file (app.py), dilengkapi dengan struktur template dasar dan aset statis.

## Fitur
- Aplikasi Flask dalam satu file (app.py) untuk kemudahan dan produktivitas maksimal.
- Struktur template HTML dasar dengan gaya dan JavaScript minimal.
- Setup proyek yang sederhana dan intuitif tanpa kompleksitas berlebihan.
- Mudah disesuaikan untuk pengembangan aplikasi web secara cepat.

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

This starter project is ready to be used as a foundation for building web applications. The app.py file contains all the Flask routes and logic, making it simple to expand and customize. You can add more templates, routes, or static files as needed.

## Customization
You can easily modify:

 - The HTML structure in `templates/index.html`
 - The styling in `static/style.css`
 - The interactivity in `static/script.js`

Feel free to update the app.py file to add your routes or any additional logic to fit your needs.

## License
This project is licensed under the MIT License.

## Contributing
Feel free to fork this repository and create pull requests if you have improvements or bug fixes. If you have any suggestions, open an issue, and we’ll discuss it!

This project is built with simplicity and efficiency in mind, perfect for quickly starting small web apps or prototypes with minimal overhead.
