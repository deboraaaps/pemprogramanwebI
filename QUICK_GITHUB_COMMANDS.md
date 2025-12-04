# ⚡ Quick Reference: Update GitHub

Cheat sheet cepat untuk update/push ke GitHub. Copy-paste siap pakai!

---

## 🚀 PUSH PERUBAHAN (5 Langkah Cepat)

```bash
# 1. Lihat file yang berubah
git status

# 2. Stage file
git add .

# 3. Commit dengan pesan
git commit -m "feat: deskripsi perubahan"

# 4. Pull (untuk sync)
git pull origin main

# 5. Push ke GitHub
git push origin main

# ✅ SELESAI!
```

---

## 📝 Commit Message Format

```
<type>: <subject>

<body>

<footer>
```

**Types:**
- `feat:` - Feature baru
- `fix:` - Bug fix
- `docs:` - Dokumentasi
- `style:` - Format code
- `refactor:` - Refactor
- `perf:` - Performance
- `test:` - Testing

**Contoh:**
```
feat: add dark mode untuk website

- Implement toggle button
- Add CSS variables
- Update documentation

Closes #123
```

---

## 🔄 UPDATE dari GitHub (Sync)

```bash
# Jika orang lain sudah update repository:

# Pull latest changes
git pull origin main

# Atau jika ada conflict:
git fetch origin
git merge origin/main
# ... resolve conflict ...
git push origin main
```

---

## 🌳 Bekerja dengan Branch

```bash
# Buat branch baru
git checkout -b feature/nama-fitur

# ... edit files ...

# Push branch ke GitHub
git push origin feature/nama-fitur

# Setelah merge ke main, hapus branch
git branch -d feature/nama-fitur
git push origin --delete feature/nama-fitur
```

---

## 🛠️ Useful Commands

```bash
# Lihat apa yang akan di-push
git log origin/main..HEAD
git diff origin/main

# Lihat history commits
git log --oneline -10

# Lihat branches
git branch -a

# Unstage file
git reset HEAD filename

# Discard changes
git checkout -- filename

# Undo last commit (belum push)
git reset --soft HEAD~1

# Undo last commit (sudah push)
git revert HEAD
git push origin main
```

---

## ⚠️ Troubleshooting

```bash
# Error: "Permission denied (publickey)"
# → Setup SSH key atau gunakan HTTPS + token

# Error: "Everything up-to-date"
# → Tidak ada changes untuk di-push
# → Check: git status

# Error: "CONFLICT merging"
# → Edit file, hapus markers, git add, git commit, git push

# Error: "Your branch is behind"
# → git pull origin main
# → git push origin main

# Error: "fatal: not a git repository"
# → git init (atau clone repository)
```

---

## 📋 Workflow Standar Per Hari

```bash
# 🌅 PAGI: Start kerja
git pull origin main

# 💻 TENGAH HARI: Save progress
git add .
git commit -m "feat: fitur X sedang dikerjakan"
git push origin main

# 🌆 SORE: Fitur selesai
git add .
git commit -m "feat: complete fitur X"
git push origin main

# 🌙 MALAM: Sebelum tidur
git pull origin main  # Sync dengan rekan
git status  # Verifikasi
```

---

## 🔐 Setup Pertama Kali

```bash
# Install Git
# Windows: https://git-scm.com/download/win
# macOS: brew install git
# Linux: sudo apt-get install git

# Configure
git config --global user.name "Nama Anda"
git config --global user.email "email@example.com"

# Clone repository
git clone https://github.com/deboraaaps/pemprogramanwebI.git
cd pemprogramanwebI

# Verify
git remote -v
```

---

## 💾 One-Liner Commands

```bash
# Stage + commit + push sekaligus (hanya untuk file yang sudah tracked)
git commit -am "pesan" && git push origin main

# Update + push sekaligus
git pull origin main && git push origin main

# Lihat status dalam 1 baris
git status && git log --oneline -5

# Setup tracking untuk new branch
git push -u origin feature/nama
```

---

## 📱 Emergency Commands

```bash
# Jika push failed karena belum pull:
git pull origin main --rebase
git push origin main

# Jika ingin revert last commit (belum push):
git reset --hard HEAD~1

# Jika push dengan --force (HATI-HATI!):
git push origin main --force

# Jika butuh undo push (sudah push):
git revert HEAD
git push origin main
```

---

## 🎯 Scenarios

### Scenario 1: Simple edit & push
```bash
nano README.md
git add README.md
git commit -m "docs: update README"
git push origin main
```

### Scenario 2: Multiple files
```bash
nano file1.html
nano file2.css
nano file3.js
git add .
git commit -m "feat: implement new feature"
git push origin main
```

### Scenario 3: Create branch untuk fitur besar
```bash
git checkout -b feature/redesign
# ... work for days ...
git push origin feature/redesign
# Create PR di GitHub, merge, delete branch
```

---

## ✅ Checklist Sebelum Push

- [ ] Sudah `git status` untuk lihat changes?
- [ ] Semua file yang mau di-push sudah di-add?
- [ ] Commit message ditulis dengan baik?
- [ ] Sudah `git pull` sebelum push?
- [ ] Tidak ada conflict?

Jika semua OK → `git push origin main` ✅

---

## 🔗 Links

- [Full Guide](./PANDUAN_UPDATE_GITHUB.md)
- [GitHub Help](https://docs.github.com)
- [Git Docs](https://git-scm.com/doc)

---

<div align="center">

**Butuh bantuan? Baca PANDUAN_UPDATE_GITHUB.md untuk penjelasan lengkap!**

Quick Commands Saved Successfully! ⚡

</div>

---

*Last Updated: Desember 2025*
