# NL2SQL ChatBot 🤖

## 📑 Deskripsi Projek
NL2SQL ChatBot adalah Asisten Belanja Virtual berbasis bahasa **Python, Ollama, Qwen 2.5, MySQL**. 

Dengan sistem ini, pengguna dapat melihat ketersediaan produk, perbandingan harga, atau riwayat transaksi menggunakan bahasa sehari-hari. ChatBot akan menerjemahkan teks tersebut dengan bahasa **SQL**, mengeksekusi ke database toko, dan mengembalikan jawaban yang mudah dipahami oleh pengguna.

| No | Nama Komponen | Kategori/Istilah Teknis | Fungsi dalam proyek NL2SQL ChatBot |
| --- | ------------- | ------------------------ | ----| 
| 1. | **Stremlit** | Antarmuka Pengguna (User Interface / Frontend) | Pustaka (Library) Python yang digunakan untuk membangun UI web chatbot, menyediakan kolom input obrolan, serta mengonversi DataFrame dari Pandas menjadi visualisasi tabel data yang rapi dan interaktif di layar pengguna. |
| 2. | **Python🐍** | Bahasa Pemrograman (Programming Language) | Bahasa Utama yang digunakan dalam membuat kode program, mengatur logika aplikasi, menghubungkan database, dan menjembatani AI dengan pengguna. |
| 3. | **Ollama🦙** | Alat Manajemen Model AI *(LLM Runner/Framework)* | Alat atau Software yang berfungsi untuk mengunduh, menjalankan, dan mengelola Model Bahasa *(LLM)* secara lokal di komputer/server sendiri. |
| 4. | **Qwen 2.5🧠** | Model Bahasa Besar *(Large Language/LLM)* | Kecerdasan buatan AI buatan Alibaba yang bertugas memahami bahasa manusia *(Natural Langguage)* dan menerjemahkannya menjadi kode perintah SQL. |
| 5. | **MySQL🐬** | Sistem Manajemen Database *(RDBMS)* | Tempat penyimpanan data terstruktur (seperti data produk, harga, stok, dan transaksi) yang dikelola melalui XAMPP dan akan diakses menggunakan query SQL. |
| 6. | **NL2SQL🤖** | Metode/Fitur (Natural Language to SQL) | Pendekatan teknologi yang bertugas mengubah teks pertanyaan santai dari pengguna menjadi sintaks query SQL yang valid agar bisa dibaca oleh MySQL. |

## 📂 Struktur NL2SQL ChatBot
```
│   app.py
│   config.py
│   push.bat
│   README.md
│   RECREATION_GUIDE.md
│   requirements.txt
│   sidebar.py
│
├───helpers
│       dataframe.py
│       env.py
│       identifiers.py
│       sql.py
│       sql_script.py
│
├───repositories
│       mysql_repository.py
│
├───services
│       chat_service.py
│       import_service.py
│       ollama_service.py
│
└───ui
        chat_view.py
        import_view.py
        schema_view.py
        sidebar.py
```

## 🏃‍➡️ Cara Menjalankan Aplikasi
### 1. Setup Ollama 🦙
```bash
  bash
  ollama run qwen2.5:latest
  ollama serve
```
### 2. XAMPP 🐬
```
   DEFAULT_MYSQL_HOST = "localhost"
   DEFAULT_MYSQL_PORT = 3306
   DEFAULT_MYSQL_USER = "root"
   DEFAULT_MYSQL_PASSWORD = ""
   DEFAULT_MYSQL_DATABASE = "shopdb"

   DEFAULT_OLLAMA_URL = "localhost:12363"
   DEFAULT_OLLAMA_MODEL = "qwen2.5:latest"****
```
### 3. Setup Aplikasi 🚀
```
    pip install -r requirements.txt
    streamlit run app.py
```
