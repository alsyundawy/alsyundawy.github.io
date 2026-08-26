# ALSYUNDAWY IT SOLUTION

## System Administrator · DNS & ISP Infrastructure Specialist · Mail & Virtualization Expert

![Portfolio](https://alsyundawy.github.io/portofolio.webp)

**Harry Dertin Sutisna Alsyundawy** · DKI Jakarta, Indonesia

[![Website](https://img.shields.io/badge/Website-alsyundawy.com-blue?style=flat-square)](https://alsyundawy.com)
[![GitHub](https://img.shields.io/badge/GitHub-alsyundawy-black?style=flat-square&logo=github)](https://github.com/alsyundawy)
[![Email](https://img.shields.io/badge/Email-alsyundawy%40gmail.com-red?style=flat-square&logo=gmail)](mailto:alsyundawy@gmail.com)
[![Phone](https://img.shields.io/badge/Phone-%2B6285658515212-green?style=flat-square&logo=whatsapp)](https://wa.me/6285658515212)
[![License](https://img.shields.io/badge/License-Copyleft-lightgrey?style=flat-square)](#license)

[![Followers](https://img.shields.io/github/followers/alsyundawy?label=Followers&style=flat-square&color=3b82f6)](https://github.com/alsyundawy)
[![Stars](https://img.shields.io/github/stars/alsyundawy/alsyundawy.github.io?style=flat-square&color=7c3aed)](https://github.com/alsyundawy/alsyundawy.github.io/stargazers)
[![Forks](https://img.shields.io/github/forks/alsyundawy/alsyundawy.github.io?style=flat-square&color=10b981)](https://github.com/alsyundawy/alsyundawy.github.io/network/members)

---

## Overview

Portfolio profesional satu halaman yang menampilkan keahlian teknis tingkat lanjut di bidang **System Administration**, **DNS/RPZ Infrastructure**, **ISP Hardware**, **Hypervisor & Virtualization**, **Mail Systems**, dan **Apple Mac Ecosystem**.

Dikembangkan dengan fokus pada:

- **Performa tinggi** — scroll 60 FPS, optimasi DOM, dan lazy loading
- **Keamanan modern** — SRI hash, CSP-ready, dan CDN integrity checks
- **Aksesibilitas** — WCAG-oriented, dark/light mode, keyboard navigation
- **Responsif** — optimal dari 320px hingga 4K display
- **SEO-friendly** — structured data, Open Graph, Twitter Cards, sitemap

> **Live Demo:** [https://alsyundawy.github.io](https://alsyundawy.github.io)

---

## Quickstart

Untuk menjalankan atau meninjau portfolio secara lokal di komputer Anda:

```bash
# Clone repository
git clone https://github.com/alsyundawy/alsyundawy.github.io.git
cd alsyundawy.github.io

# Opsi 1: Buka langsung index.html di browser
open index.html

# Opsi 2: Menggunakan HTTP server lokal (direkomendasikan)
python3 -m http.server 8000
# Buka http://localhost:8000 pada browser
```

---

## Dependencies

Repository ini menggunakan arsitektur web modern tanpa dependency build framework yang rumit, mengandalkan CDN assets terlindungi Subresource Integrity (SRI):

| Komponen | Teknologi / Library | Versi / Sumber |
| ---------- | -------------------- | ---------------- |
| **Structure** | HTML5 Semantic | Standar W3C Living Standard |
| **Styling** | Vanilla CSS + CSS Custom Properties | Native CSS |
| **UI Framework** | Bootstrap (Grid, Utilities & Components) | 5.3.8 (CDN via jsDelivr + SRI) |
| **Icons** | Font Awesome Free | 6.7.2 (CDN via cdnjs + SRI) |
| **Typography** | Google Fonts (Inter) | Modern Sans-Serif |
| **Logic** | Vanilla JavaScript | ES6+ Modern JavaScript |
| **Hosting** | GitHub Pages & Custom Domain | GitHub Static Infrastructure |

---

## Configuration

Website portofolio ini dapat dikonfigurasi melalui beberapa file kunci:

- **Metadata & SEO**: Diatur langsung di bagian `<head>` pada `index.html` (OpenGraph, Twitter Cards, dan Schema.org JSON-LD).
- **Theme & Color Modes**: Mendukung light/dark theme otomatis sesuai preferensi sistem (`prefers-color-scheme`) atau disimpan manual di `localStorage` dengan key `theme`.
- **PWA & Manifest**: Dikonfigurasi pada `site.webmanifest` untuk metadata nama aplikasi, ikon, dan tema browser.
- **Sitemap**: Didefinisikan pada `sitemap.xml` untuk indexing search engine (Google, Bing).
- **Minifikasi Inline**: Skrip pemroses `minify_inline.py` tersedia untuk memadatkan inline CSS dan JS secara aman sebelum rilis.

---

## Running Tests

Uji kualitas, validitas sintaks, dan performa halaman web dapat dijalankan menggunakan:

```bash
# 1. Validasi struktur HTML dan data JSON-LD (Python)
python3 -c "import json, re; c=open('index.html').read(); json.loads(re.search(r'<script type=\"application/ld\+json\">(.*?)</script>', c, re.S).group(1)); print('JSON-LD OK')"

# 2. Uji HTTP server lokal
python3 -m http.server 8899 &
curl -I http://localhost:8899/index.html

# 3. Audit performa & aksesibilitas
# Buka Google Chrome DevTools -> Lighthouse -> Run Navigation Audit (Performance, Accessibility, Best Practices, SEO)
```

---

## Area Keahlian

| Domain | Spesialisasi |
| -------- | ------------- |
| **ISP Hardware & Infrastructure** | Server deployment, MikroTik RouterOS, bandwidth management, monitoring 99.9% uptime |
| **DNS & RPZ** | PowerDNS, BIND9, DNSSEC, TrustPositif integration, DNS filtering enterprise |
| **DNS Security** | RPZ binary conversion, blacklist/whitelist management, threat intelligence |
| **Virtualization** | Proxmox VE, VMware vCenter/ESXi, KVM, Hyper-V, HA clustering, VM migration 100+ |
| **Mail & SMTP** | Zimbra, Proxmox Mail Gateway, WHM/cPanel, DKIM/SPF/DMARC, antispam, forensic incident response & malware remediation |
| **Apple macOS** | macOS deployment, FileVault, Apple Silicon optimization, MDM bypass |
| **Monitoring** | Smokeping, Uptime Kuma, Grafana, Prometheus, Zabbix, Nagios, PRTG |
| **Linux SysAdmin** | Ubuntu, Debian, FreeBSD, CentOS, Bash automation, SELinux, Fail2ban |

---

## Fitur Utama

- **Theme Toggle** — Dark/Light mode dengan localStorage persistence
- **Smooth Scroll** — Navigasi antar section dengan requestAnimationFrame
- **Image Fallbacks** — Graceful degradation untuk gambar yang gagal dimuat
- **Intersection Observer** — Reveal animations performan tinggi
- **SEO Optimized** — 50+ meta tags, JSON-LD structured data, Open Graph
- **PWA Ready** — Web App Manifest, favicon set lengkap
- **CLS Optimized** — Dimensi eksplisit pada semua gambar
- **SRI Protected** — Subresource Integrity pada CDN assets

---

## Struktur Proyek

```bash
├── index.html                   # Berkas HTML utama portofolio
├── portofolio.webp              # Foto profil hero beresolusi tinggi (WebP)
├── alsyundawy-hero.webp         # Gambar latar belakang hero section
├── favicon.ico                  # Aset favicon klasik 
├── favicon.svg                  # Favicon modern berbasis vektor
├── favicon-16x16.png            # Favicon ukuran kecil
├── favicon-32x32.png            # Favicon ukuran sedang
├── apple-touch-icon.png         # Ikon untuk sistem iOS/Apple Devices
├── site.webmanifest             # Manifest konfigurasi aplikasi web
├── sitemap.xml                  # Peta situs untuk pengoptimalan SEO
├── minify_inline.py             # Script helper minifikasi inline CSS & JS
└── xmg/                         # Direktori gambar logo klien & branding IT
```

---

## Repositori & Proyek

### Original Creations

- [TrustPositif To RPZ Binary](https://github.com/alsyundawy/TrustPositif-To-RPZ-Binary) — Konversi blacklist TrustPositif ke PowerDNS RPZ binary
- [TrustPositif Database](https://github.com/alsyundawy/TrustPositif) — Database TrustPositif Kominfo dengan auto-update harian
- [TrustPositif Validator](https://github.com/alsyundawy/TrustPositif-Validator) — Validasi domain multi-core dengan RFC compliance
- [Sunat TrustPositif](https://github.com/alsyundawy/sunat-trustpositif) — Validasi dan pembersihan data TrustPositif
- [StevenBlack Host RPZ](https://github.com/alsyundawy/StevenBlack-Host-RPZ) — Database blacklist komprehensif
- [PHP Looking Glass](https://github.com/alsyundawy/php-looking-glass) — Single-file PHP Looking Glass untuk diagnostik jaringan
- [MikroTik Script Automation](https://github.com/alsyundawy/MIKROTIK-SCRIPT) — Kumpulan script otomatisasi MikroTik
- [MikroTik Blacklist](https://github.com/alsyundawy/mikrotik-blacklist) — Sistem manajemen blacklist otomatis
- [ACL BIND9 Indonesia + OpenIXP](https://github.com/alsyundawy/bind-acl-indonesia-openixp) — Generator ACL Indonesia untuk BIND9
- [DNS Performance Test](https://github.com/alsyundawy/dnsperftest) — Benchmarking DNS dengan reporting detail
- [UFW Ipset Blocklist Auto Update](https://github.com/alsyundawy/ufw-ipset-blocklist-autoupdate) — Auto-update blokir IP dengan ipset & UFW
- [PowerDNS Zone Backups](https://github.com/alsyundawy/PowerDNS-Zone-Backups) — Backup otomatis PowerDNS dengan incremental backup
- [Microsoft Office for macOS](https://github.com/alsyundawy/Microsoft-Office-For-MacOS) — Installer Office macOS (Intel & Apple Silicon) ⭐ 5.9k
- [SkipMDM macOS Bypass](https://github.com/alsyundawy/skipmdm-bypass) — Bypass MDM untuk macOS Monterey/Ventura/Sonoma
- [PHP File & Directory Browser](https://github.com/alsyundawy/File-Directory-Browser) — Browser file PHP dengan CSRF protection
- [ZCS Eradicate Malware Suite](https://github.com/alsyundawy/eradicate-zimbra-malware) — Enterprise Forensic Incident Response, Anti-Ransomware & Zimbra Permission Healing Suite
- [Zimbra Clean Spam](https://github.com/alsyundawy/Zimbra-Clean-Spam) — Pembersihan antrian spam Zimbra
- [Bash Script Uninstall Zimbra](https://github.com/alsyundawy/uninstall-zimbra) — Uninstall Zimbra lengkap
- [Z2C Migration](https://github.com/alsyundawy/Z2C) — Migrasi Zimbra ke Carbonio

### Maintained Forks

- [The Best Blocklist Collection](https://github.com/alsyundawy/Sefinek-Blocklist-Collection) — 100+ links, 5+ juta domain
- [Hagezi DNS Blocklists](https://github.com/alsyundawy/dns-blocklists) — DNS filtering lists komprehensif
- [Generic Shell Script Compiler (SHC)](https://github.com/alsyundawy/shc) — Kompiler shell script dengan enkripsi
- [NotepadNext for macOS](https://github.com/alsyundawy/NotepadNext-MacOS) — Notepad++ untuk macOS
- [Xiaomi ADB & Fastboot Tools](https://github.com/alsyundawy/XiaomiADBFastbootTools-Win32) — Tools diagnostik Xiaomi
- [OpenVPN Road Warrior Installer](https://github.com/alsyundawy/OpenVPN-Install) — Installer OpenVPN dual-stack IPv4/IPv6

---

## Tutorial & Panduan Teknis

16 panduan komprehensif untuk administrasi sistem dan infrastruktur:

| Tutorial | Topik |
| ---------- | ------- |
| [Build Zimbra FOSS](https://alsyundawy.com/Build-Zimbra-FOSS.html) | Build Zimbra dari source |
| [Install Zimbra FOSS](https://alsyundawy.com/Install-Zimbra-FOSS.html) | Instalasi Zimbra pada Ubuntu/Rocky Linux |
| [Cacti Monitoring Stack](https://alsyundawy.com/Cacti.html) | Network graphing pada Debian |
| [HyperGlass](https://alsyundawy.com/HyperGlass.html) | BGP Looking Glass modern berbasis Python |
| [Ookla Speedtest Server](https://alsyundawy.com/Ookla-Speedtest.html) | Deployment Speedtest Server dual-stack |
| [OpenVPN Road Warrior](https://alsyundawy.com/OpenVPN-Install.html) | OpenVPN dengan Unbound DNS |
| [PHP PowerAdmin](https://alsyundawy.com/PowerAdmin.html) | PowerDNS Authoritative dengan web UI |
| [PHP-LookingGlass](https://alsyundawy.com/PHP-LookingGlass.html) | Alat diagnostik jaringan single-file |
| [phpIPAM](https://alsyundawy.com/phpIPAM.html) | IP Address Management open-source |
| [PowerDNS-Admin Debian](https://alsyundawy.com/PowerDNS-Admin-Debian.html) | PowerDNS Master-Slave pada Debian |
| [PowerDNS-Admin Ubuntu](https://alsyundawy.com/PowerDNS-Admin-Ubuntu.html) | PowerDNS dengan MariaDB & Flask |
| [Prometheus & Grafana](https://alsyundawy.com/Prometheus-Grafana-Debian.html) | Stack monitoring lengkap |
| [Proxmox VE 9](https://alsyundawy.com/Proxmox-VE-9.html) | Instalasi & konfigurasi Proxmox |
| [TrustPositif RPZ Install](https://alsyundawy.com/TrustPositif-RPZ-Install.html) | BIND9 DNS Filtering TrustPositif |
| [vSphere Unsupported HW](https://alsyundawy.com/vSphere.html) | vSphere/ESXi pada hardware tidak didukung |
| [WalkieFleet Server](https://alsyundawy.com/WalkieFleet.html) | Push-to-Talk server pada Debian/Ubuntu |

---

## Klien & Mitra

Dipercaya oleh **56+ perusahaan dan organisasi** di bidang ISP, networking, dan IT infrastructure di Indonesia.

[Lihat semua klien →](https://alsyundawy.github.io/#clients)

---

## Statistik GitHub

[![GitHub followers](https://img.shields.io/github/followers/alsyundawy?label=Followers&style=flat-square&color=3b82f6)](https://github.com/alsyundawy)
[![GitHub stars](https://img.shields.io/github/stars/alsyundawy?style=flat-square&color=7c3aed)](https://github.com/alsyundawy)
[![GitHub forks](https://img.shields.io/github/forks/alsyundawy/alsyundawy.github.io?style=flat-square&color=10b981)](https://github.com/alsyundawy/alsyundawy.github.io/network/members)
[![Contributions](https://img.shields.io/badge/Contributions-10%2C407%2B-brightgreen?style=flat-square)](https://github.com/alsyundawy)

---

## Tautan Penting

| Platform | URL |
| ---------- | ----- |
| **Website** | [https://alsyundawy.com](https://alsyundawy.com) |
| **GitHub** | [https://github.com/alsyundawy](https://github.com/alsyundawy) |
| **Portfolio** | [https://alsyundawy.github.io](https://alsyundawy.github.io) |
| **Email** | [alsyundawy@gmail.com](mailto:alsyundawy@gmail.com) |
| **WhatsApp** | [+62 856-5851-5212](https://wa.me/6285658515212) |
| **Telegram** | [@alsyundawy](https://t.me/alsyundawy) |
| **YouTube** | [@alsyundawy](https://youtube.com/@alsyundawy) |
| **Instagram** | [@harry.ds.alsyundawy](https://instagram.com/harry.ds.alsyundawy) |
| **Facebook** | [alsyundawy](https://facebook.com/alsyundawy) |
| **X/Twitter** | [@Alsyundawy](https://x.com/Alsyundawy) |
| **PayPal** | [paypal.me/alsyundawy](https://www.paypal.me/alsyundawy) |

---

## Contributing

Kontribusi sangat diterima! Jika Anda ingin:

- Melaporkan bug atau masalah tampilan
- Mengajukan fitur atau optimasi baru
- Memperbaiki dokumentasi
- Menambahkan tautan tutorial

Silakan buat [Issue](https://github.com/alsyundawy/alsyundawy.github.io/issues) atau ajukan [Pull Request](https://github.com/alsyundawy/alsyundawy.github.io/pulls).

---

## License

Copyleft (c) 2026 **ALSYUNDAWY IT SOLUTION** (Harry Dertin Sutisna).

Kode sumber terbuka bagi siapa saja yang ingin berkreasi dan memanfaatkannya dengan tetap mencantumkan atribusi kredit pemilik asli.

---

## Dibuat dengan ❤️ oleh Harry Dertin Sutisna Alsyundawy

[⬆ Kembali ke atas](#alsyundawy-it-solution)
