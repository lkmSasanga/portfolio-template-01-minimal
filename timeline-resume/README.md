# Timeline Resume Portfolio

A beautiful, modern, and animated portfolio template featuring a stunning CSS-only timeline layout. Perfect for showcasing your experience, education, skills, and projects in an instantly impressive way.

![Portfolio Preview](https://via.placeholder.com/1200x600?text=Timeline+Resume+Portfolio+Preview)

## ✨ Features

- **CSS-Only Timeline Animation** - Smooth, impressive timeline animations without JavaScript
- **Fully Responsive** - Looks great on desktop, tablet, and mobile devices
- **Easy Customization** - Edit one CONFIG object to update all content
- **Modern Design** - Clean, minimal, recruiter-friendly interface
- **Accessible** - Semantic HTML, keyboard navigation, focus styles
- **Lightweight** - No frameworks or external dependencies
- **System Fonts** - Fast loading with native system fonts

## 🚀 Quick Start

1. **Clone or download this repository**
   ```bash
   git clone https://github.com/yourusername/timeline-resume-portfolio.git
   cd timeline-resume-portfolio
   ```

2. **Open `index.html` in your browser**
   - That's it! No build process, no dependencies to install.

3. **Customize your content**
   - Open `js/main.js`
   - Edit the `CONFIG` object with your information
   - See the [Customization Guide](#customization-guide) below

## 📝 Customization Guide (5 Minutes)

### Step 1: Update Personal Information

Open `js/main.js` and edit the `CONFIG` object:

```javascript
const CONFIG = {
    name: 'Your Name',
    role: 'Your Role',
    location: 'Your Location',
    email: 'your.email@example.com',
    summary: 'Your professional summary...',
    profileImage: 'assets/profile.png', // Circular profile image (150x150px or larger)
    heroImage: 'assets/hero.jpg', // Hero background image (1920x1080px recommended)
    // ... rest of the config
};
```

### Step 2: Add Your Skills

Update the `skills` object in `CONFIG`:

```javascript
skills: {
    'Top Skills': ['JavaScript', 'React', 'Node.js'],
    'Frontend': ['React', 'Vue.js', 'CSS3'],
    'Backend': ['Node.js', 'Python', 'PostgreSQL'],
    'Tools & Others': ['Git', 'Docker', 'AWS']
}
```

### Step 3: Add Timeline Items

Add your experience and education to the `timeline` array:

```javascript
timeline: [
    {
        type: 'experience', // or 'education'
        title: 'Job Title',
        organization: 'Company Name',
        date: '2022 - Present',
        location: 'City, State',
        description: [
            'Achievement or responsibility 1',
            'Achievement or responsibility 2'
        ],
        tags: ['React', 'TypeScript', 'Node.js']
    }
]
```

### Step 4: Add Projects

Update the `projects` array:

```javascript
projects: [
    {
        title: 'Project Name',
        description: 'Project description...',
        tech: ['React', 'Node.js'],
        links: [
            { label: 'Live Demo', url: 'https://...' },
            { label: 'GitHub', url: 'https://...' }
        ]
    }
]
```

### Step 5: Customize Colors

**Easy Method:** Simply change the primary color in one place! Open `css/styles.css` and find:

```css
--color-primary: #059669;  /* ← Change this one line */
```

See **[COLOR_GUIDE.md](COLOR_GUIDE.md)** for a complete guide with color examples and tips!

**Advanced:** Edit all CSS variables at the top of `css/styles.css`:

```css
:root {
    --color-primary: #2563eb;      /* Main brand color */
    --color-primary-dark: #1e40af;
    --color-accent: #0ea5e9;
    --color-text: #1e293b;
    /* ... more variables */
}
```

### Step 6: Add Your Images

1. **Profile Image** (`profile.png`):
   - Add your profile image to the `assets/` folder
   - Recommended: 150x150px or larger, square aspect ratio
   - The image will be automatically cropped to a circle
   - Or update the path in `CONFIG.profileImage`

2. **Hero Background Image** (`hero.jpg`):
   - Add a hero background image to the `assets/` folder
   - Recommended: 1920x1080px or larger, landscape orientation
   - This creates a stunning full-width background in the hero section
   - Choose images with good contrast for text readability
   - Or update the path in `CONFIG.heroImage`

## 🎨 Design Customization

### Colors

**Quick Color Change:** To change the primary color, simply edit **one line** in `css/styles.css`:

```css
--color-primary: #059669;  /* ← Change this to your color */
```

See **[COLOR_GUIDE.md](COLOR_GUIDE.md)** for detailed instructions and color examples!

All colors are defined as CSS variables in `css/styles.css`. Change them to match your brand:

- `--color-primary`: Main brand color (buttons, links, accents)
- `--color-accent`: Secondary accent color
- `--color-text`: Main text color
- `--color-bg`: Background color

### Spacing

Adjust spacing using the spacing variables:

```css
--spacing-xs: 0.5rem;
--spacing-sm: 1rem;
--spacing-md: 1.5rem;
--spacing-lg: 2rem;
--spacing-xl: 3rem;
--spacing-2xl: 4rem;
```

### Typography

The template uses system fonts for fast loading. To use custom fonts:

1. Add your font files to the `assets/` folder
2. Add `@font-face` declarations in `css/styles.css`
3. Update `--font-family` variable

## 📱 Responsive Breakpoints

- **Desktop**: Default styles (max-width: 1100px)
- **Tablet**: 768px and below
- **Mobile**: 480px and below

The timeline automatically adapts to smaller screens, becoming a single-column layout on mobile.

## 🚀 Deployment

This is a simple HTML/CSS template with no build process required, making deployment extremely easy and free!

**Recommended Free Hosting Options:**

- **[GitHub Pages](https://pages.github.com/)** - Free hosting directly from your GitHub repository
- **[Vercel](https://vercel.com/)** - Free deployment with drag-and-drop or Git integration
- **[Netlify](https://www.netlify.com/)** - Free hosting with continuous deployment

Simply push your code to GitHub and enable GitHub Pages, or drag and drop your folder to Vercel/Netlify. No configuration needed - it's that simple!

## 📂 Project Structure

```
timeline-resume-portfolio/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styles and animations
├── js/
│   └── main.js         # CONFIG object and rendering logic
├── assets/
│   ├── profile.png     # Your profile image (circular, 150x150px+)
│   └── hero.jpg        # Hero background image (1920x1080px recommended)
├── README.md           # This file
├── LICENSE             # MIT License
└── .gitignore          # Git ignore file
```

## 🎯 Key Features Explained

### Timeline Animation

The timeline features a CSS-only animation that:
- Draws the vertical line from top to bottom on page load
- Staggers the appearance of timeline items with fade-in and slide effects
- Respects `prefers-reduced-motion` for accessibility

### Skill Tags

Modern, pill-shaped skill tags with:
- Hover effects
- Category grouping
- Easy to scan and customize

### Navigation

- Sticky navigation bar
- Smooth scrolling to sections
- Active section highlighting using IntersectionObserver
- Mobile-friendly hamburger menu

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Credits

Built with the Timeline Resume Portfolio template. Feel free to use this template for your own portfolio!

## 💡 Tips

- **Keep it updated**: Regularly update your timeline and projects
- **Use real images**: Replace placeholder images with your own (both profile.png and hero.jpg)
- **Test on mobile**: Always preview your site on mobile devices
- **Optimize images**: Compress your profile image for faster loading
- **Add analytics**: Consider adding Google Analytics or similar

## 🐛 Troubleshooting

**Timeline not animating?**
- Check that CSS is loading properly
- Ensure JavaScript is enabled
- Check browser console for errors

**Images not showing?**
- Verify image paths are correct
- Check that images are in the `assets/` folder
- Ensure image filenames match exactly (case-sensitive)

**Styles not applying?**
- Clear browser cache
- Check that `css/styles.css` is linked correctly in `index.html`

## 📞 Support

If you encounter any issues or have questions:
1. Check this README first
2. Review the code comments in `js/main.js`
3. Open an issue on GitHub

---

## 🔧 Original Generation Prompt

This template was generated using the following Cursor prompt:

```text
You are an expert front-end developer and UI designer. Generate a complete, production-ready, beginner-friendly portfolio template repo.

GOAL
Build "Timeline Resume Portfolio" — a beautiful, modern, and animated portfolio template featuring a stunning CSS-only timeline layout.

Hook:
- CSS-only timeline animation that draws from top to bottom on page load
- Smooth, impressive animations without JavaScript dependencies

Wow features:
- CSS-only timeline animation with staggered item appearances
- Timeline layout for experience and education
- Easy customization through single CONFIG object

TECH + CONSTRAINTS
- Use ONLY vanilla HTML, CSS, and JavaScript
- No frameworks, no build tools, no external libraries
- Simple, readable code for beginners
- Fully responsive (mobile, tablet, desktop)
- Accessible: semantic HTML, keyboard navigation, focus states
- Performance-focused: lightweight, CSS-only animations
- Use system font stack only

REPO STRUCTURE
/
  index.html
  css/
    styles.css
  js/
    main.js
  assets/
    profile.png (circular profile image)
    hero.jpg (hero background image)
  README.md
  LICENSE (MIT)
  .gitignore
  COLOR_GUIDE.md

DESIGN REQUIREMENTS
- Clean, modern, recruiter-friendly interface
- CSS-only timeline with vertical line animation
- Max width ~ 1100px centered
- Sections:
  1) Sticky header with navigation
  2) Hero section (with profile image and background image)
  3) Skills section (grouped by category with tags)
  4) Timeline section (experience and education items)
  5) Projects section (project cards with links)
  6) Contact section (email and social links)
  7) Footer

TIMELINE FEATURE (MAIN FEATURE)
- Vertical timeline layout with:
  - Animated vertical line that draws on page load
  - Timeline items (experience/education) on alternating sides
  - Staggered fade-in and slide animations for items
  - Responsive: single column on mobile
- Timeline items include:
  - Type (experience/education)
  - Title and organization
  - Date and location
  - Description (bullet points)
  - Tags (technology stack)

TIMELINE ANIMATION
- CSS-only implementation:
  - Vertical line animates from top to bottom using CSS animations
  - Timeline items fade in with staggered delays
  - Smooth slide-in effects
  - Respects prefers-reduced-motion for accessibility
- No JavaScript required for animations

REUSABILITY (VERY IMPORTANT)
Make customization extremely easy:

- Add a big "EDIT HERE" comment block in index.html
- In js/main.js define a CONFIG object:

{
  name: "Your Name",
  role: "Your Role",
  location: "Your Location",
  email: "your.email@example.com",
  summary: "Your professional summary...",
  profileImage: "assets/profile.png",
  heroImage: "assets/hero.jpg",
  social: [
    { name: "GitHub", url: "...", icon: "..." },
    { name: "LinkedIn", url: "...", icon: "..." }
  ],
  skills: {
    "Top Skills": ["JavaScript", "React", "Node.js"],
    "Frontend": ["React", "Vue.js", "CSS3"],
    "Backend": ["Node.js", "Python", "PostgreSQL"]
  },
  timeline: [
    {
      type: "experience",
      title: "Job Title",
      organization: "Company Name",
      date: "2022 - Present",
      location: "City, State",
      description: ["Achievement 1", "Achievement 2"],
      tags: ["React", "TypeScript"]
    }
  ],
  projects: [
    {
      title: "Project Name",
      description: "Project description...",
      tech: ["React", "Node.js"],
      links: [
        { label: "Live Demo", url: "https://..." },
        { label: "GitHub", url: "https://..." }
      ]
    }
  ]
}

- Render all content from this CONFIG object
- Users should only edit this config to update content

RESPONSIVE BEHAVIOR
- Timeline:
  - Alternating sides on desktop (left/right)
  - Single column on mobile/tablet
  - Smooth transitions between breakpoints
- Navigation: hamburger menu on mobile
- All sections stack vertically on mobile

STYLING
- Use CSS variables for colors, spacing, radius
- Light theme by default
- Subtle transitions only
- CSS-only animations (no JavaScript for animations)

NAV + UX
- Sticky navigation bar
- Smooth scroll navigation
- Active link highlight on scroll (IntersectionObserver)
- Mobile-friendly hamburger menu
- Skip to main content link for accessibility

COLOR CUSTOMIZATION
- Create COLOR_GUIDE.md with:
  - Instructions to change primary color in one line
  - Color examples and combinations
  - Tips for choosing colors

README.md REQUIREMENTS
Include:
- Overview + screenshot placeholder
- Quick start (open index.html)
- Customization guide:
  - Edit CONFIG object
  - Change CSS variables
  - Add images
- How timeline animation works
- Deploy guide (GitHub Pages)
- MIT license note
- Original generation prompt section

DELIVERABLE
Output full contents of:
- index.html
- css/styles.css
- js/main.js
- README.md
- LICENSE
- .gitignore
- COLOR_GUIDE.md

EXTRA
- Keep UI premium but code simple
- No unnecessary complexity
- Everything in a single page
- CSS-only animations for performance
```

---

**Made with ❤️ for developers who want a beautiful portfolio without the complexity.**

