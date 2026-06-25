#Digital Garden 🌿

**A clean, minimalist Jekyll-powered personal knowledge base and digital garden.**  
It combines thoughtful technical writing with practical tools — including a high-security PDF management and decryption system.

**Live Site**: [https://blueflylabor.github.io/](https://blueflylabor.github.io/)

---

## ✨ Project Highlights

### 📂 PDF Secure Cabinet (High-Performance Tool)
A fully static, client-side PDF file management and secure decryption system located at `/filestore/`.

**Core Capabilities:**
- **Static File Cabinet**: Automatic listing of public PDFs with modal preview (PDF.js), one-click download, and absolute URL copying.
- **High-Security Decrypt Viewer**: Perfect alignment with OpenSSL 3.x using AES-256-CBC, PBKDF2-SHA512, and 204,800 iterations.
- Robust frontend decryption (CryptoJS) with fixes for key/IV derivation issues.
- URL-based direct access: `?f=filename.enc&k=yourpassword`
- Smooth UX with auto-scroll during long decryption and high-DPI Retina rendering.
- Multilingual support (Chinese, English, German).

**Recommended Encryption Command:**
```bash
openssl enc -aes-256-cbc -salt -pbkdf2 -iter 204800 -md sha512 \
  -in yourfile.pdf -out yourfile.enc -k "yourpassword"
```

**Access**: [Open PDF Secure Cabinet →](https://blueflylabor.github.io/filestore/)

---

## 🚀 Site Structure (2026 Rebuild)

The site is organized into four main pillars:

- **Notes**: Core technical documentation (Distributed Systems, Databases, Python, macOS, etc.)
- **Insights**: Deep analysis and logical deconstruction of complex topics
- **Solutions**: Practical, step-by-step troubleshooting guides
- **Archive**: Historical records and legacy materials

---

## ✨ Key Features

- **Minimalist & Readable Design**: Focused on content clarity with no unnecessary visual noise
- **Jekyll Static Site**: Blazing-fast generation and native GitHub Pages deployment
- **Bilingual Automation**: Chinese ↔ English content with Python-powered translation workflow
- **Rich Content Support**:
  - MathJax for mathematics
  - Mermaid for diagrams
  - Syntax highlighting
  - Full Markdown extensions
- **Search Functionality**: Fast client-side search
- **Responsive & Modern**: Excellent experience on all devices
- **PDF Management Suite**: Public cabinet + enterprise-grade client-side encryption/decryption tool
- **SEO Optimized**: Meta tags, sitemap, and clean URLs
- **Automation Ready**: Python scripts for content processing and translation

---

## 🛠️ Quick Start (Local Development)

### Prerequisites
- Ruby + Bundler, or Docker (recommended)

### Using Bundler
```bash
git clone https://github.com/blueflylabor/blueflylabor.github.io.git
cd blueflylabor.github.io
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`

### Using Docker
```bash
docker-compose up
```

---

## 📁 Project Structure

```
blueflylabor.github.io/
├── _posts/              # Blog posts & notes
├── _pages/              # Static pages
├── filestore/           # PDF management system
│   ├── files/           # Public PDFs
│   ├── encrypted/       # Encrypted files
│   ├── cabinet/         # Public file cabinet
│   └── decrypt/         # Secure decryption viewer
├── _layouts/            # HTML layouts
├── _includes/           # Reusable components
├── _sass/               # Styles (Sass)
├── assets/              # JS, CSS, images
├── _config.yml          # Site configuration
├── translate.py         # Translation automation
├── Gemfile
├── docker-compose.yml
└── README.md
```

---

## 🧩 Customization

- Edit `_config.yml` for site title, author, language, etc.
- Add new posts in `_posts/` using `YYYY-MM-DD-title.md`
- Place public PDFs in `filestore/files/`
- Place encrypted files in `filestore/encrypted/`
- Customize styles in `_sass/`
- Extend languages in the JavaScript i18n dictionaries

---

## 🛠️ Tech Stack

- **Static Site Generator**: Jekyll
- **Theme**: Customized Jekyll-Paper / Minimalist
- **Styling**: Sass + Flexbox + Modern CSS
- **Frontend Tools**: CryptoJS, PDF.js, custom high-DPI rendering
- **Automation**: Python scripts + GitHub Actions
- **Hosting**: GitHub Pages
- **Search**: Client-side JSON index

---

## Security Note (PDF Tool)

All decryption occurs **entirely in the browser**. No data or passwords are transmitted to any server. The system is designed for maximum security on static hosting.

---

## Deployment

1. Push to the `main` branch
2. Enable GitHub Pages in repository settings
3. Site will be live at `https://blueflylabor.github.io/`

---

## License

This project is open source under the [MIT License](LICENSE).

---

**Made with ❤️ for clarity, security, and continuous learning.**
