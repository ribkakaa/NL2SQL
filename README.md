# NL2SQL ChatBot "AssistControl"

## Deskripsi Projek
**AssistControl** adalah proyek pengembang Asisten Virtual (ChatBot) pintar berbasis teks yang dirancang khusus untuk memfatilisasi kebutuhan Administrasi. **AssistControl** menggunakan bahasa **Python**

ChatBot seperti ini sangat berguna bagi Mahasiswa Baru, Mahasiswa Aktif, ataupun Dosen dalam mendapatkan informasi Akademis ataupun yang lainnya dengan cara cepat.

Projek ini bertujuan untuk mengatasi masalah yang ada di Administrasi. Administrasi itu **mengantri dengan sangat panjang** dan **lamanya penyebaran informasi**. Karna itulah ChatBot dibuat agar Mahasiswa, Dosen, ataupun yang lainnya dapat **melihat informasi tersebut dengan sangat cepat.**

## Identifikasi Komponen Sistem dan Fungsinya pada AsistControl
| No | Nama Komponen | Kategori/Istilah Teknis | Fungsi dalam Projek NL2SQL ChatBot "AsistControl" |
| ------ | ------- | ----------------- | ------- |
| 1. | Streamlit | Antar muka Mahasiswa (User Interface/Fronted) | Fungsinya untuk Mahasiswa bisa mengetahui dan mempertanyakan sesuatu tentang Universitas mereka | 
| 2. | Python | Bahasa Pemrograman (Programming Language) | Python digunakan sebagai pengatur logika UI, AI, dan DataBase di balik layar |
| 3. | Ollama | Alat Manajemen Model AI *(LLM)* | Alat atau Software yang digunakan untuk mengunduh, menjalankan, dan mengelola bahasa *(LLM)* secara lokal di komputer |
| 4. | Qwen 2.5 | Model Bahasa Besar *(Large Language/LLM)* | kecerdasan buatan AI yang bertugas untuk memahami Bahasa Manusia dan menerjemahkannya ke dalam kode Quary SQL |
| 5. | MySQL | Sistem Manajemen DataBase | Tempat penyimpanan Data terstruktur yang dikelola oleh XAMPP dan dapat diakses menggunakan  Quary SQL |
| 6. | NL2SQL | Metode/Fitur | NL2SQL bertugas sebagai mengubah teks pertanyaan santai dari pengguna menjadi sintaks Query SQL yang valid agar bisa dibaca oleh MySQL |



## Isi Tabel Dosen
| No | Id Dosen | Nidn | Nama Lengkap | Jenis Kelamin | Id Fakultas | Id Jabatan | Pendidikan Terakhir | Usia | Tanggal Bergabung | Status Kegawaian |
| --- | ------- | -------- | ----------------- | ------------- | -----------| ---------- | ----------- | ---- | --------- | ----------- |
| 1. | 3 | 809677201 | Fajar Rahayu Kurniawan, S. Ag. M. AL | L | 6 | 1 | S2 | 50 | 2017-01-24 | DPK |
| 2. | 5 | 705954598 | Yanto Eko Lestari, S. H. M. H | L | 6 | 1 | S2 | 38 | 2022-03-15 | Kontrak |
|3. | 33 | 203694788 | Zahra Ifran Nugroho, S. Si. M. Si | P | 5 | S2 | 43 | 2015-06-18 |
