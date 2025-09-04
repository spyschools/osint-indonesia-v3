# osint-indonesia-v3
Tools OSINT Indonesia, untuk cek NIK & No HP. Script ini tidak akan ambil data dari database ilegal, tapi hanya dari sumber OSINT publik.

Files:
- osint_v3.py         (main scanner with multi-threaded Google dorking)
- kode_wilayah.json   (provinsi/kabupaten/kecamatan full)
- README.md

$ sudo apt update && sudo apt install python3 python3-pip -y

$ git clone https://github.com/spyschools/osint-indonesia-v3.git

$ cd osint-indonesia-v3

$ pip3 install requests beautifulsoup4

Jalankan scanner contoh:
$ python3 osint_v3.py 3208074509870004

$ python3 osint_v3.py 3275124308050003 +6281234567890

*UPDATE
$ python3 osint_builder.py

$ unzip osint_v3.zip -d osint_v3_pkg

$ cd osint_v3_pkg

$ python3 osint_v3.py 3275124308050003 +6281234567890

Output:
- report_TIMESTAMP.html (buka di browser)

Notes:
- Google scraping dapat rate-limit; gunakan bijak.
- Jika API wilayah.id berubah, generator bisa gagal; kamu bisa isi kode_wilayah.json manual.
- gunakan tools ini dengan bijak, tools ini hanya untuk pengetesan dan pengembangan

gunakan tools ini dengan bijak, tools ini hanya untuk pengetesan dan pengembangan
