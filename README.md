# Project Nautica Landing Page - Maintenance Guide

This guide will help you maintain and customize the Project Nautica landing page, even if you're new to web development. Follow these detailed instructions to make common updates while preserving the page's professional appearance.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the main navigation and brand name. To update:

1. **Company Name:**
```html
<a href="/" class="text-2xl font-bold">Project Nautica</a>
```
Simply replace "Project Nautica" with your company name.

2. **Announcement Bar:**
```html
<div class="bg-black text-white text-sm py-2 text-center">
    <p>Fast Worldwide Shipping (5 days delivery) 🚀</p>
</div>
```
Modify the text between `<p>` tags to update your announcement.

### Hero Section
Located at the top of the page with the large background image:

1. **Main Heading:**
```html
<h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">
    Build Your Store in Minutes, Not Days
</h1>
```
Replace the text while keeping the HTML tags intact.

2. **Subheading:**
```html
<p class="text-xl md:text-2xl mb-8">Bright. Precise. Professional.</p>
```

### Tailwind CSS Classes Explained
Common classes used throughout:
- `text-[size]`: Controls text size (xl, 2xl, 3xl, etc.)
- `font-[weight]`: Controls text boldness (bold, semibold, normal)
- `mb-[size]`: Adds margin bottom (4, 6, 8, etc.)
- `py-[size]`: Adds padding top and bottom
- `px-[size]`: Adds padding left and right

Example of modifying text size:
```html
<!-- Original -->
<h2 class="text-3xl font-bold">Enhance Your Photography</h2>

<!-- Modified to be larger -->
<h2 class="text-4xl font-bold">Enhance Your Photography</h2>
```

## Managing Links

### Navigation Menu Links
Located in the header section:
```html
<div class="hidden md:flex space-x-6">
    <a href="#features" class="text-gray-600 hover:text-black transition-colors">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-black transition-colors">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-black transition-colors">FAQ</a>
</div>
```

To update:
1. Locate the `href` attribute
2. Replace the value with your new link
3. Update the text between `<a>` tags

Example:
```html
<!-- Original -->
<a href="#features" class="text-gray-600 hover:text-black transition-colors">Features</a>

<!-- Modified -->
<a href="#products" class="text-gray-600 hover:text-black transition-colors">Products</a>
```

### Call-to-Action Links
Found throughout the page:
```html
<a href="https://projectnautica.com" class="inline-block bg-black text-white px-6 py-2 rounded-full hover:bg-gray-800 transition-colors">
    Buy Now
</a>
```

Replace `https://projectnautica.com` with your actual purchase or signup page URL.

## Adding Privacy and Terms Pages

### Footer Link Updates
Located at the bottom of the page:
```html
<div>
    <h4 class="font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
    </ul>
</div>
```

To link to policy pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check for typos in URLs
   - Ensure file names match exactly
   - Verify files are in the correct directory

2. **Styling Problems**
   - Make sure Tailwind CSS is properly loaded
   - Check for missing class names
   - Verify closing tags are present

3. **Responsive Design Issues**
   - Keep the `md:` prefix for desktop-specific styles
   - Don't remove the viewport meta tag
   - Test on multiple screen sizes

### Need Help?
If you encounter issues:
1. Check the browser's developer tools (F12) for errors
2. Verify all HTML tags are properly closed
3. Ensure all files are in the correct location
4. Compare your changes against the original code

Remember to always backup your files before making changes, and test your updates across different browsers and devices.