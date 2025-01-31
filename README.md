# Melbourne Website Design - Landing Page Maintenance Guide

This guide will help you maintain and customize the Melbourne Website Design landing page. Whether you're new to web development or need a quick reference, follow these instructions to make updates safely and effectively.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. **Logo Text (MWD)**
```html
<a href="/" class="text-2xl font-bold text-gray-800 hover:text-blue-600 transition duration-300">
    MWD  <!-- Change this text to your desired logo text -->
</a>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Update text here -->
    <a href="#benefits">Benefits</a>  <!-- Update text here -->
    <a href="#faq">FAQ</a>           <!-- Update text here -->
    <a href="#contact">Contact</a>    <!-- Update text here -->
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 leading-tight tracking-tight">
    Best Websites In Melbourne  <!-- Update main headline here -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    Professional web design solutions...  <!-- Update subheading here -->
</p>
```

### Tailwind CSS Tips
- Font sizes: `text-sm`, `text-base`, `text-lg`, `text-xl`, `text-2xl`, etc.
- Colors: `text-gray-900`, `bg-blue-600`, `text-white`
- Spacing: `p-4` (padding), `m-4` (margin), `space-x-4` (horizontal spacing)
- Responsive prefixes: `md:`, `lg:` (e.g., `md:text-xl`)

## Managing Links

### External Links
Replace these placeholder URLs with your actual links:

```html
<!-- Header "Get Started" button -->
<a href="https://mwd.com" class="hidden md:inline-block bg-blue-600">
    Get Started
</a>

<!-- Hero section button -->
<a href="https://mwd.com" class="inline-block bg-blue-600">
    Start Your Project
</a>
```

### Internal Navigation Links
Update these to match your section IDs:

```html
<!-- In the navigation menu -->
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

### Social Media Links
Located in the footer:

```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-300 hover:text-white">
        <i class="fab fa-twitter text-xl"></i>
    </a>
    <!-- Replace # with your social media URLs -->
</div>
```

## Adding Privacy and Terms Pages

### 1. Create New Files
Create two new files in your project directory:
- `privacy.html`
- `terms.html`

### 2. Update Footer Links
Replace the placeholder links in the footer:

```html
<div>
    <h4 class="text-white text-lg font-bold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="privacy.html" class="hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### 3. Maintain Consistent Styling
Copy these classes for new page links:
- Normal state: `text-gray-300`
- Hover state: `hover:text-white transition duration-300`

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check for typos in `href` attributes
   - Ensure file names match exactly (case-sensitive)
   - Verify all files are in the correct directory

2. **Responsive Design Issues**
   - Check responsive prefixes (`md:`, `lg:`)
   - Test on different screen sizes
   - Ensure mobile menu is working

3. **Style Problems**
   - Verify Tailwind CSS CDN link is working
   - Check for missing classes
   - Ensure Font Awesome CDN is loading

### Need Help?
If you encounter issues:
1. Check the browser console for errors (F12)
2. Verify all CDN links are accessible
3. Test on different browsers
4. Ensure all files are properly saved

Remember to always make a backup before making significant changes to your site.

---

For additional support or questions, contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).