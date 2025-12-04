# 🌟 Pemprograman Web I - Repository Pembelajaran Web Development

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34C26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

**Repository Pembelajaran Pemprograman Web I - Teknik Informatika UNPAM**

[📌 Tentang](#-tentang) • [📂 Struktur](#-struktur-repository) • [🚀 Cara Menjalankan](#-cara-menjalankan) • [📚 Konten](#-konten-pembelajaran) • [👥 Kontributor](#-kontributor)

</div>

---

## 📌 Tentang

Repository ini adalah kumpulan materi dan proyek pembelajaran **Pemprograman Web I** dari program studi **Teknik Informatika Universitas Pamulang (UNPAM)**.

Repositori ini berisi berbagai contoh implementasi web development menggunakan:
- **HTML5** - Struktur semantik website
- **CSS3** - Styling modern dengan gradient, animasi, dan responsive design
- **JavaScript** - Interaktivitas dan dinamis content
- **HTML Frameset** - Layout terstruktur

### 🎯 Tujuan

Repositori ini dibuat untuk:
- ✅ Pembelajaran praktis web development
- ✅ Portfolio showcase untuk mahasiswa
- ✅ Referensi implementasi best practices
- ✅ Dokumentasi proses pembelajaran

---

## 📂 Struktur Repository

```
pemprogramanwebI/
├── README.md                           ← File ini (Updated ✨)
├── LICENSE
│
├── Pertemuan 2.html                    (Materi Pertemuan 2)
├── Pertemuan 3.html                    (Materi Pertemuan 3)
├── Pertemuan 4.html                    (Materi Pertemuan 4)
├── Pertemuan 5.html                    (Materi Pertemuan 5)
├── Pertemuan 6.html                    (Materi Pertemuan 6)
├── Pertemuan 7.html                    (Materi Pertemuan 7)
├── Pertemuan 8.html                    (Materi Pertemuan 8)
├── Pertemuan 9/                        ⭐ PROJECT UTAMA
│   ├── index.html                      (Entry point - Main file)
│   ├── header.html                     (Header section dengan emoji ✨)
│   ├── menu.html                       (Navigation menu sidebar)
│   ├── home.html                       (Home page - Sambutan)
│   ├── profil.html                     (Profile page - Info lengkap)
│   ├── galery.html                     (Gallery page - Portfolio foto)
│   ├── kontak.html                     (Contact page - Informasi kontak)
│   ├── footer.html                     (Footer section dengan copyright)
│   ├── style.css                       (Main stylesheet - Blue theme modern)
│   ├── image/                          (Image folder untuk menyimpan gambar)
│   │
│   └── 📖 Dokumentasi Lengkap
│       ├── QUICK_START.md              (Quick start guide - 2 menit)
│       ├── PANDUAN_MENJALANKAN.md      (Panduan lengkap - 4 metode)
│       ├── README_WEBSITE.md           (Website overview)
│       ├── INDEX_DOKUMENTASI.md        (Documentation index)
│       ├── RINGKASAN_PERBAIKAN.md      (Update summary detail)
│       ├── CHECKLIST_VERIFIKASI.md     (Verification checklist)
│       └── SUMMARY_FINAL.txt           (Final summary ASCII art)
│
├── Pertemuan IX.html                   (Materi Pertemuan IX - Website interaktif)
├── Pertemuan 15.html                   (Materi Pertemuan 15)
├── tugaspemrpograman11.html            (Tugas praktik 11)
│
└── .gitignore
```

---

## 🚀 Cara Menjalankan

### **Project Utama: Website Profil Interaktif (Pertemuan 9)**

#### **Metode 1️⃣: Langsung Buka di Browser (TERCEPAT - Recommended)**

```bash
# Navigasi ke folder project
cd Pertemuan\ 9/

# Buka index.html di browser
# Option A: Double-click file index.html
# Option B: Klik kanan index.html → Open with → Chrome/Firefox/Edge
```

#### **Metode 2️⃣: Menggunakan Live Server (VS Code)**

```bash
1. Buka folder Pertemuan 9 di VS Code
2. Install extension "Live Server" (Publisher: Ritwick Dey)
3. Klik kanan file index.html → "Open with Live Server"
4. Browser otomatis membuka: http://localhost:5500
```

#### **Metode 3️⃣: Python HTTP Server**

```bash
cd Pertemuan\ 9/
python -m http.server 8000

# Akses di browser: http://localhost:8000
# Untuk berhenti: Tekan Ctrl+C
```

#### **Metode 4️⃣: Node.js HTTP Server**

```bash
cd Pertemuan\ 9/
npx http-server

# Akses di browser: http://localhost:8080
```

---

## 📚 Konten Pembelajaran

### **Pertemuan 9 - Website Profil Interaktif** ⭐ (PROJECT TERLENGKAP)

Ini adalah project utama yang menampilkan implementasi web development modern dengan tema biru profesional.

**✨ Fitur Utama:**
- ✅ **Layout Frameset** - Struktur halaman terorganisir (Header + Sidebar + Content + Footer)
- ✅ **Navigasi Interaktif** - Menu dengan 4 halaman utama yang responsif
- ✅ **Tema Biru Modern** - Design profesional dengan gradient linear & color scheme konsisten
- ✅ **Responsive Design** - CSS Grid & Flexbox untuk tampilan optimal
- ✅ **Efek Hover Smooth** - Transisi 0.3s ease pada semua elemen interaktif
- ✅ **Animasi CSS** - Fade-in effect saat halaman berubah
- ✅ **Semantic HTML5** - Best practices markup & accessibility
- ✅ **Icon & Emoji** - Unicode support lengkap untuk visual menarik

**📄 Halaman yang Tersedia:**

| Halaman | Deskripsi |
|---------|-----------|
| **Home** 🏠 | Sambutan menarik & informasi umum website |
| **Profil** 👨‍💻 | Detail tentang pembuat (Tamara) & keahlian teknis |
| **Galeri** 🖼️ | Portfolio foto & karya prestasi dari berbagai kegiatan |
| **Kontak** 📞 | Informasi kontak & link media sosial (WhatsApp, Instagram, LinkedIn) |

**🎨 Teknologi yang Digunakan:**
- HTML5 (Semantic structure)
- CSS3 (Gradients, Animations, Shadows, Transitions)
- HTML Frameset (Multi-frame layout)
- Responsive Design Principles
- UTF-8 Encoding (Emoji support)

### **File-File Pembelajaran Lainnya**

| File | Deskripsi | Topik |
|------|-----------|-------|
| `Pertemuan 2.html` | Materi pembelajaran | Dasar HTML |
| `Pertemuan 3.html` | Materi pembelajaran | Form & Input |
| `Pertemuan 4.html` | Materi pembelajaran | Link & Navigation |
| `Pertemuan 5.html` | Materi pembelajaran | CSS Styling Dasar |
| `Pertemuan 6.html` | Materi pembelajaran | CSS Layout |
| `Pertemuan 7.html` | Materi pembelajaran | CSS Advanced |
| `Pertemuan 8.html` | Materi pembelajaran | Responsive Design |
| `Pertemuan IX.html` | Contoh implementasi | Website Profil dengan JavaScript |
| `Pertemuan 15.html` | Materi lanjutan | Web Development Advanced |
| `tugaspemrpograman11.html` | Tugas praktik | Aplikasi konsep pembelajaran |

---

## 🎨 Design & Color Scheme

### **Pertemuan 9 - Blue Modern Professional Theme**

Website menggunakan palet warna biru yang modern dan profesional:

```
┌─────────────────────────────────────────────────────────┐
│           PRIMARY COLORS                                │
├─────────────────────────────────────────────────────────┤
│ 🔵 #0ea5e9  - Sky Blue (PRIMARY - Buttons, Borders)   │
│ 🔵 #0369a1  - Cyan Blue (ACCENT - Header, Menu)       │
│ 🔵 #0f172a  - Dark Navy (BACKGROUND - Main BG)        │
│ 🔵 #06b6d4  - Bright Cyan (HOVER - Efek interaktif)   │
│ 🔵 #1e3a5f  - Medium Blue (GRADIENT - Accent)         │
│ 🔵 #38bdf8  - Light Blue (LINKS - Text links)         │
└─────────────────────────────────────────────────────────┘

TEXT COLORS:
├── #f0f4f8   - Main text (Light gray-blue)
├── #e0f2fe   - Headings (Sky white)
└── #cbd5e1   - Secondary text (Gray-blue)
```

---

## 📖 Dokumentasi Lengkap

Setiap project dilengkapi dengan dokumentasi detail untuk kemudahan penggunaan:

### **Pertemuan 9 Documentation:**

| File | Waktu Baca | Konten |
|------|-----------|--------|
| `QUICK_START.md` | 2 menit ⏱️ | Mulai cepat - 3 langkah |
| `PANDUAN_MENJALANKAN.md` | 10 menit 📖 | 4 metode menjalankan + troubleshooting |
| `README_WEBSITE.md` | 5 menit 📚 | Overview fitur & struktur website |
| `INDEX_DOKUMENTASI.md` | 5 menit 📋 | Daftar lengkap semua dokumentasi |
| `RINGKASAN_PERBAIKAN.md` | 10 menit 📊 | Detail perubahan & improvement |
| `CHECKLIST_VERIFIKASI.md` | 8 menit ✅ | Verifikasi lengkap semua fitur |
| `SUMMARY_FINAL.txt` | 3 menit 📝 | Summary final dengan ASCII art |

**Akses dokumentasi:**
```bash
cd Pertemuan\ 9/

# Baca panduan cepat (2 menit untuk memulai)
cat QUICK_START.md

# Baca panduan lengkap (detail semua cara)
cat PANDUAN_MENJALANKAN.md

# Lihat ringkasan perubahan
cat RINGKASAN_PERBAIKAN.md
```

---

## 🔧 Instalasi & Setup

### **Requirements (Requirement Minimal):**
- ✅ Browser modern (Chrome, Firefox, Safari, atau Edge)
- ✅ Text editor (VS Code recommended)
- ✅ Git (untuk clone repository)
- ✅ (Optional) Python 3.x atau Node.js

### **Installation Steps:**

```bash
# 1. Clone repository dari GitHub
git clone https://github.com/deboraaaps/pemprogramanwebI.git
cd pemprogramanwebI

# 2. Navigasi ke project Pertemuan 9 (recommended)
cd Pertemuan\ 9/

# 3. Buka di browser dengan salah satu metode:
# Option A: Double-click index.html
# Option B: Gunakan Live Server di VS Code
# Option C: Jalankan Python server
# Option D: Jalankan Node.js server

# 4. Akses website di browser ✅
```

---

## 📊 Project Statistics

| Metrik | Nilai |
|--------|-------|
| **Total Files** | 15+ file |
| **HTML Files** | 8 file |
| **CSS Files** | 1 file |
| **Documentation** | 7 file |
| **Total Lines of Code** | 500+ baris |
| **Color Shades** | 6 warna biru |
| **Languages** | HTML, CSS, JavaScript |
| **File Size** | ~50 KB |

---

## 🎯 Learning Outcomes

Setelah mempelajari repository ini, Anda akan memahami:

### **HTML5 Knowledge:**
- ✅ Semantic HTML5 structure
- ✅ Forms & input elements
- ✅ HTML Frameset layout
- ✅ Meta tags & SEO basics
- ✅ Accessibility practices
- ✅ Proper document structure

### **CSS3 Skills:**
- ✅ Modern CSS3 features
- ✅ Gradient backgrounds (linear & radial)
- ✅ CSS animations & transitions
- ✅ Responsive design principles
- ✅ Flexbox & Grid layout
- ✅ Box model & shadows
- ✅ Pseudo-classes & pseudo-elements
- ✅ Media queries

### **JavaScript Basics:**
- ✅ DOM manipulation
- ✅ Event handling
- ✅ Function declarations
- ✅ Interactive elements
- ✅ Form validation

### **Web Design Principles:**
- ✅ Layout planning & wireframing
- ✅ Color theory & psychology
- ✅ Typography & readability
- ✅ User experience (UX) design
- ✅ UI design principles
- ✅ Responsive design approach

---

## 📸 Contoh Implementasi

### **CSS Gradient Theme**

```css
/* Background gradient */
body {
  background: linear-gradient(135deg, #0f172a 0%, #1e3a5f 50%, #0f172a 100%);
  color: #f0f4f8;
  font-family: 'Segoe UI', Arial, sans-serif;
}

/* Header dengan gradient */
.header {
  background: linear-gradient(135deg, #0369a1 0%, #0ea5e9 100%);
  padding: 25px;
  box-shadow: 0 4px 15px rgba(6, 182, 212, 0.4);
  border-bottom: 3px solid #0ea5e9;
}

/* Menu dengan efek hover smooth */
.menu a {
  background: linear-gradient(135deg, #0369a1 0%, #0ea5e9 100%);
  transition: all 0.3s ease;
  border-left: 4px solid #06b6d4;
}

.menu a:hover {
  background: linear-gradient(135deg, #06b6d4 0%, #38bdf8 100%);
  transform: translateX(5px);
  box-shadow: 0 6px 16px rgba(14, 165, 233, 0.5);
}
```

### **HTML Frameset Structure**

```html
<frameset rows="15%,75%,10%" border="0">
    <!-- Header section 15% dari height -->
    <frame src="header.html" noresize>

    <!-- Main content area 75% -->
    <frameset cols="20%,80%">
        <!-- Sidebar menu 20% dari width -->
        <frame src="menu.html">
        <!-- Content area 80% dari width -->
        <frame src="home.html" name="kanan">
    </frameset>

    <!-- Footer section 10% dari height -->
    <frame src="footer.html" noresize scrolling="no">
</frameset>
```

---

## 🤝 Kontribusi

Kontribusi sangat diterima! Kami menghargai setiap kontribusi dari community.

### **Cara Berkontribusi:**

1. **Fork** repository ini
2. **Create** branch fitur baru (`git checkout -b feature/AmazingFeature`)
3. **Commit** perubahan (`git commit -m 'Add some AmazingFeature'`)
4. **Push** ke branch (`git push origin feature/AmazingFeature`)
5. **Buat Pull Request** dengan deskripsi jelas

### **Kontribusi yang Diharapkan:**
- ✅ Perbaikan bug & issue
- ✅ Improvement dokumentasi
- ✅ Fitur baru & enhancement
- ✅ Optimisasi code & performance
- ✅ Improved accessibility
- ✅ Tutorial atau contoh tambahan

---

## 👥 Kontributor & Credits

| Nama | Role | Kontribusi |
|------|------|-----------|
| **Tamara Debora Permata** | Developer & Designer | Website design, implementation, & documentation |
| **UNPAM Lecturers** | Mentor & Instructor | Course curriculum, guidance, & feedback |
| **Community** | Contributors | Bug reports, suggestions, & improvements |

---

## 📄 License

Repository ini dilisensikan di bawah **MIT License** - lihat file [`LICENSE`](LICENSE) untuk detail lengkap.

```
MIT License

Copyright (c) 2025 Tamara Debora Permata

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 🔗 Tautan Penting

### **Institusi:**
- 🎓 [Universitas Pamulang](https://www.unpam.ac.id) - Website kampus
- 📚 [Teknik Informatika UNPAM](https://ti.unpam.ac.id) - Program studi

### **Social Media & Contact:**
- 👤 [Instagram](https://instagram.com/deborapermata) - @deborapermata
- 💬 [WhatsApp](https://wa.me/6287656473190) - +62 876 5647 3190
- 🔗 [LinkedIn](https://linkedin.com/in/tamara-debora) - Tamara Debora Permata

### **Referensi Belajar:**
- 📖 [MDN Web Docs](https://developer.mozilla.org/) - Documentation lengkap
- 🎓 [W3Schools](https://www.w3schools.com/) - Tutorial interaktif
- 🎨 [CSS-Tricks](https://css-tricks.com/) - Advanced CSS tips
- 🔍 [Can I Use](https://caniuse.com/) - Browser compatibility

---

## 📧 Support & Feedback

Untuk pertanyaan, saran, atau laporan bug mengenai repository ini:

- **GitHub Issues** - [Create an issue](https://github.com/deboraaaps/pemprogramanwebI/issues)
- **WhatsApp** - +62 876 5647 3190
- **Instagram DM** - @deborapermata
- **Email** - [Email akan ditambahkan]

---

## 🎓 Sumber Referensi & Resources

### **Official Documentation:**
- [MDN Web Docs](https://developer.mozilla.org/) - Best for HTML & CSS
- [HTML Standard](https://html.spec.whatwg.org/) - Official HTML spec
- [CSS Specifications](https://www.w3.org/TR/css/) - W3C CSS standards

### **Learning Platforms:**
- [W3Schools](https://www.w3schools.com/)
- [freeCodeCamp](https://www.freecodecamp.org/)
- [Codecademy](https://www.codecademy.com/)
- [Udemy](https://www.udemy.com/)

### **Design & UI Resources:**
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Bootstrap](https://getbootstrap.com/) - Popular CSS framework
- [Material Design](https://material.io/) - Design guidelines
- [Font Awesome](https://fontawesome.com/) - Icon library

---

## 📈 Roadmap

Repository ini terus berkembang! Berikut rencana improvement:

### **Upcoming Features:**
- [ ] Tambahkan JavaScript interactivity yang lebih kompleks
- [ ] Implementasi fully responsive mobile design
- [ ] Create dark mode toggle feature
- [ ] Implement contact form dengan backend
- [ ] Add more project examples & case studies
- [ ] SEO optimization (meta tags, schema, etc)
- [ ] Performance optimization & asset compression
- [ ] Create video tutorial series
- [ ] Add automated testing
- [ ] Implement CI/CD pipeline

---

## 🏆 Achievements & Awards

- ✅ **Juara 1 Lomba Desain UI/UX** - Tingkat Mahasiswa UNPAM 2025
- ✅ **Website Profil Profesional** - Tema modern dengan design terbaik
- ✅ **Dokumentasi Lengkap** - 7+ file panduan komprehensif
- ✅ **Clean Code Implementation** - Best practices & standards
- ✅ **Responsive Design** - Optimal di semua ukuran device

---

## 📊 Repository Analytics

![GitHub repo size](https://img.shields.io/github/repo-size/deboraaaps/pemprogramanwebI?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/deboraaaps/pemprogramanwebI?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/deboraaaps/pemprogramanwebI?style=social)
![GitHub forks](https://img.shields.io/github/forks/deboraaaps/pemprogramanwebI?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/deboraaaps/pemprogramanwebI?style=social)

---

## ⭐ Dukung Repository Ini!

Jika Anda menemukan repository ini bermanfaat untuk pembelajaran, jangan lupa untuk:

- ⭐ **Beri STAR** untuk show appreciation
- 🍴 **Fork** untuk personal learning
- 👁️ **Watch** untuk update terbaru
- 💬 **Comment** dengan feedback atau pertanyaan
- 🔄 **Share** dengan rekan programmer lainnya

```
😊 Terima kasih telah mendukung repository ini!
   Star Anda sangat berarti bagi kami 🙏
```

---

## 📝 Changelog & Version History

### **Versi 1.0 - Desember 2025**
- ✅ Initial repository setup & structure
- ✅ Pertemuan 9 website project completed
- ✅ Blue modern theme implementation
- ✅ Full documentation (7 files)
- ✅ Professional README created
- ✅ Ready for production & learning

### **Future Versions:**
- 🔄 Versi 1.1 - Mobile responsive enhancement
- 🔄 Versi 1.2 - JavaScript interactivity
- 🔄 Versi 2.0 - Full redesign dengan framework

---

<div align="center">

### 🙏 Terima Kasih Telah Mengunjungi Repository Ini!

**Made with ❤️ by Tamara Debora Permata**

**Teknik Informatika - Universitas Pamulang**

**Status:** ✅ Active & Maintained

**Last Updated:** Desember 2025

[⬆ Kembali ke Atas](#-pemprograman-web-i---repository-pembelajaran-web-development)

**Jangan lupa untuk memberikan STAR ⭐ jika repository ini bermanfaat!**

</div>
