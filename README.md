# Portofolio — Syafaq Jiwa Raharjo

Website portofolio pribadi yang dibangun untuk **Tugas K2 — Teknologi Platform (ITB)**.
Situs statis (HTML, CSS, JavaScript) yang di-deploy otomatis menggunakan **CI/CD pipeline**.

🔗 **Live:** https://syafaq2112.github.io/portofolio-website/

## ✨ Fitur

- Desain modern, responsif (mobile & desktop)
- Mode gelap / terang dengan penyimpanan preferensi
- Animasi reveal saat scroll, progress bar, smooth scrolling
- Section: Hero, Tentang, Pendidikan, Pengalaman, Proyek, Skill, Kontak

## 🛠️ Teknologi

| Bagian       | Teknologi                          |
| ------------ | ---------------------------------- |
| Markup       | HTML5                              |
| Styling      | CSS3 (custom properties, grid)     |
| Interaktif   | JavaScript (vanilla)               |
| CI/CD        | GitHub Actions → GitHub Pages      |

## 🚀 Menjalankan secara lokal

```bash
# dari dalam folder proyek
python3 -m http.server 4321
# lalu buka http://localhost:4321
```

## ⚙️ Deployment (CI/CD)

Situs di-deploy ke **GitHub Pages** dengan sumber **branch `main`**. Setiap
`git push` ke `main` otomatis memicu pipeline bawaan GitHub
(`pages-build-deployment`, terlihat di tab **Actions**) yang membangun ulang dan
mempublikasikan situs. Inilah inti CI/CD: **perubahan kode → otomatis live**,
tanpa langkah manual.

Alur demonstrasi:

```bash
# ubah sesuatu di index.html, lalu:
git add .
git commit -m "update konten"
git push
# tab Actions akan menjalankan pages-build-deployment,
# beberapa saat kemudian situs live ikut berubah.
```

## 📁 Struktur

```
portofolio-website/
├── index.html      # Halaman utama
├── styles.css      # Seluruh styling
├── script.js       # Interaktivitas
└── README.md
```
