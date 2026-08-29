Eleventy + Tailwind starter for Soumithri

Quick start (Windows):

1. Open a terminal in site/:
   cd "C:\Users\ADMIN\Desktop\Projects\website-v2\site"

2. Install dependencies:
   npm install @11ty/eleventy tailwindcss postcss autoprefixer --save-dev

3. Initialize Tailwind and build styles (one-time):
   npx tailwindcss -i ./src/styles/input.css -o ./_site/styles.css --watch

4. In a separate terminal, run Eleventy dev server:
   npx eleventy --serve

Eleventy will serve the generated site at http://localhost:8080 (default) and rebuild on changes.

Editing content:
- Homepage: src/index.md
- Blog posts: src/posts/*.md

When ready to publish, run:
  npx eleventy --output=_site

Then deploy the contents of _site/ to Netlify, Vercel (static) or GitHub Pages.

If you'd like, I can run the installs and start the dev server for you, or migrate sections from your old index.html into the new templates.
