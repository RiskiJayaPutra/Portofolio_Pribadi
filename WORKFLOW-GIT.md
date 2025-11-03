# 📚 Dokumentasi Workflow Git - Portofolio Pribadi

## 🎯 Ringkasan

Dokumen ini menjelaskan langkah-langkah workflow Git yang telah dilakukan untuk project website portofolio pribadi.

---

## 🔄 Langkah-Langkah Workflow Git

### 1️⃣ Inisialisasi Git Repository

```bash
cd "d:\Data_Kuliah\Semester_5\PPW\Judul 2"
git init
git config user.name "RiskiJayaPutra"
git config user.email "rizkijayaputra2005@gmail.com"
```

**Hasil**: Repository Git berhasil diinisialisasi dengan konfigurasi user yang sesuai.

---

### 2️⃣ Commit Bertahap untuk Setiap Section

#### Commit 1: File .gitignore
```bash
git add .gitignore
git commit -m "Inisialisasi: Tambah file .gitignore"
```

#### Commit 2: Aset Gambar
```bash
git add assets/
git commit -m "Tambah aset gambar: Foto profil dan sertifikat"
```

#### Commit 3: Styling Dasar
```bash
git add style.css
git commit -m "Tambah styling dasar: Reset CSS dan konfigurasi font"
```

#### Commit 4: Struktur HTML
```bash
git add index.html
git commit -m "Tambah struktur HTML: Navigasi, Hero section, dan About Me"
```

#### Commit 5: Screenshot
```bash
git add image.png
git commit -m "Tambah screenshot tampilan website"
```

**Hasil**: Setiap komponen website di-commit secara terpisah untuk tracking yang lebih baik.

---

### 3️⃣ Buat Branch untuk Eksperimen Styling

```bash
git checkout -b styling-eksperimen
```

**Hasil**: Branch baru `styling-eksperimen` berhasil dibuat untuk eksperimen perubahan styling.

---

### 4️⃣ Eksperimen Styling di Branch Baru

#### Eksperimen 1: Gradien Background
```bash
# Ubah background dari solid color menjadi gradient
git add style.css
git commit -m "Eksperimen: Perbaiki gradien background dan section title"
```

#### Eksperimen 2: Efek Hover Navigasi
```bash
# Tingkatkan efek hover dengan animasi dan shadow
git add style.css
git commit -m "Eksperimen: Tingkatkan efek hover navigasi dengan animasi"
```

#### Eksperimen 3: Finalisasi
```bash
git add style.css
git commit -m "Eksperimen: Finalisasi perubahan styling"
```

**Hasil**: 3 commit eksperimen styling berhasil dibuat di branch `styling-eksperimen`.

---

### 5️⃣ Merge Branch ke Main

```bash
# Kembali ke branch main
git checkout main

# Merge branch styling-eksperimen
git merge styling-eksperimen -m "Merge: Gabungkan styling eksperimen ke main"
```

**Hasil**: Perubahan styling dari branch `styling-eksperimen` berhasil digabungkan ke branch `main`.

---

### 6️⃣ Buat README.md yang Informatif

```bash
git add README.md
git commit -m "Dokumentasi: Buat README.md yang informatif dan lengkap"
```

**Hasil**: README.md lengkap dengan deskripsi project, cara instalasi, dan informasi kontak.

---

### 7️⃣ Push ke GitHub

```bash
# Tambahkan remote repository
git remote add origin https://github.com/RiskiJayaPutra/Portofolio_Pribadi.git

# Pastikan branch utama bernama main
git branch -M main

# Push branch main
git push -u origin main

# Push branch styling-eksperimen
git push origin styling-eksperimen
```

**Hasil**: Semua commit berhasil di-push ke repository GitHub.

---

## 📊 Visualisasi Git Log

```
* aae2ee3 (HEAD -> main, origin/main) Dokumentasi: Buat README.md yang informatif dan lengkap
* 1321ab6 (origin/styling-eksperimen, styling-eksperimen) Eksperimen: Finalisasi perubahan styling
* de89627 Eksperimen: Tingkatkan efek hover navigasi dengan animasi
* 136a6ab Eksperimen: Perbaiki gradien background dan section title
* c4f4adc Tambah screenshot tampilan website
* b8e6909 Tambah struktur HTML: Navigasi, Hero section, dan About Me
* 2c67ff5 Tambah styling dasar: Reset CSS dan konfigurasi font
* 4537791 Tambah aset gambar: Foto profil dan sertifikat
* 38673f5 Inisialisasi: Tambah file .gitignore
```

---

## 🎓 Pelajaran yang Dipetik

### ✅ Best Practices yang Diterapkan:

1. **Commit Message yang Jelas**: Setiap commit memiliki pesan yang deskriptif
2. **Commit Atomik**: Setiap commit fokus pada satu perubahan spesifik
3. **Branching Strategy**: Menggunakan branch terpisah untuk eksperimen
4. **Dokumentasi Lengkap**: README.md yang informatif dan komprehensif
5. **Version Control**: Tracking perubahan dengan sistematis

### 📌 Struktur Commit Message:

Format: `[Kategori]: [Deskripsi singkat]`

Kategori yang digunakan:
- **Inisialisasi**: Setup awal project
- **Tambah**: Menambahkan file atau fitur baru
- **Eksperimen**: Percobaan styling atau fitur
- **Merge**: Menggabungkan branch
- **Dokumentasi**: Perubahan pada dokumentasi

---

## 🔗 Repository Information

- **Repository URL**: https://github.com/RiskiJayaPutra/Portofolio_Pribadi.git
- **Branch Utama**: main
- **Branch Eksperimen**: styling-eksperimen
- **Total Commits**: 9 commits
- **Contributors**: RiskiJayaPutra

---

## 📝 Catatan Tambahan

### File yang Telah Di-commit:
- ✅ .gitignore
- ✅ assets/ (6 gambar)
- ✅ style.css
- ✅ index.html
- ✅ image.png
- ✅ README.md

### Branch yang Ada:
- ✅ main (branch utama)
- ✅ styling-eksperimen (branch eksperimen)

---

**Dibuat oleh**: Riski Jaya Putra  
**Tanggal**: November 2024  
**Untuk**: Tugas Akhir Praktikum Pemrograman Web
