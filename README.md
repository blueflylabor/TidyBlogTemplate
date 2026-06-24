# TidyBlogTemplate

A clean, minimal, and highly customizable Jekyll template for building personal blogs, digital gardens, and knowledge bases. Perfect for developers, researchers, and writers who value content clarity over visual noise.

![Demo](https://blueflylabor.github.io/)

## ✨ Features

- **Minimalist Design**: Elegant, distraction-free layout focused on readability and content consumption.
- **Jekyll-Powered**: Built with Jekyll for fast static site generation and seamless GitHub Pages deployment.
- **Responsive & Modern**: Mobile-first design that looks great on all devices.
- **Powerful Content Organization**:
  - Categories and tags support
  - Archive pages
  - Pagination
  - Search functionality
- **Rich Content Support**:
  - Mathematics rendering with MathJax
  - Interactive diagrams with Mermaid
  - Syntax highlighting for code blocks
  - Markdown extensions (tables, footnotes, etc.)
- **Bilingual Ready**: Easy setup for multilingual content with automation support.
- **Comment System Ready**: Integrated support for Gitalk and other comment systems.
- **SEO Optimized**: Built-in SEO tags and sitemap generation.
- **Analytics Integration**: Easy Google Analytics setup.
- **Docker Support**: Run locally with Docker Compose for consistent development.
- **Automation Friendly**: Includes Python scripts for content processing and translation workflows.

## 🚀 Quick Start

### Prerequisites

- Ruby + Bundler
- Or Docker (recommended for simplicity)

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/blueflylabor/TidyBlogTemplate.git
   cd TidyBlogTemplate
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Serve locally**
   ```bash
   bundle exec jekyll serve
   ```

   Visit `http://localhost:4000`

### Using Docker

```bash
docker-compose up
```

## 📁 Project Structure

```
TidyBlogTemplate/
├── _posts/           # Blog posts (Markdown)
├── _pages/           # Static pages
├── _layouts/         # HTML layouts
├── _includes/        # Reusable components
├── _sass/            # Stylesheets
├── assets/           # Images and other static files
├── _config.yml       # Main configuration
├── Gemfile           # Ruby dependencies
└── translate.py      # Content automation scripts
```

## 🛠️ Customization

### Site Configuration

Edit `_config.yml` to set:

- Site title, description, and author info
- Base URL and domain
- Language preferences
- Pagination settings
- Analytics and comment system keys

### Adding Content

Create new posts in the `_posts` directory following the naming convention:

```
YYYY-MM-DD-your-post-title.md
```

### Styling

Customize colors and typography by modifying files in the `_sass` directory.

## 🧩 Supported Features

- **Full Markdown Support** with Jekyll extensions
- **Math & Diagrams**: MathJax and Mermaid integration
- **Archives**: Automatic category, tag, and date-based archives
- **Search**: Client-side search capabilities
- **RSS Feed**: Automatic feed generation
- **Sitemap**: SEO-friendly sitemap
- **404 Page**: Custom error page
- **Dark Mode Ready**: Foundation for theme switching

## Deployment

### GitHub Pages (Recommended)

1. Push your changes to the `main` branch
2. Enable GitHub Pages in repository settings
3. Your site will be live at `https://yourusername.github.io`

## Tech Stack

- **Static Site Generator**: Jekyll
- **Styling**: Sass
- **Markdown Processor**: Redcarpet
- **Deployment**: GitHub Pages
- **Development**: Docker Compose

## License

This project is open source and available under the [MIT License](LICENSE).

---

**Live Demo**: [https://blueflylabor.github.io/](https://blueflylabor.github.io/)

Made with ❤️ for clean content and thoughtful writing.