# Harsha

## About This Blog

This blog is built with Jekyll using the beautiful [Chirpy theme][chirpy]. Here's what you'll find:

- **📚 Book Reviews & Insights**: Deep dives into self-help and personal development books
- **💻 Programming Discoveries**: Tips and learnings from working with C#, C++, and AI tools
- **🤖 AI Tools & Productivity**: How I leverage artificial intelligence in my daily workflow
- **📖 Light Novel Reviews**: Occasional thoughts on Xianxia light novels
- **🎯 Personal Growth**: Reflections on applying lessons from books to real life

Welcome to the source code of my personal blog! This is where I share insights from self-help books I read, programming discoveries, AI tools, and other interesting things I come across in my journey as a Software Engineer at Microsoft.

🌐 **Live Site**: [https://saiharshak.github.io](https://saiharshak.github.io)

When installing the [**Chirpy**][chirpy] theme through [RubyGems.org][gem], Jekyll can only read files in the folders
`_data`, `_layouts`, `_includes`, `_sass` and `assets`, as well as a small part of options of the `_config.yml` file
from the theme's gem. If you have ever installed this theme gem, you can use the command
`bundle info --path jekyll-theme-chirpy` to locate these files.

The Jekyll team claims that this is to leave the ball in the user’s court, but this also results in users not being
able to enjoy the out-of-the-box experience when using feature-rich themes.

## 🚀 Local Development Setup

### Prerequisites
- Ruby (3.1 or higher)
- Bundler gem
- Git

### Installation & Running Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/SaiHarshaK/saiharshak.github.io.git
   cd saiharshak.github.io
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the development server**
   ```bash
   bundle exec jekyll serve
   ```
   Or use the provided script:
   ```bash
   ./tools/run.sh
   ```

4. **Open your browser**
   Navigate to `http://localhost:4000` to see the site locally.

### Building for Production
```bash
bundle exec jekyll build
```
Or use the test script:
```bash
./tools/test.sh
```

## 🌐 GitHub Pages Deployment

This blog is automatically deployed to GitHub Pages using GitHub Actions. Here's how it works:

### Automatic Deployment
1. **Push to main branch** - Any commit to the `main` branch triggers automatic deployment
2. **GitHub Actions** - The site is built and deployed using Jekyll GitHub Actions
3. **Live in minutes** - Changes appear at [saiharshak.github.io](https://saiharshak.github.io) within a few minutes

### Manual Setup (if needed)
1. Go to your repository **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. The Jekyll workflow should be automatically detected

### Custom Domain (Optional)
To use a custom domain:
1. Add your domain to **Settings** → **Pages** → **Custom domain**
2. Update the `url` field in `_config.yml`
3. Create a `CNAME` file in the root directory with your domain

## 📁 Repository Structure

```
├── _posts/              # Blog posts
├── _tabs/               # Sidebar navigation pages
├── _data/               # Site data (authors, contact info, etc.)
├── _includes/           # Reusable HTML components
├── _layouts/            # Page layouts
├── _sass/               # Stylesheets
├── assets/              # Images, CSS, JS files
├── tools/               # Build and development scripts
├── _config.yml          # Site configuration
└── README.md           # This file
```

## ✍️ Writing Posts

Create new posts in the `_posts/` directory with the naming convention:
```
YYYY-MM-DD-title-of-post.md
```

Each post should have front matter like:
```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS +0530
categories: [Category1, Category2]
tags: [tag1, tag2]
author: harsha
---
```

## 🛠️ Customization

- **Site settings**: Edit `_config.yml`
- **About page**: Edit `_tabs/about.md`
- **Contact info**: Edit `_data/contact.yml`
- **Author info**: Edit `_data/authors.yml`

## 📚 Theme Documentation

For more advanced customization and features, check out the [Chirpy theme documentation](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

## License

This project is open source and available under the [MIT License][mit].

---

**Built with ❤️ using Jekyll and the Chirpy theme**

[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[mit]: https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE
