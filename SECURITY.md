# 🛡️ Kebijakan Keamanan (Security Policy)

**🇮🇩 Bahasa Indonesia** | [🇬🇧 English](#-security-policy-english)

Keamanan komunitas ThyoCloud adalah prioritas kami. Dokumen ini menjelaskan versi yang didukung, cara melaporkan kerentanan, apa yang kami harapkan dari pelapor, dan apa yang bisa Anda harapkan dari kami.

---

## 📦 Versi yang Didukung

| Versi / Branch | Dukungan Keamanan |
|:---|:---:|
| `main` (terbaru) | ✅ Didukung |
| Fork yang tertinggal dari `main` | ❌ Tidak didukung |

Perbaikan keamanan hanya dirilis di *branch* `main`. Harap selalu sinkronkan hasil *fork* Anda dengan *branch* utama kami.

---

## 🎯 Cakupan (Scope)

**Termasuk dalam cakupan:**

- Website resmi [thyo.cloud](https://thyo.cloud) beserta API-nya
- Bot Telegram `@ThyoCloudBot` (verifikasi token dan pengiriman kredensial)
- Repositori ini, termasuk workflow GitHub Actions
- Alur pembuatan token, verifikasi, dan penyimpanan/penghapusan kredensial sementara

**Di luar cakupan:**

- Kelemahan pada layanan pihak ketiga (GitHub, Telegram, Railway, Cloudflare, dll.). Laporkan langsung ke vendor terkait
- Serangan *Denial of Service* (DoS/DDoS), *spam*, atau uji beban
- *Social engineering* atau *phishing* terhadap admin maupun pengguna
- Laporan hasil *scanner* otomatis tanpa bukti dampak nyata (*proof of concept*)
- Masalah akibat kelalaian pengguna sendiri, misalnya membagikan token atau kredensial RDP ke orang lain
- Temuan yang membutuhkan akses fisik ke perangkat pengguna

---

## 🔍 Pelaporan Kerentanan (Vulnerability Reporting)

> 🚨 **Tolong JANGAN memublikasikan kerentanan secara publik, di GitHub Issues, Discussions, atau grup komunitas sebelum kami sempat memperbaikinya.**

Kami menganut prinsip *Responsible Disclosure*. Laporkan temuan Anda secara privat melalui:

| Kanal | Keterangan |
|:---|:---|
| 💬 **Telegram (DM)** | [Hubungi Admin ThyoCloud](https://t.me/thyocloud), kirim pesan langsung ke admin, bukan di grup publik |

### 📝 Yang Perlu Disertakan dalam Laporan

Semakin lengkap laporan Anda, semakin cepat kami dapat menindaklanjuti:

1. **Ringkasan** kerentanan dan komponen yang terdampak (website, API, bot, workflow)
2. **Langkah reproduksi** yang jelas, berurutan, dan dapat diulang
3. **Bukti** (*proof of concept*), berupa tangkapan layar, video singkat, atau *request/response*
4. **Dampak** yang Anda perkirakan (data apa yang bisa bocor, akses apa yang bisa didapat)
5. **Saran perbaikan** (opsional, tapi sangat dihargai)
6. **Nama/alias** yang ingin dicantumkan di Hall of Fame (opsional)

---

## ⏱️ Yang Bisa Anda Harapkan dari Kami

| Tahap | Target Waktu |
|:---|:---:|
| 📬 Konfirmasi laporan diterima | 24–48 jam |
| 🔎 Triase dan validasi awal | ± 3–7 hari |
| 🛠️ Perbaikan (tergantung tingkat keparahan) | Kritis: secepatnya · Lainnya: sesuai kompleksitas |
| 📢 Pengungkapan publik terkoordinasi | Setelah perbaikan dirilis, dibahas bersama pelapor |

Kami akan mengabari Anda secara berkala mengenai perkembangan laporan. Mohon beri kami waktu yang wajar (disarankan hingga **90 hari**) untuk memperbaiki sebelum Anda mengungkapkan temuan ke publik.

### 📊 Tingkat Keparahan

| Level | Contoh |
|:---:|:---|
| 🔴 **Kritis** | Kebocoran kredensial RDP pengguna, pengambilalihan akun, eksekusi kode di infrastruktur kami |
| 🟠 **Tinggi** | Bypass verifikasi token, akses tanpa izin ke data pengguna atau panel admin |
| 🟡 **Sedang** | Kelemahan validasi yang berdampak terbatas, kebocoran informasi non-sensitif |
| 🟢 **Rendah** | Masalah konfigurasi minor, *hardening* yang disarankan |

---

## 🤝 Safe Harbor (Perlindungan bagi Peneliti)

Kami tidak akan mengambil tindakan hukum terhadap peneliti yang bertindak dengan itikad baik dan mematuhi kebijakan ini. Agar tetap berada dalam perlindungan tersebut, mohon:

- ✅ Hanya menguji **akun dan instance milik Anda sendiri**
- ✅ Berhenti dan segera melapor jika tanpa sengaja mengakses data pengguna lain
- ✅ Tidak mengunduh, menyalin, mengubah, atau menghapus data milik pengguna lain
- ✅ Tidak mengganggu ketersediaan layanan bagi pengguna lain
- ✅ Tidak membagikan temuan ke pihak lain sebelum diperbaiki
- ❌ Tidak menggunakan temuan untuk keuntungan pribadi atau memeras

---

## 🔐 Catatan Penanganan Data

Sesuai [Catatan Transparansi](README.md#️-keamanan--transparansi) di README: RDP adalah layanan gratis berbatas waktu (maksimal 6 jam) dan dikelola terpusat. Salinan kredensial disimpan **sementara** untuk keperluan dukungan teknis, lalu **dihapus otomatis** setelah sesi kedaluwarsa. Setiap celah yang berkaitan dengan penyimpanan atau penghapusan data ini kami anggap **prioritas tinggi**.

---

## 🏆 Pengakuan (Recognition)

Kami menghargai setiap kontribusi. Pelapor dengan temuan valid dapat:

- 🏅 Dicantumkan di **[Security Hall of Fame](README.md#-security-hall-of-fame-special-thanks)** pada README utama
- 🤝 Diundang sebagai kontributor proyek
- 📢 Mendapat ucapan terima kasih publik setelah perbaikan dirilis

> ℹ️ Saat ini kami **belum menyediakan program bug bounty berbayar**. Penghargaan diberikan dalam bentuk pengakuan publik.

---

## 🙏 Terima Kasih

Terima kasih telah membantu menjaga ThyoCloud tetap aman bagi seluruh komunitas.

---
---

# 🛡️ Security Policy (English)

[🇮🇩 Bahasa Indonesia](#️-kebijakan-keamanan-security-policy) | **🇬🇧 English**

The security of the ThyoCloud community is our priority. This document explains which versions are supported, how to report vulnerabilities, what we expect from reporters, and what you can expect from us.

## 📦 Supported Versions

| Version / Branch | Security Support |
|:---|:---:|
| `main` (latest) | ✅ Supported |
| Forks that are behind `main` | ❌ Not supported |

Security fixes are released on the `main` branch only. Please keep your fork in sync with our main branch.

## 🎯 Scope

**In scope:**

- The official website [thyo.cloud](https://thyo.cloud) and its API
- The Telegram bot `@ThyoCloudBot` (token verification and credential delivery)
- This repository, including GitHub Actions workflows
- Token creation, verification, and temporary credential storage/deletion flows

**Out of scope:**

- Weaknesses in third-party services (GitHub, Telegram, Railway, Cloudflare, etc.). Please report those to the vendor
- Denial of Service (DoS/DDoS), spam, or load testing
- Social engineering or phishing against admins or users
- Automated scanner output without a demonstrated real-world impact (proof of concept)
- Issues caused by users' own negligence, such as sharing tokens or RDP credentials
- Findings that require physical access to a user's device

## 🔍 Reporting a Vulnerability

> 🚨 **Please do NOT disclose vulnerabilities publicly — in GitHub Issues, Discussions, or community groups — before we have had a chance to fix them.**

We follow *Responsible Disclosure*. Report your findings privately via:

| Channel | Details |
|:---|:---|
| 💬 **Telegram (DM)** | [Contact the ThyoCloud Admin](https://t.me/thyocloud) — message an admin directly, not in the public group |

### 📝 What to Include

1. **Summary** of the vulnerability and the affected component (website, API, bot, workflow)
2. **Clear, repeatable steps** to reproduce
3. **Evidence** (proof of concept): screenshots, a short video, or request/response samples
4. **Impact** as you understand it (what data could leak, what access could be gained)
5. **Suggested fix** (optional, but appreciated)
6. **Name/alias** to be listed in the Hall of Fame (optional)

## ⏱️ What You Can Expect From Us

| Stage | Target Time |
|:---|:---:|
| 📬 Acknowledgement of your report | 24–48 hours |
| 🔎 Triage and initial validation | ~3–7 days |
| 🛠️ Fix (depends on severity) | Critical: as soon as possible · Others: based on complexity |
| 📢 Coordinated public disclosure | After the fix is released, agreed with the reporter |

We will keep you updated on progress. Please allow a reasonable time (up to **90 days** is suggested) to fix the issue before any public disclosure.

### 📊 Severity Levels

| Level | Examples |
|:---:|:---|
| 🔴 **Critical** | Leak of users' RDP credentials, account takeover, code execution on our infrastructure |
| 🟠 **High** | Token verification bypass, unauthorized access to user data or the admin panel |
| 🟡 **Medium** | Validation weaknesses with limited impact, disclosure of non-sensitive information |
| 🟢 **Low** | Minor misconfigurations, recommended hardening |

## 🤝 Safe Harbor

We will not pursue legal action against researchers who act in good faith and follow this policy. To stay within that protection, please:

- ✅ Test only **your own accounts and instances**
- ✅ Stop and report immediately if you accidentally access another user's data
- ✅ Do not download, copy, modify, or delete other users' data
- ✅ Do not disrupt service availability for other users
- ✅ Do not share your findings with others before they are fixed
- ❌ Do not use findings for personal gain or extortion

## 🔐 Data Handling Note

As stated in the [Transparency Notice](README.en.md#️-security--transparency) in the README: this RDP is a free, time-limited (max 6 hours), centrally managed service. A copy of credentials is stored **temporarily** for technical support and **automatically deleted** after the session expires. Any flaw related to storing or deleting this data is treated as **high priority**.

## 🏆 Recognition

We value every contribution. Reporters with valid findings may be:

- 🏅 Listed in the **[Security Hall of Fame](README.en.md#-security-hall-of-fame-special-thanks)** in the main README
- 🤝 Invited as a project contributor
- 📢 Publicly thanked once the fix is released

> ℹ️ We do **not currently run a paid bug bounty program**. Recognition is given in the form of public credit.

## 🙏 Thank You

Thank you for helping keep ThyoCloud safe for the whole community.
