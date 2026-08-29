# Quick Start Guide - Getting Your Portfolio Live

## Step 1: Local Testing

1. Open `index.html` in your web browser to preview the site locally
2. Test all sections: Home, Work, Blog, About, and Contact
3. Check responsiveness by resizing your browser window

## Step 2: Customize Your Information

### Edit `index.html`:
1. Replace all instances of "Soumithri" with your name
2. Update the hero tagline to your own
3. Modify the "About Me" section with your story
4. Update the skills list
5. Replace social media links with your own profiles

### Edit `config.json`:
1. Update your personal information
2. Customize colors if desired
3. Update social media links
4. Add/modify your projects and blog posts

## Step 3: Add Your Projects

Replace the sample projects in the "Featured Work" section:
- Update project titles and descriptions
- Change gradient colors for project images
- Update technologies/tags
- Add real project links

## Step 4: Create Blog Posts

1. Create new files in the `blog/` folder (e.g., `post4.html`)
2. Copy the structure from `post1.html`, `post2.html`, or `post3.html`
3. Write your content
4. Update the blog card in `index.html` to link to your new post

## Step 5: Deploy to Production

### Option A: Netlify (Easiest)

1. Push your code to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio commit"
   git push origin main
   ```

2. Visit [netlify.com](https://netlify.com)
3. Click "New site from Git"
4. Connect your GitHub repository
5. Click Deploy
6. Add your domain in Site Settings

### Option B: Vercel

1. Push your code to GitHub
2. Visit [vercel.com](https://vercel.com)
3. Import your repository
4. Click Deploy
5. Add your custom domain

### Option C: Your Hosting Provider

1. Upload all files via FTP or file manager
2. Ensure `index.html` is in the root directory
3. Point your domain to the hosting provider's nameservers

## Step 6: Connect Your Domain

For `soumithri93.com`:
1. Go to your domain registrar (GoDaddy, Namecheap, etc.)
2. Find DNS settings
3. Update nameservers or A records to point to your hosting
4. Wait 24-48 hours for DNS to propagate

## Common Customizations

### Change Color Scheme

Edit `styles.css`, look for the `:root` section:
```css
:root {
    --primary: #667eea;      /* Change this */
    --secondary: #764ba2;    /* And this */
    --accent: #f5576c;       /* And this */
}
```

### Update Navigation Links

Edit the `<nav>` section in `index.html` to add/remove menu items.

### Modify Contact Form

Currently, the form shows an alert. To make it work:
- **Netlify**: Forms work automatically once deployed
- **Formspree**: Use `<form action="https://formspree.io/f/YOUR_ID" method="POST">`
- **Email.js**: Add the Email.js library and update `script.js`

### Add a Favicon

1. Create or download a favicon (16x16, 32x32, or 64x64 pixels)
2. Save it as `favicon.png` in the root directory
3. Add this to the `<head>` of `index.html`:
   ```html
   <link rel="icon" type="image/png" href="favicon.png">
   ```

## Performance Tips

1. **Optimize Images**
   - Use tools like TinyPNG to compress images
   - Use WebP format for faster loading

2. **Minify Code**
   - Use online minifiers for CSS and JavaScript
   - Or use build tools like Webpack

3. **Use a CDN**
   - Netlify and Vercel provide built-in CDN
   - Cloudflare offers free CDN services

## SEO Optimization

Add these meta tags to `<head>` in `index.html`:
```html
<meta name="description" content="Your professional portfolio">
<meta name="keywords" content="developer, portfolio, web design">
<meta name="author" content="Your Name">
<meta property="og:title" content="Your Name - Portfolio">
<meta property="og:description" content="Your professional portfolio">
<meta property="og:image" content="your-image-url">
```

## Troubleshooting

**Blog posts don't load:**
- Check that file paths in blog card links match your file structure
- Ensure all files are uploaded/committed

**Styles look broken:**
- Clear browser cache (Ctrl+Shift+Del)
- Check that all CSS files are linked correctly

**Form doesn't work:**
- Use Netlify Forms or Formspree for email functionality
- Test in browser console (F12) for JavaScript errors

**Mobile menu doesn't work:**
- Check that `script.js` is linked in `index.html`
- Verify no JavaScript errors in console

## Next Steps

1. ✅ Customize your information
2. ✅ Add your projects
3. ✅ Write blog posts
4. ✅ Test locally
5. ✅ Deploy to production
6. ✅ Set up your domain
7. ✅ Monitor analytics (optional: add Google Analytics)

## Keep Your Portfolio Fresh

- Add new projects as you complete them
- Write blog posts regularly
- Update your skills as you learn new technologies
- Keep the design modern and relevant

## Support & Resources

- **Documentation**: Check README.md for detailed information
- **Code Comments**: Read through index.html, styles.css, and script.js for inline comments
- **Deployment Help**: Consult Netlify or Vercel documentation

---

**Ready to launch? Start customizing and get your portfolio online! 🚀**
