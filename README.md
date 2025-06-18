# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Follow these detailed instructions to make common updates while preserving the design and functionality.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<div class="text-2xl font-bold">Lorem ipsum</div>
```
- To change the company name/logo text, replace "Lorem ipsum" with your desired text
- Keep it brief (2-3 words) to maintain layout

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8">Modern Solutions for Modern Business</h1>
<p class="text-xl text-gray-600 mb-12">Transform your business presence...</p>
```
- Update the main heading by replacing "Modern Solutions for Modern Business"
- Modify the subheading text while keeping similar length for layout consistency

#### Feature Cards
Each feature card follows this structure:
```html
<div class="bg-white p-8 rounded-2xl shadow-lg hover:shadow-xl transition-shadow duration-300">
    <div class="w-12 h-12 bg-gray-900 rounded-lg mb-6"></div>
    <h3 class="text-xl font-bold mb-4">Professional Design</h3>
    <p class="text-gray-600">Modern and minimalist approach...</p>
</div>
```
- Update card titles in the `<h3>` tags
- Modify description text in the `<p>` tags
- Maintain similar text length to preserve layout

### Tailwind CSS Modifications

#### Understanding Key Classes
- `container`: Centers content and sets max-width
- `mx-auto`: Centers elements horizontally
- `px-6`: Adds horizontal padding
- `py-4`: Adds vertical padding
- `text-gray-600`: Sets text color
- `hover:text-gray-900`: Changes text color on hover

#### Responsive Classes
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl">
```
This example shows responsive text sizing:
- `text-4xl`: Base size (mobile)
- `md:text-5xl`: Medium screens
- `lg:text-6xl`: Large screens

#### Modifying Colors
To change colors, replace these classes:
- Background colors: `bg-white`, `bg-gray-900`
- Text colors: `text-gray-600`, `text-gray-900`
- Border colors: `border-gray-100`

⚠️ **Important**: When modifying classes, always test on multiple screen sizes to ensure responsiveness.

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Home</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">About</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Services</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. Replace `#` with proper page URLs
2. Example:
   ```html
   <a href="index.html">Home</a>
   <a href="about.html">About</a>
   <a href="services.html">Services</a>
   <a href="contact.html">Contact</a>
   ```

### Social Media Links
Located in the footer:
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-600 hover:text-gray-900">
        <!-- Twitter SVG -->
    </a>
    <a href="#" class="text-gray-600 hover:text-gray-900">
        <!-- LinkedIn SVG -->
    </a>
</div>
```

To update:
1. Replace `#` with full social media profile URLs
2. Example:
   ```html
   <a href="https://twitter.com/yourprofile">
   <a href="https://linkedin.com/in/yourprofile">
   ```

## 3. Linking Privacy and Terms Pages

### Footer Legal Links
Current structure:
```html
<div>
    <h4 class="text-lg font-bold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create privacy.html and terms.html files in your project folder
2. Update the links:
   ```html
   <li><a href="privacy.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Privacy Policy</a></li>
   <li><a href="terms.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Terms of Service</a></li>
   ```

### Troubleshooting Tips

1. **Broken Links**
   - Use relative paths (e.g., `about.html`) for internal pages
   - Use full URLs (e.g., `https://...`) for external links
   - Test all links after updating

2. **Style Consistency**
   - Copy existing link classes when adding new links
   - Maintain the same hover effects and transitions

3. **Common Issues**
   - If pages don't load, check file names and paths
   - Ensure all HTML files are in the correct directory
   - Verify that all files use the same CSS framework links

Need help? Check the browser's developer tools (F12) for error messages in the console.