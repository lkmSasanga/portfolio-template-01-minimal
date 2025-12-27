# Project Case-Study Portfolio

A clean, modern, single-page portfolio template that showcases your projects as detailed case studies. Perfect for developers and designers who want a professional portfolio without the complexity of frameworks or build tools.

![Portfolio Template](screenshot.png)

## ✨ Features

- **Single-page design** - All content on one page, no routing needed
- **Case study layout** - Project cards expand into detailed case studies with problem/solution/impact format
- **Fully responsive** - Mobile, tablet, and desktop optimized
- **Accessible** - Semantic HTML, keyboard navigation, ARIA labels
- **Performance-focused** - Vanilla JavaScript, no dependencies, lightweight
- **Easy to customize** - Edit one array to update all projects
- **Modern UI** - Clean, product-style design with smooth interactions

## 🚀 Quick Start

1. Clone or download this repository
2. Open `index.html` in your browser
3. That's it! No build process or dependencies required.

## 📁 Project Structure

```
/
  index.html          # Main HTML file
  css/
    styles.css        # All styles (customize colors & spacing here)
  js/
    main.js           # JavaScript logic (edit PROJECTS array here)
  assets/
    project-1.jpg     # Project images (replace with your own)
    project-2.jpg
    project-3.jpg
  README.md
  LICENSE
  .gitignore
```

## 🎨 Customization Guide

### Adding/Editing Projects

Open `js/main.js` and find the `PROJECTS` array. Update it with your own project data:

```javascript
const PROJECTS = [
    {
        id: "project-1",                    // Unique ID
        title: "Your Project Name",          // Project title
        shortDesc: "Brief description...",   // Shown on card
        image: "assets/project-1.jpg",       // Image path
        tech: ["React", "Node.js"],          // Tech stack tags
        problem: "The problem statement...",
        solution: "How you solved it...",
        features: [
            "Feature 1",
            "Feature 2",
            // Add more features
        ],
        results: "Results and impact metrics...",
        liveLink: "https://yourproject.com",  // Live demo URL
        repoLink: "https://github.com/..."    // GitHub repo URL
    },
    // Add more projects...
];
```

**Tips:**
- Add as many projects as you want
- Images should be at least 800px wide for best quality
- Use realistic, impactful metrics in your results section
- Keep short descriptions concise (1-2 sentences)

### Changing Colors & Spacing

Open `css/styles.css` and find the `:root` section at the top. Update the CSS variables:

```css
:root {
    /* Colors */
    --color-primary: #2563eb;        /* Primary brand color */
    --color-primary-dark: #1e40af;   /* Darker shade for hover */
    --color-text: #1e293b;           /* Main text color */
    --color-bg: #ffffff;             /* Background color */
    
    /* Spacing */
    --spacing-md: 1.5rem;            /* Default spacing */
    --spacing-xl: 3rem;              /* Large spacing */
    
    /* Typography */
    --font-size-lg: 1.5rem;          /* Large text size */
    
    /* Layout */
    --container-width: 1000px;       /* Max content width */
}
```

### Updating Personal Information

1. **Header/Navigation**: Edit the logo text in `index.html`:
   ```html
   <a href="#home" class="nav__logo">Your Name</a>
   ```

2. **Hero Section**: Update the hero text in `index.html`:
   ```html
   <h1 class="hero__title">Your Headline</h1>
   <p class="hero__description">Your description...</p>
   ```

3. **About Section**: Update your bio and skills in `index.html`

4. **Contact Section**: Update email and social links in `index.html`:
   ```html
   <a href="mailto:your.email@example.com">your.email@example.com</a>
   ```

5. **Footer**: Update copyright text in `index.html`

6. **Meta Tags**: Update the `<title>` and `<meta name="description">` in the `<head>` section

### Adding Project Images

1. Add your project images to the `assets/` folder
2. Name them consistently (e.g., `project-1.jpg`, `project-2.jpg`)
3. Update the `image` property in the `PROJECTS` array to match your filenames
4. Recommended size: 1200x800px (3:2 ratio) for best results

## 🌐 Deployment

### GitHub Pages

1. Push your repository to GitHub
2. Go to **Settings** → **Pages**
3. Select the branch (usually `main` or `master`)
4. Select `/ (root)` as the source folder
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/repository-name`

### Other Hosting Options

- **Netlify**: Drag and drop the folder to Netlify Drop
- **Vercel**: Connect your GitHub repo or deploy via CLI
- **Any static hosting**: Upload all files to any web server

No build step required - just upload the files as-is!

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

Uses modern CSS features like CSS Grid and Flexbox. Gracefully degrades in older browsers.

## 🎯 Best Practices

### Writing Case Studies

Follow this structure for compelling case studies:

1. **Problem**: Define the challenge clearly
2. **Solution**: Explain your approach and design decisions
3. **Features**: List key functionality and highlights
4. **Results**: Include metrics and impact (use real data when possible)

### Image Optimization

- Use WebP or optimized JPG/PNG formats
- Aim for file sizes under 200KB per image
- Use appropriate dimensions (don't use massive images)

### Performance Tips

- Lazy load images (already implemented)
- Keep project descriptions concise
- Optimize your images before adding them

## 📄 License

MIT License - feel free to use this template for personal or commercial projects.

## 🤝 Contributing

This is a template repository, but if you find bugs or have suggestions:
1. Fork the repository
2. Make your changes
3. Submit a pull request

## 💡 Tips for Beginners

- Start by editing the `PROJECTS` array - it's the easiest way to see changes
- Use browser DevTools (F12) to inspect and understand the CSS
- Don't worry about getting everything perfect - iterate and improve over time
- Replace placeholder images before sharing your portfolio

## 📞 Support

For issues or questions:
- Open an issue on GitHub
- Check the code comments (marked with `EDIT HERE`) for guidance

---

**Perfect for dev/design portfolios & case studies.** Made with ❤️ using vanilla HTML, CSS, and JavaScript.

