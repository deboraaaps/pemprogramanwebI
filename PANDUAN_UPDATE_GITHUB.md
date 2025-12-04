# 📚 Panduan Lengkap: Cara Update di GitHub

Panduan ini menjelaskan berbagai cara untuk update/push perubahan ke GitHub repository.

---

## 📋 Daftar Isi

1. [Setup Awal](#setup-awal)
2. [Push Perubahan (Basic)](#push-perubahan-basic)
3. [Update dari Upstream](#update-dari-upstream)
4. [Cara Setiap Hari](#cara-setiap-hari)
5. [Troubleshooting](#troubleshooting)
6. [Best Practices](#best-practices)

---

## 🔧 Setup Awal

### **Langkah 1: Install Git**

**Windows:**
```bash
# Download dari https://git-scm.com/download/win
# Atau pakai Chocolatey
choco install git
```

**macOS:**
```bash
# Pakai Homebrew
brew install git
```

**Linux:**
```bash
# Ubuntu/Debian
sudo apt-get install git

# Fedora
sudo dnf install git
```

**Verifikasi:**
```bash
git --version  # Seharusnya muncul versi git
```

### **Langkah 2: Configure Git**

```bash
# Set nama Anda
git config --global user.name "Nama Anda"

# Set email Anda
git config --global user.email "email@example.com"

# Verifikasi
git config --list
```

### **Langkah 3: Clone Repository**

```bash
# Clone dari GitHub
git clone https://github.com/deboraaaps/pemprogramanwebI.git

# Masuk ke folder
cd pemprogramanwebI

# Lihat remote
git remote -v
```

---

## 📤 Push Perubahan (BASIC)

### **Metode 1: Push Perubahan Sederhana**

```bash
# ========== STEP 1: Lihat status ==========
git status

# Seharusnya muncul:
# On branch main
# Changes not staged for commit:
#   modified:   file.html
#   Untracked files:
#     newfile.md

# ========== STEP 2: Stage file ==========
# Option A: Stage satu file
git add filename.html

# Option B: Stage semua file
git add .

# Option C: Stage dengan interactive
git add -p

# ========== STEP 3: Commit ==========
git commit -m "feat: penambahan fitur baru"

# ========== STEP 4: Push ke GitHub ==========
git push origin main

# Done! ✅
```

### **Metode 2: Commit + Push Sekaligus (untuk file yang sudah tracked)**

```bash
# Stage dan commit sekaligus
git commit -am "docs: update dokumentasi"

# Push
git push origin main
```

### **Format Commit Message yang Baik**

```
feat: menambah fitur baru
fix: memperbaiki bug
docs: update dokumentasi
style: format code
refactor: reorganisasi code
perf: improvement performance
test: tambah testing
chore: update dependencies
```

**Contoh Lengkap:**

```
feat: add blue theme untuk website profil

- Tambahkan gradient background biru
- Update CSS dengan color scheme baru
- Add hover effects untuk menu
- Update dokumentasi

Closes #123
```

---

## 🔄 Update dari Upstream

### **Kasus: Repository di-update orang lain, Anda ingin sync**

```bash
# ========== LANGKAH 1: Fetch dari upstream ==========
git fetch origin

# ========== LANGKAH 2: Lihat perbedaan ==========
git log --oneline origin/main..HEAD  # Commit lokal
git log --oneline HEAD..origin/main  # Commit dari server

# ========== LANGKAH 3: Pull (update lokal) ==========
git pull origin main

# Jika ada conflict, resolve manual lalu:
git add .
git commit -m "Resolve merge conflict"
git push origin main
```

### **Jika Anda Fork Repository (Contribusi ke orang lain)**

```bash
# ========== Setup awal ==========
git clone https://github.com/USERNAME/pemprogramanwebI.git
cd pemprogramanwebI

# Tambah upstream (original repo)
git remote add upstream https://github.com/deboraaaps/pemprogramanwebI.git
git remote -v  # Verifikasi

# ========== Keep fork synchronized ==========
# Fetch dari original repo
git fetch upstream

# Merge ke main branch Anda
git checkout main
git merge upstream/main

# Push ke fork Anda
git push origin main
```

---

## 📅 Cara Setiap Hari

### **Saat Mulai Bekerja**

```bash
# Update lokal dengan perubahan terbaru
git pull origin main

# Buat branch baru untuk fitur
git checkout -b feature/nama-fitur

# Work on your feature...
```

### **Saat Selesai Fitur**

```bash
# ========== STEP 1: Check status ==========
git status

# ========== STEP 2: Stage changes ==========
git add .

# ========== STEP 3: Commit ==========
git commit -m "feat: complete fitur X

- Added new functionality
- Updated documentation
- Fixed related bugs"

# ========== STEP 4: Push ==========
git push origin feature/nama-fitur

# ========== STEP 5: Create Pull Request ==========
# Buka GitHub → Compare & pull request
```

### **Merge PR ke Main**

```bash
# Setelah PR di-approve:

# Switch ke main
git checkout main

# Pull latest
git pull origin main

# Delete feature branch (local)
git branch -d feature/nama-fitur

# Delete feature branch (remote)
git push origin --delete feature/nama-fitur
```

---

## 🐛 Troubleshooting

### **Problem 1: "fatal: not a git repository"**

```bash
# Solution: Initialize git dulu
git init

# Atau clone repository
git clone https://github.com/deboraaaps/pemprogramanwebI.git
```

### **Problem 2: "Permission denied (publickey)"**

**Solution A: Setup SSH Key**

```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "email@example.com"

# Copy public key
cat ~/.ssh/id_ed25519.pub

# Paste ke GitHub → Settings → SSH Keys → Add SSH Key
```

**Solution B: Pakai HTTPS + Token**

```bash
# Clone dengan HTTPS
git clone https://github.com/deboraaaps/pemprogramanwebI.git

# Masukkan username & personal access token saat diminta
```

**Buat Personal Access Token:**
1. GitHub → Settings → Developer settings → Personal access tokens
2. Generate new token → Select scopes → repo
3. Copy token & gunakan sebagai password

### **Problem 3: "Everything up-to-date"**

```bash
# Berarti tidak ada perubahan untuk di-push
# Cara check:
git status

# Pastikan sudah commit
git log --oneline -5  # Lihat recent commits
```

### **Problem 4: Merge Conflict**

```bash
# Saat git pull muncul conflict:

# ========== STEP 1: Lihat conflict ==========
git status  # Akan show "both modified"

# ========== STEP 2: Edit file manual ==========
# Buka file, cari marker:
# <<<<<<< HEAD
# (kode anda)
# =======
# (kode dari server)
# >>>>>>> branch-name

# Pilih atau kombinasikan, hapus marker

# ========== STEP 3: Resolve ==========
git add .
git commit -m "Resolve merge conflict"
git push origin main
```

### **Problem 5: "Branch 'main' set up to track remote 'origin/main'"**

```bash
# Ini OK, berarti branch sudah linked
# Sekarang cukup pakai:
git push     # instead of git push origin main
git pull     # instead of git pull origin main
```

### **Problem 6: Undo Last Commit**

```bash
# Jika belum push:
git reset --soft HEAD~1  # Keep changes staged
git reset --hard HEAD~1  # Discard changes

# Jika sudah push:
git revert HEAD  # Buat commit baru yang undo
git push origin main
```

---

## ⭐ Best Practices

### **1. Commit Message yang Baik**

```
✅ GOOD:
git commit -m "feat: add dark mode toggle

- Implement toggle button in settings
- Add CSS variables for theme
- Update documentation"

❌ BAD:
git commit -m "fix stuff"
git commit -m "asdfjkl"
git commit -m "wtf"
```

### **2. Commit Sering**

```bash
# ✅ GOOD: Commit setiap fitur kecil selesai
git commit -m "feat: add form validation"

# ❌ BAD: Commit setelah banyak perubahan
git commit -m "update everything"
```

### **3. Pull Sebelum Push**

```bash
# Always lakukan ini:
git pull origin main
git push origin main

# Jangan langsung push tanpa pull!
```

### **4. Gunakan Branch untuk Fitur**

```bash
# ✅ GOOD:
git checkout -b feature/new-design
# ... work ...
git push origin feature/new-design

# ❌ BAD:
# Edit langsung di main branch
git push origin main
```

### **5. Review Before Push**

```bash
# Lihat apa yang akan di-push:
git diff origin/main

# Atau:
git log origin/main..HEAD

# Preview file yang berubah:
git status
```

---

## 🔐 Security Tips

```bash
# ✅ DO:
# - Use HTTPS atau SSH key
# - Don't commit sensitive data
# - Keep token secure

# ❌ DON'T:
# - Commit password/API keys
# - Share SSH keys
# - Use weak tokens
# - Push sensitive files

# Jika accidentally commit secret:
git filter-branch --tree-filter 'rm -f SECRET_FILE' HEAD
git push origin main --force
```

---

## 📊 Useful Commands

```bash
# View history
git log --oneline              # Recent commits
git log --graph --oneline      # Visual tree

# Check differences
git diff                       # Unstaged changes
git diff --cached              # Staged changes
git diff HEAD~1..HEAD          # Last commit

# View remote
git remote -v                  # List remotes
git remote show origin         # Details

# Branch management
git branch                     # List local branches
git branch -r                  # List remote branches
git branch -a                  # All branches

# Clean up
git clean -fd                  # Remove untracked files
git gc                         # Garbage collection
```

---

## 🎯 Skenario Praktis

### **Skenario 1: Update 1 File Sederhana**

```bash
# Edit file
nano README.md

# Check changes
git diff README.md

# Stage, commit, push
git add README.md
git commit -m "docs: update README"
git push origin main
```

### **Skenario 2: Banyak File Berkaitan**

```bash
# Edit multiple files
nano file1.html
nano file2.css
nano README.md

# Stage semua
git add .

# Commit dengan deskripsi detail
git commit -m "feat: implement new design

Files modified:
- file1.html: added new structure
- file2.css: styling untuk new design
- README.md: documented changes

Related to issue #42"

# Push
git push origin main
```

### **Skenario 3: Push Perubahan dari Kolaborator Lain**

```bash
# Check latest dari remote
git fetch origin

# Lihat perbedaan
git log HEAD..origin/main

# Pull untuk update
git pull origin main

# Lihat perubahan
git log --oneline -5
```

---

## 🔄 Workflow Diagram

```
┌─────────────────────────────────────────────────┐
│ 1. MAKE CHANGES                                 │
│    Edit files di editor Anda                   │
└─────────────────┬───────────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────────┐
│ 2. CHECK STATUS                                 │
│    git status                                  │
│    git diff                                    │
└─────────────────┬───────────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────────┐
│ 3. STAGE CHANGES                                │
│    git add .                                   │
└─────────────────┬───────────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────────┐
│ 4. COMMIT                                       │
│    git commit -m "message"                     │
└─────────────────┬───────────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────────┐
│ 5. PULL (update)                                │
│    git pull origin main                        │
└─────────────────┬───────────────────────────────┘
                  │
                  ▼
┌─────────────────────────────────────────────────┐
│ 6. PUSH                                         │
│    git push origin main                        │
└─────────────────┬───────────────────────────────┘
                  │
                  ▼
         ✅ SELESAI!
```

---

## 📱 Command Cheat Sheet

```bash
# SETUP
git init                           # Initialize repository
git clone <URL>                    # Clone repository
git config user.name "<name>"      # Set name

# DAILY WORKFLOW
git status                         # Check status
git add .                          # Stage all files
git commit -m "message"            # Commit
git push origin main               # Push
git pull origin main               # Pull

# BRANCHES
git branch <name>                  # Create branch
git checkout <branch>              # Switch branch
git checkout -b <branch>           # Create & switch
git merge <branch>                 # Merge branch
git branch -d <branch>             # Delete branch

# HISTORY
git log                            # View history
git log --oneline                  # Short history
git show <commit>                  # Show commit details
git revert <commit>                # Undo commit

# UNDO
git reset <file>                   # Unstage file
git reset --hard HEAD~1            # Undo last commit
git checkout <file>                # Discard changes

# REMOTE
git remote -v                      # List remotes
git fetch origin                   # Fetch updates
git pull origin main               # Fetch & merge
git push origin main               # Push changes
```

---

## 🎓 Referensi

- [Official Git Documentation](https://git-scm.com/doc)
- [GitHub Help](https://docs.github.com/en)
- [Atlassian Git Tutorials](https://www.atlassian.com/git)
- [Git - Simple Guide](https://rogerdudler.github.io/git-guide/)

---

## ❓ FAQ

**Q: Berapa sering harus push?**  
A: Setiap fitur kecil selesai, atau minimal 1x sehari.

**Q: Apa bedanya commit & push?**  
A: Commit = simpan lokal, Push = kirim ke GitHub.

**Q: Bagaimana jika lupa pull sebelum push?**  
A: Git akan reject, lakukan pull dulu, resolve conflict jika ada.

**Q: Bisa undo push?**  
A: Ya, pakai `git revert` untuk membuat commit baru yang undo.

**Q: Perlu branch untuk setiap fitur?**  
A: Best practice ya, tapi tidak wajib untuk project kecil.

---

<div align="center">

**Selamat! Sekarang Anda siap update GitHub! 🚀**

Jika masih bingung, lihat contoh praktis di skenario.

Good luck! 💪

</div>

---

*Last Updated: Desember 2025*
