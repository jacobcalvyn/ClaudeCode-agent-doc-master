# Doc-Master Agent untuk Claude Code CLI

## 📋 Deskripsi
Doc-Master adalah custom agent untuk Claude Code CLI yang dirancang khusus untuk menghasilkan dokumentasi project secara otomatis dalam Bahasa Indonesia. Agent ini akan membuat 4 file dokumentasi komprehensif yang membantu AI memahami struktur dan logika project Anda.

## 🚀 Cara Instalasi Doc-Master Agent

### Langkah-langkah:

#### 1. Buka Claude Code CLI dan jalankan command:
```bash
/agents
```

#### 2. Pilih opsi:
```
Create new agent
```

#### 3. Step 1: Choose location
Pilih:
```
Project (.claude/agents/)
```

#### 4. Step 2: Creation method
Pilih:
```
Manual configuration
```

#### 5. Step 3: Agent type (identifier)
Masukkan:
```
doc-master
```

#### 6. Step 4: System prompt
Copy **SEMUA ISI** dari file `system-prompt.md` dan paste di sini.

#### 7. Step 5: Description
Copy **SEMUA ISI** dari file `description.md` dan paste di sini.

#### 8. Step 6: Select tools
Pilih tools yang diperlukan untuk Doc-Master:
- ✅ Read
- ✅ Write
- ✅ Edit
- ✅ MultiEdit
- ✅ LS
- ✅ Glob
- ✅ Grep
- ✅ Task (opsional untuk analisis kompleks)

#### 9. Step 7: Select model
Rekomendasi:
```
claude-3-5-sonnet (atau model terbaru)
```

#### 10. Step 8: Choose background color
Pilih warna sesuai preferensi Anda

#### 11. Final step: Confirm and save
Review semua konfigurasi dan tekan Enter untuk menyimpan.

## 📖 Cara Penggunaan Doc-Master

Setelah agent terinstall, Anda bisa menggunakan Doc-Master dengan beberapa cara:

### 1. Trigger Otomatis
Cukup ketik salah satu keyword berikut:
- "buat dokumentasi project"
- "dokumentasi project saya"
- "generate API documentation"
- "update dokumentasi"
- "dokumentasi arsitektur"

### 2. Command Spesifik
```bash
# Generate dokumentasi awal
/doc-master init

# Update dokumentasi setelah perubahan code
/doc-master update

# Refresh seluruh dokumentasi
/doc-master refresh

# Validasi kualitas dokumentasi
/doc-master validate
```

## 📁 Output Dokumentasi

Doc-Master akan menghasilkan 4 file di root directory project Anda:

1. **PROJECT_STRUCTURE.md** - Arsitektur, tech stack, struktur folder
2. **API_DOCUMENTATION.md** - Dokumentasi komponen, fungsi, endpoint
3. **LOGIC_FLOW.md** - Alur bisnis, user journey, data flow
4. **AI_GUIDE.md** - Panduan development, coding standards, troubleshooting

## 🎯 Fitur Utama

- ✨ **100% Bahasa Indonesia** - Semua dokumentasi dalam Bahasa Indonesia
- 🤖 **AI-Optimized** - Dioptimalkan untuk pemahaman AI
- 🔍 **Auto-Detection** - Mendeteksi tech stack secara otomatis
- 🌐 **Multi-Stack Support** - Mendukung React, Vue, Node.js, Django, dll
- 📊 **Business Domain Aware** - E-commerce, SaaS, FinTech, dll
- 🔄 **Smart Update** - Update incremental tanpa menghapus customization

## 💡 Tips Penggunaan

1. **Project Baru**: Gunakan `/doc-master init` setelah setup awal project
2. **Setelah Refactoring**: Jalankan `/doc-master refresh` untuk update menyeluruh
3. **Development Rutin**: Gunakan `/doc-master update` setelah menambah fitur
4. **Code Review**: Jalankan `/doc-master validate` sebelum PR/merge

## 🛠️ Troubleshooting

Jika agent tidak berfungsi:
1. Pastikan semua tools yang diperlukan sudah dipilih saat setup
2. Cek apakah system prompt dan description ter-copy dengan lengkap
3. Gunakan model Sonnet atau yang lebih baru untuk hasil optimal

## 📝 Catatan

- Doc-Master akan selalu menyimpan file di root directory project
- File dokumentasi lama akan di-backup sebelum refresh
- Customization manual akan dipertahankan saat update

---

Made with ❤️ for Indonesian developers