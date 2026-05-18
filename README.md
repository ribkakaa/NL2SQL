# NL2SQL ChatBot 🤖

## 📑 Deskripisi NL2SQL
NL2SQL ChatBot adalah Asisten Belanja Virtual berbasis bahasa **Python, Ollama, Qwen 2.5, dan NL2SQL**. 

Dengan sistem ini, pengguna dapat melihat ketersediaan produk, perbandingan harga, atau riwayat transaksi menggunakan bahasa sehari-hari. ChatBot akan menerjemahkan teks tersebut dengan bahasa SQL, mengeksekusi ke data base toko, dan mengembaklikan jawaban yang mudah dipahami oleh pengguna.

| No | Nama Komponen | Katergor/Istilah Teknis | Fungsi dalam proyek NL2SQL ChatBot |
| --- | ------------- | ------------------------ | ----| 
| 1. | Python 🐍 | Bahasa Pemograman (Programming Language) | Bahasa Utama yang digunakan dalam membuat kode program, mengatur logika aplikasi, menghubungkan data base, dan menjebatani AI dengan pengguna.
| 2. | Ollama 🦙 | Alat Manajemen Model AI *(LLM Runner/Framwork)* | Alat atau Software yang berfungsi untuk mengunduh, menjalankan, dan mengelola Model Bahasa *(LLM)* secara lokal di komputer/server sendiri.
| 3. | Qwen 2.5 🧠 | Model Besar Bahasa *(Large Langguage/LLM)* | Kecerdasab buatan AI buatan Alibaba yang bertugas memahami bahasa manusia *(Natural Langguage)* dan menterjemahkannya menjadi kode perintah SQL.
| 4. | NL2SQL 🐬 | Sistem Manajemen DataBase | Tempat penyimpanan data terstruktur (seperti data produk, harga, stok, dan transaksi) yang nantinya akan diakses menggunakan query SQL. |

## 📂 Strukrur NL2SQL ChatBot
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
   ollama run qwen2.5:latest
   ollama serve
```
### 2. XAMPP 🐬

    Run XAMPP Control Panel
    Start Apache dan MySQL

### 3. Setup Aplikasi 🚀
```
    pip install -r requirements.txt
    streamlit run app.py
```
