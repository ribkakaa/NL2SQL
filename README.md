# NL2SQL ChatBot "AssistControl" 

## Deskripsi Proyek 📑
**AssistControl** adalah proyek pengembang Asisten Virtual (ChatBot) pintar berbasis teks yang dirancang khusus untuk memfasilitasi kebutuhan Administrasi. **AssistControl** menggunakan bahasa **Python**

ChatBot seperti ini sangat berguna bagi Mahasiswa Baru, Mahasiswa Aktif, ataupun Dosen dalam mendapatkan informasi Akademik ataupun yang lainnya dengan cara cepat.

Proyek ini bertujuan untuk mengatasi masalah yang ada di Administrasi. Proses Administrasi yang konvensional sering kali **memakan waktu yang cukup lama**, sehingga mengakibatkan penyaluran informasi juga menjadi **sangat lambat.** Karna itulah ChatBot dibuat agar Mahasiswa, Dosen, ataupun yang lainnya dapat **melihat informasi tersebut dengan sangat cepat.**


## Identifikasi Komponen Sistem dan Fungsinya pada AssistControl 
| No | Nama Komponen | Kategori/Istilah Teknis | Fungsi dalam Proyek NL2SQL ChatBot "AssistControl" |
| ------ | ------- | ----------------- | ------- |
| 1. | Streamlit | Antar muka Mahasiswa (User Interface/Fronted) | Fungsinya untuk Mahasiswa bisa mengetahui dan mempertanyakan sesuatu tentang Universitas mereka | 
| 2. | Python | Bahasa Pemrograman (Programming Language) | Python digunakan sebagai pengatur logika UI, AI, dan DataBase di balik layar |
| 3. | Ollama | Alat Manajemen Model AI *(LLM)* | Alat atau Software yang digunakan untuk mengunduh, menjalankan, dan mengelola bahasa *(LLM)* secara lokal di komputer |
| 4. | Qwen 2.5 | Model Bahasa Besar *(Large Language/LLM)* | kecerdasan buatan AI yang bertugas untuk memahami Bahasa Manusia dan menerjemahkannya ke dalam kode Quary SQL |
| 5. | MySQL | Sistem Manajemen DataBase | Tempat penyimpanan Data terstruktur yang dikelola oleh XAMPP dan dapat diakses menggunakan  Quary SQL |
| 6. | NL2SQL | Metode/Fitur | NL2SQL bertugas sebagai mengubah teks pertanyaan santai dari pengguna menjadi sintaks Query SQL yang valid agar bisa dibaca oleh MySQL |


## Kolom Tabel `dosen`
| id_dosen | nidn | nama_lengkap | jenis_kelamin | id_fakultas | id_jabatan | pendidikan_terakhir | usia | tanggal_bergabung | status_kegawaian | foto |
| ------- | -------- | ----------------- | ------------- | -----------| ---------- | ----------- | ---- | --------- | ----------- | ---- |
| 3 | 809677201 | Fajar Rahayu Kurniawan, S.Ag., M.A | L | 6 | 1 | S2 | 50 | 2017-01-24 | DPK | NULL |
| 5 | 705954598 | Yanto Eko Lestari, S.H., M.H | L | 6 | 1 | S2 | 38 | 2022-03-15 | Kontrak | NULL |
| 33 | 203694788 | Zahra Ifran Nugroho, S.Si., M.Si | P | 5 | 1 | S2 | 43 | 2015-06-18 | Tetap | NULL |

## Kolom Tabel `fakultas`
| id_fakultas | nama_fakultas | kode_fakultas | dekan | id_dekan |
| ----------- | ------------ | ---------------- | ---- | --- |
| 1 | Fakultas Matematika dan IPA | FMIPA | Prof. Dr. Hendra Kusuma, M.Si | NULL |
| 5 | Fakultas Hukum | FH | Prof. Dr. Ahmad Fauzi, S.H., M.H | NULL |
| 9 | Fakultas Pertanian | FP | Prof. Dr. Agus Prasetyo, M.P | NULL |

## Kolom Tabel `jabatan_fungsional`
| id_jabatan | nama_jabatan | kode_jabatan | angka_kredit_min |
| ---------- | ---------- | ------------ | ----------- |
| 1 | Asisten Ahli | AA | 150 |
| 2 | Lektor | L | 200 |
| 3 | Lektor Kepala | LK | 400 |

## Kolom Tabel `remunerasi`
| id_remunerasi | id_dosen | tahun | bulan | gaji_pokok | tunjangan_jabatan | tunjangan_fungsional |tunjangan kinerja | total_remunerasi |
| ------- | ----------- | --------- | --------- | --------- | ------- | ------- | -------- | -------- |
| 1 | 1 | 2025| 1 | 5931672.70 | 732978.36 | 634011.55 | 1684310.65 | 8982973.26 |
| 2 | 2 | 2025 | 1 | 5076887.94 | 1196191.50 | 680932.97 | 1628272.04 | 8582284.45 |
| 3 | 3 | 2025 | 1 | 4303375.51 | 615703.57 | 552301.70 | 761593.27 | 6232974.05 |

## Struktur Projek
### AssistControl

│   .env
│   app.py
│   config.py
│   README.md
│   requirements.txt
│   
├───.streamlit
│       config.toml
│       
├───assets
│       icon.png
│       
├───helpers
│       dataframe.py
│       env.py
│       identifiers.py
│       sql.py
│       sql_script.py
│       
├───repositories
│       repository.py
│       
├───services
│       chat_service.py
│       import_service.py
│       ollama_services.py
│       
└───ui
        chat_view.py
        import_view.py
        schema_view.py
        sidebar.py
