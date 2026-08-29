# Soumithri's Portfolio Website

A modern, clean, and responsive personal portfolio website built with HTML, CSS, and JavaScript.

## 🚀 Features

- **Responsive Design** - Looks great on all devices (mobile, tablet, desktop)
- **Modern UI** - Clean and professional design with gradient accents
- **Smooth Animations** - Fade-in effects and hover animations
- **Portfolio Section** - Showcase your best projects
- **Blog Section** - Share your thoughts and knowledge
- **About Section** - Tell your story
- **Contact Form** - Let visitors get in touch
- **Mobile Menu** - Hamburger menu for mobile devices
- **Fast Loading** - Lightweight and optimized

## 📁 Project Structure

```
website-v2/
├── index.html          # Main homepage
├── styles.css          # Global styles
├── script.js           # JavaScript interactivity
└── blog/
    ├── post1.html      # Sample blog post 1
    ├── post2.html      # Sample blog post 2
    ├── post3.html      # Sample blog post 3
    └── blog.css        # Blog-specific styles
```

## 🎨 Customization Guide

### 1. Update Your Information

**In `index.html`:**
- Replace "Soumithri" with your name
- Update the tagline in the hero section
- Modify skills, social links, and about text

**Update Social Links:**
```html
<a href="https://github.com/yourprofile" target="_blank">
    <i class="fab fa-github"></i> GitHub
</a>
```

### 2. Add Your Projects

Replace the three sample projects in the "Work" section:
```html
<div class="work-card">
    <div class="work-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);"></div>
    <div class="work-content">
        <h3>Your Project Name</h3>
        <p>Your project description</p>
        <div class="tags">
            <span>Technology</span>
            <span>Framework</span>
        </div>
        <a href="your-project-link" class="work-link">View Project →</a>
    </div>
</div>
```

### 3. Add More Blog Posts

Create new HTML files in the `blog/` folder following the structure of `post1.html`, `post2.html`, and `post3.html`.

Then update the blog cards in `index.html`:
```html
<article class="blog-card">
    <div class="blog-meta">
        <span class="date">Your Date</span>
        <span class="read-time">X min read</span>
    </div>
    <h3>Your Blog Post Title</h3>
    <p>Your post summary</p>
    <a href="blog/your-post.html" class="read-more">Read More →</a>
</article>
```

### 4. Customize Colors

Edit the CSS variables in `styles.css`:
```css
:root {
    --primary: #667eea;      /* Main brand color */
    --secondary: #764ba2;    /* Secondary color */
    --accent: #f5576c;       /* Accent color */
    /* ... other colors ... */
}
```

### 5. Update Meta Information

In `index.html`, update:
```html
<title>Your Name - Portfolio</title>
```

### 6. Add Favicon

Add a favicon to the `<head>` section:
```html
<link rel="icon" type="image/png" href="favicon.png">
```

## 📱 Responsive Breakpoints

- **Mobile**: 480px and below
- **Tablet**: 481px - 768px
- **Desktop**: 769px and above

## 🔧 Features to Enhance

### 1. **Contact Form Integration**
Currently shows a confirmation alert. To make it functional:
- Use a backend service like Formspree, Netlify Forms, or SendGrid
- Or use a static site service like Vercel or Netlify with built-in form handling

### 2. **Dark Mode**
Add a dark mode toggle by implementing additional CSS and JavaScript:
```css
body.dark-mode { /* dark styles */ }
```

### 3. **Search Functionality**
Add a search feature for blog posts as your collection grows.

### 4. **Dynamic Content Loading**
Use JavaScript or a static site generator to load content dynamically.

### 5. **Performance Optimization**
- Optimize images using tools like TinyPNG
- Minify CSS and JavaScript
- Use a CDN for faster delivery

## 🚢 Deployment Options

### Netlify (Recommended for beginners)
1. Push code to GitHub
2. Connect GitHub to Netlify
3. Deploy with automatic updates on push

### Vercel
1. Connect your GitHub repository
2. Deploy with one click
3. Automatic deployments on push

### GitHub Pages
1. Push code to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Access at `username.github.io`

### Traditional Hosting
Upload files via FTP to your hosting provider.

## 📝 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📄 License

This template is free to use for personal projects. Modify and customize as needed!

## 💡 Tips

1. **Update regularly** - Keep your portfolio fresh with new projects and blog posts
2. **Test on devices** - Always test on real phones and tablets
3. **Keep it clean** - Avoid cluttering; less is more
4. **Mobile first** - Design for mobile, then enhance for desktop
5. **Fast loading** - Optimize images and minimize external requests

## 🤝 Contributing

Feel free to customize and improve this template!

## 📧 Need Help?

Check the inline comments in the code for additional guidance and explanations.

---

Happy coding! 🎉
