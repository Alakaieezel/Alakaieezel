# Panduan Profil GitHub — Muhammad Haikal Aghista

Repo ini sudah dipersonalisasi untuk akun **`Alakaieezel`**. Tinggal dipasang di repo spesial GitHub, lalu dirawat.

## 1. Buat repo spesial

README profil hanya tampil kalau nama repo **sama dengan username** dan repo-nya **public**.

1. Buka `https://github.com/new`
2. Repository name: `Alakaieezel`
3. Public → centang **Add a README file** → Create
4. Kosongkan README bawaan, lalu copy semua isi folder ini:

```
README.md
SETUP.md
assets/banner.svg
assets/footer.svg
.github/workflows/snake.yml
```

## 2. Push

Dari folder ini:

```powershell
git init
git add .
git commit -m "feat: profile readme with custom banner"
git branch -M main
git remote add origin https://github.com/Alakaieezel/Alakaieezel.git
git push -u origin main
```

Buka `https://github.com/Alakaieezel` — banner dan README langsung tampil.

## 3. Data yang sudah dipasang

| Bagian | Isi |
| :-- | :-- |
| Nama di banner | Haikal Aghista |
| Role | Fullstack Developer · Informatics Student |
| Portfolio | https://alakaieezel.github.io/Portofolio/ (sudah live) |
| Instagram | https://www.instagram.com/hykall_ags |
| TikTok | https://www.tiktok.com/@hykalags |
| Highlights | Portofolio Angkasa + repo profil ini |
| Stack | HTML, CSS, JS, React, Tailwind, Git, GitHub, VS Code, Node.js, Python, PostgreSQL, MongoDB, Docker, Actions, npm, Bash |

## 4. Yang sebaiknya kamu rapikan di GitHub (bukan di README)

- **Settings → Profile**: ganti *Name* jadi `Muhammad Haikal Aghista`, isi *Bio* singkat, tambahkan *Location* dan *Website* (`https://alakaieezel.github.io/Portofolio/`).
- **Pin repository**: buka profil → *Customize your pins* → pilih `Portofolio`. Nanti kalau repo lain sudah ada, pin 3–6 yang terbaik.
- **Repo Portofolio**: tambahkan *Description* + *Topics* (`portfolio`, `javascript`, `solar-system`, `frontend`).
- **Repo profil**: isi description `My GitHub profile` dan topic `profile-readme`.

Kenapa penting: kartu "Popular repositories" di halaman profil diambil dari pin, bukan dari README. Bagian ini yang dilihat orang sebelum scroll.

## 5. Opsional: animasi snake

Snake menghasilkan gambar dari grafik kontribusi. Sekarang kontribusinya masih sedikit, jadi di README bloknya masih dikomentari. Kalau sudah ramai:

1. **Settings → Actions → General → Workflow permissions** → pilih **Read and write permissions** → Save
2. Tab **Actions** → *Generate Snake* → **Run workflow** (tunggu ±1 menit, branch `output` muncul)
3. Buka `README.md`, cari komentar `SNAKE ANIMATION (opsional)`, hapus `<!--` dan `-->`
4. Commit + push

## 6. Cara edit konten

| Mau ganti | Edit di |
| :-- | :-- |
| Nama, role, tagline, chip di banner | `assets/banner.svg` (cari `<text`) |
| Teks perkenalan + list fakta | `README.md`, section `❯ whoami` |
| Daftar project | `README.md`, tabel `❯ highlights` |
| Icon teknologi | URL `skillicons.dev/icons?i=...` di section `❯ stack` |
| Warna aksen | ganti `0B1020`, `22D3EE`, `8B5CF6`, `34D399` di `README.md` + `assets/*.svg` |
| Link sosial | badge di bagian atas `README.md` |

Setelah edit SVG, cek cepat: buka file di browser. Kalau tampil, XML-nya valid.

## 7. Catatan teknis

- **Kartu statistik** memakai `github-profile-summary-cards.vercel.app` (aktif saat dibuat). Dulu sempat pakai `github-readme-stats`, tapi servicenya sedang mati total (503). Kalau suatu saat kartu ini rusak, fork repo `github-profile-summary-cards`, deploy sendiri ke Vercel, ganti domainnya.
- Kartu statistik sengaja dimasukkan ke `<details>` (tertutup default) karena jumlah kontribusi masih kecil — lebih rapi begitu, dan tinggal dibuka kalau mau.
- **Skill icons** otomatis ikut tema terang/gelap lewat `<picture>` + `prefers-color-scheme`.

## 8. Checklist

- [ ] Repo `Alakaieezel/Alakaieezel` public dan sudah di-push
- [ ] Profil menampilkan banner + README
- [ ] Nama, bio, website, dan pin repo sudah dirapikan
- [ ] Cek tampilan di mode terang dan gelap
- [ ] Cek di HP (badge akan turun baris, itu normal)
- [ ] (Opsional) snake diaktifkan setelah kontribusi mulai ramai
