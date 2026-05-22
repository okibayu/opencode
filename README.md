<p align="center">
<a href="[https://opencode.ai](https://opencode.ai)">
<picture>
<source srcset="packages/console/app/src/asset/logo-ornate-dark.svg" media="(prefers-color-scheme: dark)">
<source srcset="packages/console/app/src/asset/logo-ornate-light.svg" media="(prefers-color-scheme: light)">
<img src="packages/console/app/src/asset/logo-ornate-light.svg" alt="OpenCode logo">
</picture>
</a>
</p>
<p align="center">Agen pengodean AI sumber terbuka (open source).</p>
<p align="center">
<a href="[https://opencode.ai/discord](https://opencode.ai/discord)"><img alt="Discord" src="[https://img.shields.io/discord/1391832426048651334?style=flat-square&label=discord](https://img.shields.io/discord/1391832426048651334?style=flat-square&label=discord)" /></a>
<a href="[https://www.npmjs.com/package/opencode-ai](https://www.npmjs.com/package/opencode-ai)"><img alt="npm" src="[https://img.shields.io/npm/v/opencode-ai?style=flat-square](https://img.shields.io/npm/v/opencode-ai?style=flat-square)" /></a>
<a href="[https://github.com/anomalyco/opencode/actions/workflows/publish.yml](https://github.com/anomalyco/opencode/actions/workflows/publish.yml)"><img alt="Build status" src="[https://img.shields.io/github/actions/workflow/status/anomalyco/opencode/publish.yml?style=flat-square&branch=dev](https://img.shields.io/github/actions/workflow/status/anomalyco/opencode/publish.yml?style=flat-square&branch=dev)" /></a>
</p>
<p align="center">
<a href="README.md">English</a> |
<a href="README.zh.md">简体中文</a> |
<a href="README.zht.md">繁體中文</a> |
<a href="README.ko.md">한국어</a> |
<a href="README.de.md">Deutsch</a> |
<a href="README.es.md">Español</a> |
<a href="README.fr.md">Français</a> |
<a href="README.it.md">Italiano</a> |
<a href="README.da.md">Dansk</a> |
<a href="README.ja.md">日本語</a> |
<a href="README.pl.md">Polski</a> |
<a href="README.ru.md">Русский</a> |
<a href="README.bs.md">Bosanski</a> |
<a href="README.ar.md">العربية</a> |
<a href="README.no.md">Norsk</a> |
<a href="README.br.md">Português (Brasil)</a> |
<a href="README.th.md">ไทย</a> |
<a href="README.tr.md">Türkçe</a> |
<a href="README.uk.md">Українська</a> |
<a href="README.bn.md">বাংলা</a> |
<a href="README.gr.md">Ελληνικά</a> |
<a href="README.vi.md">Tiếng Việt</a>
</p>
OpenCode Terminal UI
### Instalasi
```bash
# YOLO
curl -fsSL https://opencode.ai/install | bash
# Package managers
npm i -g opencode-ai@latest        # atau bun/pnpm/yarn
scoop install opencode             # Windows
choco install opencode             # Windows
brew install anomalyco/tap/opencode # macOS dan Linux (direkomendasikan, selalu diperbarui)
brew install opencode              # macOS dan Linux (formula brew resmi, lebih jarang diperbarui)
sudo pacman -S opencode            # Arch Linux (Stabil)
paru -S opencode-bin               # Arch Linux (Terbaru dari AUR)
mise use -g opencode               # OS apa pun
nix run nixpkgs#opencode           # atau github:anomalyco/opencode untuk branch dev terbaru
```
> [!TIP]
> Hapus versi yang lebih lama dari 0.1.x sebelum melakukan instalasi.
> 
### Aplikasi Desktop (BETA)
OpenCode juga tersedia sebagai aplikasi desktop. Unduh langsung dari halaman rilis atau opencode.ai/download.

| Platform | Unduh |
| :--- | :--- |
| macOS (Apple Silicon) | opencode-desktop-mac-arm64.dmg |
| macOS (Intel) | opencode-desktop-mac-x64.dmg |
| Windows | opencode-desktop-windows-x64.exe |
| Linux | .deb, .rpm, atau .AppImage |

```bash
# macOS (Homebrew)
brew install --cask opencode-desktop
# Windows (Scoop)
scoop bucket add extras; scoop install extras/opencode-desktop
```
#### Direktori Instalasi
Skrip instalasi mengikuti urutan prioritas berikut untuk jalur instalasi:
 1. $OPENCODE_INSTALL_DIR - Direktori instalasi kustom
 2. $XDG_BIN_DIR - Jalur yang sesuai dengan Spesifikasi Direktori Dasar XDG
 3. $HOME/bin - Direktori biner pengguna standar (jika ada atau bisa dibuat)
 4. $HOME/.opencode/bin - Cadangan default
```bash
# Contoh
OPENCODE_INSTALL_DIR=/usr/local/bin curl -fsSL https://opencode.ai/install | bash
XDG_BIN_DIR=$HOME/.local/bin curl -fsSL https://opencode.ai/install | bash
```
### Agen
OpenCode menyertakan dua agen bawaan yang bisa Anda ganti dengan menekan tombol Tab.
 * **build** - Agen default dengan akses penuh untuk pekerjaan pengembangan
 * **plan** - Agen dengan akses baca-saja untuk analisis dan eksplorasi kode
   * Menolak pengeditan file secara default
   * Meminta izin sebelum menjalankan perintah bash
   * Ideal untuk menjelajahi basis kode yang tidak dikenal atau merencanakan perubahan
Juga disertakan sub-agen **general** untuk pencarian kompleks dan tugas multi-langkah.
Agen ini digunakan secara internal dan dapat dipanggil menggunakan @general dalam pesan.
Pelajari lebih lanjut tentang agen.
### Dokumentasi
Untuk informasi lebih lanjut tentang cara mengonfigurasi OpenCode, **kunjungi dokumentasi kami**.
### Kontribusi
Jika Anda tertarik untuk berkontribusi pada OpenCode, silakan baca dokumentasi kontribusi kami sebelum mengirimkan pull request.
### Membangun di Atas OpenCode
Jika Anda mengerjakan proyek yang terkait dengan OpenCode dan menggunakan "opencode" sebagai bagian dari namanya, contohnya "opencode-dashboard" atau "opencode-mobile", harap tambahkan catatan di README Anda untuk mengklarifikasi bahwa proyek tersebut tidak dibuat oleh tim OpenCode dan tidak berafiliasi dengan kami dalam bentuk apa pun.
**Bergabunglah dengan komunitas kami** Discord | X.com