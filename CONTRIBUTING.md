# 🤝 Panduan Berkontribusi

Terima kasih telah tertarik untuk berkontribusi pada repository **pemprogramanwebI**! 🎉

Panduan ini akan membantu Anda memahami cara berkontribusi dengan benar dan efektif.

---

## 📋 Daftar Isi

- [Kode Etik](#kode-etik)
- [Cara Memulai](#cara-memulai)
- [Proses Kontribusi](#proses-kontribusi)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Bug Report](#bug-report)
- [Feature Request](#feature-request)
- [Gaya Penulisan Code](#gaya-penulisan-code)

---

## 🎯 Kode Etik

Kami berkomitmen untuk menjaga komunitas yang ramah dan positif. Silakan:

- ✅ Gunakan bahasa yang sopan dan profesional
- ✅ Hormati pendapat dan saran dari kontributor lain
- ✅ Fokus pada improvement produk, bukan serangan personal
- ✅ Laporkan perilaku yang tidak pantas kepada maintainer

---

## 🚀 Cara Memulai

### 1. Fork Repository

```bash
# Kunjungi https://github.com/deboraaaps/pemprogramanwebI
# Klik tombol "Fork" di kanan atas
```

### 2. Clone Repository Hasil Fork

```bash
git clone https://github.com/username-anda/pemprogramanwebI.git
cd pemprogramanwebI
```

### 3. Tambah Remote Upstream

```bash
git remote add upstream https://github.com/deboraaaps/pemprogramanwebI.git
git remote -v  # Verifikasi
```

### 4. Buat Branch Baru

```bash
git checkout -b feature/nama-fitur
# atau
git checkout -b bugfix/nama-bug
# atau
git checkout -b docs/nama-dokumentasi
```

---

## 📝 Proses Kontribusi

### **Step 1: Buat Perubahan**

```bash
# Edit file yang ingin diubah
nano Pertemuan\ 9/style.css

# Atau buka dengan VS Code
code Pertemuan\ 9/
```

### **Step 2: Commit Perubahan**

```bash
# Stage files
git add .

# Commit dengan pesan yang jelas
git commit -m "feat: add new feature untuk website profil"
# atau
git commit -m "fix: perbaiki bug pada menu navigasi"
# atau
git commit -m "docs: update dokumentasi README"
```

**Format Commit Message:**
```
type(scope): deskripsi singkat

Deskripsi lebih detail (jika diperlukan)

- Point 1
- Point 2

Closes #123  (jika ada related issue)
```

**Types:**
- `feat:` - Fitur baru
- `fix:` - Bug fix
- `docs:` - Dokumentasi
- `style:` - Format code (tidak mengubah logic)
- `refactor:` - Refactor code
- `perf:` - Performance improvement
- `test:` - Testing
- `chore:` - Build tools, dependencies, dll

### **Step 3: Push ke Fork**

```bash
git push origin feature/nama-fitur
```

### **Step 4: Buat Pull Request**

1. Kunjungi repository di GitHub
2. Klik tombol "Compare & pull request"
3. Pastikan base branch adalah `main`
4. Isi deskripsi PR dengan jelas
5. Klik "Create pull request"

---

## 📋 Pull Request Guidelines

### **PR Title Format:**

```
[Type] Deskripsi singkat

Contoh:
[Feature] Tambah dark mode toggle
[Fix] Perbaiki responsive design di mobile
[Docs] Update installation guide
```

### **PR Description Template:**

```markdown
## 📝 Deskripsi
Penjelasan singkat tentang apa yang diubah dan mengapa.

## 🔄 Tipe Perubahan
- [ ] Bug fix (non-breaking change yang memperbaiki issue)
- [ ] Fitur baru (non-breaking change yang menambah fitur)
- [ ] Breaking change (perbaikan atau fitur yang mengubah existing functionality)
- [ ] Dokumentasi baru atau update

## 🧪 Testing
Deskripsi cara testing perubahan:
- [ ] Test A dilakukan
- [ ] Test B dilakukan
- [ ] Verified di Chrome
- [ ] Verified di Firefox

## 📸 Screenshots (jika applicable)
Lampirkan screenshot atau GIF untuk UI changes

## 🔗 Related Issues
Closes #123

## ✅ Checklist
- [ ] Code mengikuti style guidelines repository ini
- [ ] Saya telah melakukan self-review
- [ ] Dokumentasi telah diupdate (jika applicable)
- [ ] Tidak ada breaking changes
```

---

## 🐛 Bug Report

### **Cara Melaporkan Bug:**

1. **Cek Issue Existing** - Pastikan bug belum dilaporkan
2. **Buat Issue Baru** dengan template berikut:

```markdown
## 📌 Deskripsi Bug
Penjelasan singkat tentang bug yang Anda temukan.

## 🔍 Steps to Reproduce
1. Buka file ...
2. Klik ...
3. Lihat hasil ...

## ✅ Expected Behavior
Apa yang seharusnya terjadi

## ❌ Actual Behavior
Apa yang sebenarnya terjadi

## 📸 Screenshots/Videos
Lampirkan jika membantu

## 💻 Environment
- OS: [e.g. Windows 10, macOS 12]
- Browser: [e.g. Chrome 96, Firefox 95]
- Node version: [jika applicable]

## 📝 Additional Context
Informasi tambahan yang relevan
```

---

## 💡 Feature Request

### **Cara Mengajukan Fitur Baru:**

1. **Cek Feature Requests Existing**
2. **Buat Issue Baru** dengan template:

```markdown
## 🎯 Feature Request
Penjelasan tentang fitur yang ingin ditambahkan

## 🤔 Alasan
Mengapa fitur ini diperlukan? Apa manfaatnya?

## 💡 Implementasi yang Disarankan
Bagaimana cara implementasi fitur ini?

## 📋 Alternative
Alternatif lain yang bisa dipertimbangkan?

## ✅ Checklist
- [ ] Feature ini tidak existing di repository
- [ ] Feature ini sesuai dengan scope repository
```

---

## 🎨 Gaya Penulisan Code

### **HTML Guidelines:**

```html
<!-- ✅ GOOD -->
<div class="profile-card">
  <h2>Nama Lengkap</h2>
  <p>Deskripsi singkat</p>
</div>

<!-- ❌ BAD -->
<div class="card">
  <h2>Nama Lengkap</h2><p>Deskripsi singkat</p>
</div>
```

### **CSS Guidelines:**

```css
/* ✅ GOOD */
.profile-card {
  background: linear-gradient(135deg, #0369a1 0%, #0ea5e9 100%);
  padding: 20px;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.profile-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 30px rgba(14, 165, 233, 0.4);
}

/* ❌ BAD */
.pc{background:#0369a1;padding:20px;}
.pc:hover{transform:translateY(-5px)}
```

### **JavaScript Guidelines:**

```javascript
// ✅ GOOD
function showNavigation(id) {
  document.querySelectorAll("section").forEach(section => {
    section.classList.remove("active");
  });
  document.getElementById(id).classList.add("active");
}

// ❌ BAD
function show(id){
 document.querySelectorAll("section").forEach(s=>s.classList.remove("active"));
 document.getElementById(id).classList.add("active");
}
```

### **Dokumentasi Guidelines:**

```markdown
/* ✅ GOOD */
/**
 * Menampilkan halaman yang dipilih
 * @param {string} id - ID halaman yang ingin ditampilkan
 */
function show(id) { ... }

/* ❌ BAD */
// show function
function show(id) { ... }
```

---

## 🔍 Proses Review

Setelah Anda membuat PR, tim maintainer akan:

1. **Review Code** - Memeriksa kualitas dan style
2. **Test Changes** - Menjalankan testing
3. **Provide Feedback** - Memberikan saran atau request changes
4. **Merge atau Close** - Merge jika approved atau close jika tidak sesuai

---

## 📚 Referensi

### **Dokumentasi:**
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Flow](https://guides.github.com/introduction/flow/)
- [Semantic Commit](https://www.conventionalcommits.org/)

### **Code Style:**
- [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
- [MDN Web Docs](https://developer.mozilla.org/)
- [W3C Standards](https://www.w3.org/)

---

## 🎁 Rewards & Recognition

Kami menghargai setiap kontribusi! Kontributor aktif akan:

- ✅ Ditampilkan di bagian Contributors
- ✅ Mendapat attribution di dokumentasi
- ✅ Mendapat badge "Contributor" di repository
- ✅ Diundang sebagai collaborator (jika kontribusi signifikan)

---

## ❓ Pertanyaan?

Jika ada pertanyaan tentang proses kontribusi:

- 💬 [Diskusi di GitHub](https://github.com/deboraaaps/pemprogramanwebI/discussions)
- 📧 Email: [Akan ditambahkan]
- 💬 WhatsApp: +62 876 5647 3190
- 📸 Instagram DM: @deborapermata

---

## 🙏 Terima Kasih!

Kami sangat menghargai kontribusi Anda yang membantu membuat repository ini lebih baik! 

**Happy Contributing! 🚀**

---

*Last Updated: Desember 2025*
