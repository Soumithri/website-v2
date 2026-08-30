# Soumithri's Personal Website & Blog

A personal website and blog for **soumithri93.com**, built with [Eleventy](https://www.11ty.dev/) (static site generator) and [Tailwind CSS](https://tailwindcss.com/).

## 🚀 How it works

This is a **static site** — no server, no database. You write content as plain **Markdown**, and an automated build turns it into fast HTML files that get deployed to **GitHub Pages**.

**Your workflow:**
1. Write a blog post as a Markdown file in `site/src/posts/`
2. Commit and push to `main`
3. GitHub Actions automatically builds and deploys the site
4. Live at `https://www.soumithri93.com`

No coding required — just write Markdown and push.

## 📁 Project structure

```
website-v2/
└── site/                        # The Eleventy site (source of truth)
    ├── .eleventy.js             # Eleventy config
    ├── package.json             # Build scripts & dependencies
    ├── .github/workflows/deploy.yml  # Auto-deploy to GitHub Pages
    └── src/
        ├── index.md             # Homepage
        ├── work.md              # Work page
        ├── research.md          # Research page
        ├── contact.md           # Contact page (with form)
        ├── blog/index.md        # Blog listing page
        ├── posts/               # ← Write blog posts here (Markdown)
        │   └── welcome.md       # Example post
        ├── _includes/           # Layouts & partials (HTML templates)
        └── styles/input.css     # Tailwind + custom styles
```

## ✍️ Writing a blog post

1. Create a new file in `site/src/posts/`, e.g. `my-new-post.md`
2. Add front matter at the top:
   ```markdown
   ---
   layout: layouts/post.njk
   title: "My Post Title"
   date: 2026-08-30
   displayDate: "30 AUG 2026"
   ---
   ```
3. Write your content in Markdown below the front matter
4. Commit and push — the site auto-deploys

## 🛠 Local development

```bash
cd site
npm install
npm run dev        # starts dev server at http://localhost:8080
```

To build a production version:

```bash
cd site
npm run build      # outputs to site/_site/
```

## 🌐 Deployment

Deployment is fully automated via **GitHub Actions** (see `.github/workflows/deploy.yml`). Every push to `main` triggers a build and deploy to **GitHub Pages**.

The custom domain `www.soumithri93.com` is configured via the `CNAME` file in `site/src/`.

## 📧 Contact form

The contact form uses [Formspree](https://formspree.io/) to deliver submissions to your email. To activate it:
1. Create a free form at formspree.io
2. Replace the form ID in `site/src/contact.md` (`https://formspree.io/f/your-form-id`)

## 📄 License

Personal project. Free to use and modify.
