# Urban Trust Financial Landing Page - Maintenance Guide

This guide will help you maintain and customize the Urban Trust Financial landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates safely and effectively.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

1. Company Name:
```html
<!-- Located in header section -->
<a href="#" class="text-2xl font-bold text-white hover:text-blue-400 transition-colors duration-300">
    URBAN TRUST FINANCIAL
</a>
```
Simply replace "URBAN TRUST FINANCIAL" with your desired text.

### Hero Section
The main headline and subtitle can be updated here:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6 bg-gradient-to-r from-blue-400 to-purple-500 bg-clip-text text-transparent">
    A New Way to Buy Life Insurance
</h1>
<p class="text-xl md:text-2xl text-gray-400 mb-12 max-w-3xl mx-auto">
    Transform your financial future with innovative life insurance solutions that work for you.
</p>
```

#### Understanding Tailwind Classes:
- `text-4xl`: Large text on mobile
- `md:text-5xl`: Larger text on medium screens
- `lg:text-6xl`: Largest text on large screens
- `text-gray-400`: Light gray text color
- `mb-6`: Margin bottom spacing

### Features Section
To update feature cards:
```html
<div class="bg-gray-800 rounded-xl p-8 hover:transform hover:scale-105 transition-all duration-300">
    <i class="fas fa-university text-4xl text-blue-400 mb-6"></i>
    <h3 class="text-xl font-semibold mb-4">Become Your Own Bank</h3>
    <p class="text-gray-400">Take control of your financial future...</p>
</div>
```

To change icons, replace the `fa-university` class with any [Font Awesome icon class](https://fontawesome.com/icons).

## Managing Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300">Benefits</a>
    <a href="#faq" class="text-gray-300 hover:text-white transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-300 hover:text-white transition-colors duration-300">Contact</a>
</div>
```

To update a link:
1. Locate the `<a>` tag
2. Modify the `href` attribute
3. Update the link text between the tags

### External Links
The main call-to-action button links to:
```html
<a href="https://urbantrustfinancial.com" class="inline-block bg-blue-600 hover:bg-blue-700 text-white...">
```
Replace the URL with your desired destination.

### Email Links
Current email links use:
```html
<a href="mailto:nuvoenterprizes@gmail.com">
```
Update this email address throughout the document (appears in contact section and footer).

## Adding Privacy and Terms Pages

To add privacy and terms links to the footer:

1. Locate the footer quick links section:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Quick Links</h3>
    <ul class="space-y-2">
        <!-- Add new links here -->
```

2. Add the new links:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

3. Create matching privacy.html and terms.html files in the same directory as index.html.

## Troubleshooting

Common issues and solutions:

### Links Not Working
- Verify file names match exactly (case-sensitive)
- Ensure files are in the correct directory
- Check for typos in href attributes

### Styling Issues
- Make sure Tailwind CSS CDN link is present in head:
```html
<script src="https://cdn.tailwindcss.com"></script>
```
- Verify class names are spelled correctly
- Check for missing spaces between multiple classes

### Icons Not Showing
- Confirm Font Awesome CDN link is present:
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
```
- Verify icon class names in the [Font Awesome documentation](https://fontawesome.com/icons)

Remember to test all changes across different devices and screen sizes to ensure responsive design remains intact.

Need more help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).