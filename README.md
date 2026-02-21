# Ramji Pal - Personal Portfolio Website

A modern, fully responsive personal portfolio website for a ServiceNow Developer.

## 🚀 Features

- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Dark/Light Theme Toggle**: User preference saved in localStorage
- **Smooth Animations**: Scroll-based animations and hover effects
- **Modern UI Design**: Clean, professional design with gradient accents
- **Interactive Elements**: Dynamic navigation, contact form, and smooth scrolling
- **Performance Optimized**: Fast loading and efficient animations

## 📁 Project Structure

```
portfolio/
├── index.html          # Main HTML file with all sections
├── styles.css          # Complete styling with responsive design
├── script.js           # JavaScript for interactivity
└── README.md          # This file
```

## 🎨 Sections Included

1. **Hero Section** - Introduction with name, title, and CTA buttons
2. **About Me** - Professional summary and certifications
3. **Skills** - Categorized skills with progress bars
4. **Experience** - Timeline of professional experience
5. **Projects** - Featured projects with detailed descriptions
6. **Certifications** - ServiceNow and Microsoft certifications
7. **Contact** - Contact information and form

## 🛠️ Customization Guide

### Update Personal Information

**Contact Details** (in `index.html`):
- Line 468: Update email address
- Line 476: Update phone number
- Line 484: Update LinkedIn URL
- Line 492: Update GitHub URL

### Add Your Photo

Replace the placeholder icon in the About section:
```html
<!-- Find this in index.html around line 122 -->
<div class="image-placeholder">
    <i class="fas fa-user"></i>
</div>

<!-- Replace with: -->
<img src="your-photo.jpg" alt="Ramji Pal" style="width: 280px; height: 280px; border-radius: 50%; object-fit: cover;">
```

### Add Resume Download

1. Add your resume PDF to the portfolio folder (e.g., `ramji-pal-resume.pdf`)
2. Update the download button in `script.js` (line 116):
```javascript
downloadResumeBtn.addEventListener('click', function(e) {
    e.preventDefault();
    // Replace with actual resume file
    window.open('ramji-pal-resume.pdf', '_blank');
});
```

### Customize Colors

Update CSS variables in `styles.css` (lines 1-15):
```css
:root {
    --primary-color: #3b82f6;      /* Main blue color */
    --secondary-color: #6366f1;    /* Secondary indigo */
    --accent-color: #8b5cf6;       /* Accent purple */
}
```

### Update Social Links

In `index.html` footer section (around line 530):
```html
<a href="https://linkedin.com/in/YOUR-PROFILE" target="_blank">
<a href="https://github.com/YOUR-USERNAME" target="_blank">
```

### Modify Skills

Update skill percentages in `index.html` (Skills section, around line 150):
```html
<div class="skill-progress" style="width: 95%"></div>
```

### Add More Projects

Copy the project card structure in `index.html` (around line 350) and customize:
```html
<div class="project-card">
    <div class="project-icon">
        <i class="fas fa-your-icon"></i>
    </div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <!-- Add your content -->
    </div>
</div>
```

## 🌐 Deployment Options

### GitHub Pages
1. Create a GitHub repository
2. Push your code
3. Go to Settings > Pages
4. Select main branch and save
5. Your site will be live at `https://yourusername.github.io/portfolio`

### Netlify
1. Sign up at netlify.com
2. Drag and drop your portfolio folder
3. Your site will be live instantly

### Vercel
1. Sign up at vercel.com
2. Import your GitHub repository
3. Deploy with one click

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🎯 Performance Tips

1. Optimize images before adding them (use WebP format)
2. Keep resume PDF under 2MB
3. Test on multiple devices using browser DevTools
4. Use lazy loading for images if adding many photos

## 📧 Contact Form Setup

The contact form currently shows a success message. To make it functional:

### Option 1: Formspree (Easiest)
1. Sign up at formspree.io
2. Get your form endpoint
3. Update form action in `index.html`:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: EmailJS
1. Sign up at emailjs.com
2. Add EmailJS SDK to `index.html`
3. Update the form submission in `script.js`

### Option 3: Backend API
Integrate with your own backend service

## 🎨 Font Awesome Icons

The site uses Font Awesome 6.4.0 for icons. Find more icons at:
https://fontawesome.com/icons

## 📝 License

This portfolio template is free to use and customize for personal use.

## 🤝 Support

For issues or questions about customization, refer to:
- HTML/CSS basics: MDN Web Docs
- JavaScript: JavaScript.info
- Responsive design: CSS-Tricks

---

**Built with ❤️ for ServiceNow Developers**

Last Updated: February 2024
