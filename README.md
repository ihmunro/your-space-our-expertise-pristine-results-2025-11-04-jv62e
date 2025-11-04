# Fresh Feel Painting and Cleaning - Landing Page Maintenance Guide

Welcome! This comprehensive guide will help you maintain and customize the Fresh Feel Painting and Cleaning landing page. Whether you're updating text, fixing links, or adding new pages, this guide provides step-by-step instructions tailored to this specific website.

---

## Table of Contents

1. [Understanding the Page Structure](#understanding-the-page-structure)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Fixing and Managing Links](#fixing-and-managing-links)
5. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
6. [Troubleshooting Common Issues](#troubleshooting-common-issues)
7. [Best Practices](#best-practices)

---

## Understanding the Page Structure

Before making changes, it's helpful to understand how this landing page is organized. Think of it like a building with different floors, each serving a specific purpose.

### Main Sections of the Page

The landing page is divided into these key sections:

| Section | Purpose | Location in HTML |
|---------|---------|------------------|
| **Header/Navigation** | Menu and branding at the top | Lines 64-119 |
| **Hero Section** | Eye-catching main message | Lines 121-158 |
| **Features Section** | Three key service highlights | Lines 160-216 |
| **Benefits Section** | Why clients should choose you | Lines 218-290 |
| **Testimonials Section** | Client success stories | Lines 292-378 |
| **About Us Section** | Company information | Lines 380-425 |
| **FAQ Section** | Common questions answered | Lines 427-523 |
| **CTA Section** | Final call-to-action | Lines 525-546 |
| **Footer** | Contact info and links | Lines 548-635 |

### Key Terminology

- **HTML**: The code that structures your content (headings, paragraphs, links, etc.)
- **Tailwind CSS**: A system of pre-made styling classes that control colors, sizes, spacing, and layout
- **Class**: Instructions that tell the browser how to style an element (e.g., `text-white` makes text white)
- **Href**: The address a link points to (like `#features` or `https://example.com`)

---

## Updating Text Content

Updating text is the most straightforward customization. Here's how to do it safely and effectively.

### Finding and Replacing Text

**Step 1: Open Your HTML File**

Open `index.html` in any text editor (Notepad, VS Code, Sublime Text, etc.).

**Step 2: Use Find and Replace**

Most text editors have a "Find and Replace" feature:
- **Windows/Linux**: Press `Ctrl + H`
- **Mac**: Press `Cmd + Option + F`

This opens a dialog where you can search for old text and replace it with new text.

### Updating the Header/Logo Area

**Location**: Lines 74-77

**Current Code:**
```html
<div class="text-2xl font-bold text-gradient">
    <i class="fas fa-paint-brush mr-2"></i>Fresh Feel
</div>
```

**To Update the Company Name:**

1. Find the text `Fresh Feel`
2. Replace it with your company name
3. Keep the `<i class="fas fa-paint-brush mr-2"></i>` part—this creates the paintbrush icon

**Example:**
```html
<div class="text-2xl font-bold text-gradient">
    <i class="fas fa-paint-brush mr-2"></i>Your Company Name
</div>
```

### Updating the Hero Section (Main Headline)

**Location**: Lines 142-147

**Current Code:**
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold leading-tight tracking-tight">
    <span class="text-gradient">Your Space, Our Expertise:</span>
    <br>
    <span class="text-white">Pristine Results.</span>
</h1>
```

**To Update:**

1. Change `Your Space, Our Expertise:` to your preferred headline
2. Change `Pristine Results.` to your subtitle
3. Keep the `<span>` tags—they control styling

**Example:**
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold leading-tight tracking-tight">
    <span class="text-gradient">Transform Your Space Today:</span>
    <br>
    <span class="text-white">Professional Excellence Guaranteed.</span>
</h1>
```

### Updating the Hero Description

**Location**: Lines 149-153

**Current Code:**
```html
<p class="text-xl md:text-2xl text-gray-300 max-w-3xl mx-auto leading-relaxed font-light">
    Entrust your home or business to painting and cleaning perfection. We deliver impeccable finishes and germ-free surfaces with a commitment to excellence that exceeds expectations.
</p>
```

**To Update:**

Simply replace the text between `<p>` and `</p>` with your new description. Keep all the class names the same.

**Example:**
```html
<p class="text-xl md:text-2xl text-gray-300 max-w-3xl mx-auto leading-relaxed font-light">
    Professional painting and cleaning services that transform your space. Experience pristine finishes and spotless surfaces backed by our satisfaction guarantee.
</p>
```

### Updating Feature Cards

**Location**: Lines 180-216 (three feature cards)

Each feature card has the same structure:

**Current Code (Example - Feature 1):**
```html
<div class="card-hover bg-gray-800 border border-gray-700 hover:border-purple-500 rounded-xl p-8 shadow-lg hover:shadow-2xl transition-all duration-300">
    <div class="mb-6 text-4xl text-purple-500">
        <i class="fas fa-tools"></i>
    </div>
    <h3 class="text-2xl font-bold mb-4 text-white">Detailed Surface Prep</h3>
    <p class="text-gray-300 leading-relaxed mb-4">
        We don't cut corners. Our meticulous surface preparation...
    </p>
    <ul class="space-y-2 text-gray-400">
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-500"></i> Professional-grade cleaning
        </li>
        <!-- More list items -->
    </ul>
</div>
```

**To Update Feature Title:**
Change `Detailed Surface Prep` to your new title

**To Update Feature Description:**
Replace the paragraph text (the long description)

**To Update Feature List Items:**
Replace each list item text, keeping the `<i class="fas fa-check text-green-500"></i>` part

**To Change the Icon:**
Replace `fas fa-tools` with a different Font Awesome icon. See the [Font Awesome Icon List](https://fontawesome.com/icons) for options.

**Example:**
```html
<h3 class="text-2xl font-bold mb-4 text-white">Expert Preparation</h3>
<p class="text-gray-300 leading-relaxed mb-4">
    Thorough surface preparation is the foundation of quality work...
</p>
<ul class="space-y-2 text-gray-400">
    <li class="flex items-center gap-2">
        <i class="fas fa-check text-green-500"></i> Complete surface inspection
    </li>
    <li class="flex items-center gap-2">
        <i class="fas fa-check text-green-500"></i> Professional dust removal
    </li>
</ul>
```

### Updating Testimonials

**Location**: Lines 315-378 (four testimonial cards)

Each testimonial has this structure:

**Current Code (Example):**
```html
<div class="card-hover bg-gray-900 border border-gray-700 hover:border-purple-500 rounded-xl p-8 shadow-lg hover:shadow-2xl transition-all duration-300">
    <div class="flex items-center gap-1 mb-4">
        <i class="fas fa-star text-yellow-400"></i>
        <!-- More stars -->
    </div>
    <p class="text-gray-300 text-lg mb-6 leading-relaxed">
        "Fresh Feel transformed our office space completely..."
    </p>
    <div class="flex items-center gap-4">
        <div class="w-12 h-12 rounded-full bg-gradient-to-br from-purple-500 to-pink-500 flex items-center justify-center font-bold text-white">
            JM
        </div>
        <div>
            <p class="font-bold text-white">Jennifer Mitchell</p>
            <p class="text-gray-400 text-sm">Office Manager, Tech Solutions Inc.</p>
        </div>
    </div>
</div>
```

**To Update:**

1. Replace the testimonial text (between the quotation marks)
2. Change the initials (e.g., `JM` to match the client's name)
3. Update the client name
4. Update the client's title and company

**Example:**
```html
<p class="text-gray-300 text-lg mb-6 leading-relaxed">
    "The team did an amazing job painting our home. Professional, clean, and the results are stunning!"
</p>
<div class="flex items-center gap-4">
    <div class="w-12 h-12 rounded-full bg-gradient-to-br from-purple-500 to-pink-500 flex items-center justify-center font-bold text-white">
        DW
    </div>
    <div>
        <p class="font-bold text-white">David Williams</p>
        <p class="text-gray-400 text-sm">Homeowner, Portland OR</p>
    </div>
</div>
```

### Updating the About Section

**Location**: Lines 395-422

**Current Code (Text Portion):**
```html
<h2 class="text-4xl md:text-5xl font-bold mb-6">
    <span class="text-gradient">About Fresh Feel</span>
</h2>
<p class="text-lg text-gray-300 leading-relaxed mb-6">
    Fresh Feel Painting and Cleaning was founded...
</p>
<p class="text-lg text-gray-300 leading-relaxed">
    At Fresh Feel, we believe that quality...
</p>
```

**To Update:**

1. Change `About Fresh Feel` to your preferred heading
2. Replace the first paragraph with your company story
3. Replace the second paragraph with your company mission

**Updating Statistics:**

```html
<div class="grid grid-cols-2 gap-6 pt-8">
    <div class="bg-gray-800 rounded-lg p-6 border border-gray-700">
        <p class="text-4xl font-bold text-gradient mb-2">500+</p>
        <p class="text-gray-300">Projects Completed</p>
    </div>
    <div class="bg-gray-800 rounded-lg p-6 border border-gray-700">
        <p class="text-4xl font-bold text-gradient mb-2">98%</p>
        <p class="text-gray-300">Client Satisfaction</p>
    </div>
</div>
```

Change `500+` and `98%` to your actual statistics, and update the labels accordingly.

### Updating FAQ Items

**Location**: Lines 450-523

Each FAQ item has this structure:

**Current Code (Example):**
```html
<div class="faq-item bg-gray-900 border border-gray-700 rounded-lg overflow-hidden shadow-md hover:shadow-lg transition-all duration-300">
    <button class="faq-question w-full px-6 py-6 text-left flex items-center justify-between hover:bg-gray-800 transition-colors duration-300 cursor-pointer">
        <span class="text-lg font-semibold text-white">How long does a typical painting project take?</span>
        <i class="faq-icon fas fa-chevron-down text-purple-500 transition-transform duration-300"></i>
    </button>
    <div class="faq-answer hidden border-t border-gray-700 px-6 py-6 bg-gray-800 bg-opacity-50">
        <p class="text-gray-300 leading-relaxed">
            The timeline depends on the scope of your project...
        </p>
    </div>
</div>
```

**To Update:**

1. Change the question text (between the `<span>` tags in the button)
2. Change the answer text (between the `<p>` tags in the faq-answer div)

**Example:**
```html
<button class="faq-question w-full px-6 py-6 text-left flex items-center justify-between hover:bg-gray-800 transition-colors duration-300 cursor-pointer">
    <span class="text-lg font-semibold text-white">What areas do you service?</span>
    <i class="faq-icon fas fa-chevron-down text-purple-500 transition-transform duration-300"></i>
</button>
<div class="faq-answer hidden border-t border-gray-700 px-6 py-6 bg-gray-800 bg-opacity-50">
    <p class="text-gray-300 leading-relaxed">
        We service the greater Portland metropolitan area including all surrounding suburbs...
    </p>
</div>
```

### Updating the Footer

**Location**: Lines 575-608

**Company Description:**
```html
<p class="text-gray-400 mb-6 leading-relaxed">
    Premium painting and cleaning services for homes and businesses. Your space, our expertise.
</p>
```

**Contact Email:**
```html
<li class="flex gap-3">
    <i class="fas fa-envelope text-purple-500 mt-1"></i>
    <a href="mailto:iainhmunro@gmail.com" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">iainhmunro@gmail.com</a>
</li>
```

To update the email, change `iainhmunro@gmail.com` in both places (in the href and the display text).

**Website URL:**
```html
<li class="flex gap-3">
    <i class="fas fa-globe text-purple-500 mt-1"></i>
    <a href="https://www.freshfeelpaintingandcleaning.ca/" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">freshfeelpaintingandcleaning.ca</a>
</li>
```

**Copyright Year:**
```html
<p>&copy; 2025 Fresh Feel Painting and Cleaning. All rights reserved.</p>
```

Change `2025` to the current year and `Fresh Feel Painting and Cleaning` to your company name.

---

## Modifying Tailwind CSS Classes

Tailwind CSS uses simple class names to control how things look. This section explains the most important classes used on this landing page and how to modify them.

### Understanding Tailwind Classes

Tailwind classes are descriptive and follow a pattern:

- `text-white` = white text
- `bg-gray-900` = dark gray background
- `px-8` = horizontal padding (left and right)
- `py-4` = vertical padding (top and bottom)
- `rounded-lg` = slightly rounded corners
- `shadow-lg` = large drop shadow

### Color Classes

The landing page uses a color scheme primarily based on grays, purples, and pinks.

**Text Colors:**
```
text-white          → White text
text-gray-300       → Light gray text
text-gray-400       → Medium gray text
text-purple-500     → Purple text
text-pink-600       → Pink text
```

**Background Colors:**
```
bg-gray-900         → Very dark gray background
bg-gray-800         → Dark gray background
bg-purple-600       → Purple background
bg-pink-600         → Pink background
```

**To Change All Purple Accents to Blue:**

Use Find and Replace (Ctrl+H or Cmd+Option+F):
1. Find: `purple`
2. Replace: `blue`
3. Click "Replace All"

**To Change All Pink Accents to Red:**

1. Find: `pink`
2. Replace: `red`
3. Click "Replace All"

### Spacing Classes

Tailwind uses a spacing system where numbers represent pixel values (4 = 4px, 8 = 8px, etc.).

**Common Spacing Classes:**

```
p-4         → 4px padding on all sides
px-8        → 8px padding left and right
py-6        → 6px padding top and bottom
m-4         → 4px margin on all sides
mx-auto     → Auto margin left and right (centers elements)
gap-4       → 4px gap between flex items
```

**Example: Increase Hero Button Padding**

**Current Code:**
```html
<a href="https://www.freshfeelpaintingandcleaning.ca/" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-8 py-4 rounded-lg font-bold text-lg shadow-lg hover:shadow-2xl inline-flex items-center justify-center gap-2 transition-all duration-300">
    <i class="fas fa-arrow-right"></i> Start Your Transformation
</a>
```

**To Make the Button Larger:**

Change `px-8 py-4` to `px-12 py-6`:

```html
<a href="https://www.freshfeelpaintingandcleaning.ca/" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-12 py-6 rounded-lg font-bold text-lg shadow-lg hover:shadow-2xl inline-flex items-center justify-center gap-2 transition-all duration-300">
    <i class="fas fa-arrow-right"></i> Start Your Transformation
</a>
```

### Typography Classes

These control how text looks:

```
text-4xl        → Very large text (hero headlines)
text-2xl        → Large text (section titles)
text-lg         → Slightly larger text (descriptions)
text-sm         → Small text (captions)
font-bold       → Bold text
font-semibold   → Semi-bold text
font-light      → Light/thin text
leading-relaxed → Increased line spacing for readability
```

**Example: Make Section Titles Larger**

**Current Code:**
```html
<h2 class="text-4xl md:text-5xl font-bold mb-4">
    <span class="text-gradient">Premium Features</span>
</h2>
```

**To Make Them Even Larger:**

Change to `text-5xl md:text-6xl`:

```html
<h2 class="text-5xl md:text-6xl font-bold mb-4">
    <span class="text-gradient">Premium Features</span>
</h2>
```

**Understanding Responsive Prefixes:**

The `md:` prefix means "on medium screens and larger." This allows different sizes on different devices:

```
text-4xl        → Extra small screens (phones)
sm:text-5xl     → Small screens and up
md:text-6xl     → Medium screens and up (tablets)
lg:text-7xl     → Large screens and up (desktops)
```

### Box and Border Classes

```
rounded-lg      → Slightly rounded corners
rounded-xl      → More rounded corners
border          → 1px border
border-gray-700 → Gray border
shadow-lg       → Large drop shadow
hover:shadow-2xl → Extra large shadow on hover
```

**Example: Make Cards More Rounded**

**Current Code:**
```html
<div class="card-hover bg-gray-800 border border-gray-700 hover:border-purple-500 rounded-xl p-8 shadow-lg hover:shadow-2xl transition-all duration-300">
```

**To Make Them Very Rounded:**

Change `rounded-xl` to `rounded-2xl`:

```html
<div class="card-hover bg-gray-800 border border-gray-700 hover:border-purple-500 rounded-2xl p-8 shadow-lg hover:shadow-2xl transition-all duration-300">
```

### Grid and Layout Classes

```
grid                    → Create a grid layout
grid-cols-1            → 1 column on small screens
md:grid-cols-3         → 3 columns on medium screens and up
gap-8                  → 8px space between grid items
flex                   → Create a flex layout
items-center           → Vertically center flex items
justify-between        → Space items apart
justify-center         → Center items horizontally
```

**Example: Change Feature Cards from 3 Columns to 2 Columns**

**Current Code:**
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
    <!-- Feature cards -->
</div>
```

**To Change to 2 Columns:**

Change `md:grid-cols-3` to `md:grid-cols-2`:

```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <!-- Feature cards -->
</div>
```

### Gradient Classes

The landing page uses gradient backgrounds for visual interest:

```
bg-gradient-to-r         → Gradient from left to right
bg-gradient-to-br        → Gradient from top-left to bottom-right
from-purple-600          → Starting color of gradient
to-pink-600              → Ending color of gradient
```

**Example: Change Gradient Direction**

**Current Code:**
```html
<a href="..." class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 ...">
```

**To Change to Diagonal:**

Change `bg-gradient-to-r` to `bg-gradient-to-br`:

```html
<a href="..." class="btn-primary bg-gradient-to-br from-purple-600 to-pink-600 ...">
```

### Hover Effects

Tailwind uses the `hover:` prefix to apply styles when users hover over elements:

```
hover:text-white            → White text on hover
hover:border-purple-500     → Purple border on hover
hover:shadow-2xl            → Extra large shadow on hover
hover:from-purple-700       → Darker purple on hover
```

**Example: Change Hover Color**

**Current Code:**
```html
<a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Features</a>
```

**To Change Hover Color to Purple:**

Change `hover:text-white` to `hover:text-purple-400`:

```html
<a href="#features" class="text-gray-300 hover:text-purple-400 transition-colors duration-300 font-medium">Features</a>
```

### Opacity Classes

Control transparency:

```
opacity-50      → 50% transparent
opacity-20      → 20% transparent (mostly transparent)
bg-opacity-95   → Background is 95% opaque
```

**Example: Make Navigation More Transparent**

**Current Code:**
```html
<header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-sm border-b border-gray-800">
```

**To Make It More Transparent:**

Change `bg-opacity-95` to `bg-opacity-80`:

```html
<header class="sticky top-0 z-50 bg-gray-900 bg-opacity-80 backdrop-blur-sm border-b border-gray-800">
```

### Common Customization Scenarios

#### Scenario 1: Change Primary Color from Purple to Teal

1. Open Find and Replace (Ctrl+H or Cmd+Option+F)
2. Find: `purple`
3. Replace: `teal`
4. Click "Replace All"

Then do the same for pink:
1. Find: `pink`
2. Replace: `cyan`
3. Click "Replace All"

#### Scenario 2: Make the Page Lighter

1. Find: `bg-gray-900`
2. Replace: `bg-gray-100`
3. Click "Replace All"

Then update text colors:
1. Find: `text-white`
2. Replace: `text-gray-900`
3. Click "Replace All"

#### Scenario 3: Increase Spacing Throughout

1. Find: `gap-8`
2. Replace: `gap-12`
3. Click "Replace All"

Then:
1. Find: `p-8`
2. Replace: `p-12`
3. Click "Replace All"

---

## Fixing and Managing Links

Links are crucial for navigation and directing visitors to important pages. This section shows you how to update every link on the page.

### Understanding Link Structure

A link in HTML looks like this:

```html
<a href="https://www.example.com">Click Here</a>
```

- `<a>` = starts a link
- `href=` = where the link goes
- `"https://www.example.com"` = the destination
- `Click Here` = what visitors see and click on
- `</a>` = ends the link

### Types of Links on This Page

1. **Navigation Menu Links** - Links in the header that jump to sections
2. **CTA (Call-to-Action) Links** - Buttons that direct to your website
3. **Footer Links** - Links in the footer for navigation and policies
4. **Social Media Links** - Links to your social profiles

### Navigation Menu Links

**Location**: Lines 83-91 (Desktop) and 103-109 (Mobile)

These links use the `#` symbol to jump to sections on the same page.

**Current Code (Desktop Menu):**
```html
<a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Features</a>
<a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Benefits</a>
<a href="#testimonials" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Testimonials</a>
<a href="#faq" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
<a href="#about" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
```

**These Links Are Working Correctly** ✓

These anchor links (`#features`, `#benefits`, etc.) match the section IDs in the page:
- `<section id="features">` on line 160
- `<section id="benefits">` on line 218
- `<section id="testimonials">` on line 292
- `<section id="faq">` on line 427
- `<section id="about">` on line 380

**To Add a New Menu Link:**

1. Add the link to the navigation menu:
```html
<a href="#services" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Services</a>
```

2. Create a corresponding section in the page:
```html
<section id="services" class="py-24 bg-gray-900">
    <!-- Your services content here -->
</section>
```

3. Add the same link to the mobile menu (around line 103)

### CTA (Call-to-Action) Links

These buttons direct visitors to your main website. **These currently point to the same website**, which may cause issues.

**Location**: Lines 95-98 (Desktop Button), 111-113 (Mobile Button), 155-157 (Hero Section), 533-535 (Final CTA)

**Current Code:**
```html
<a href="https://www.freshfeelpaintingandcleaning.ca/" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
    Get Started
</a>
```

**Common Issues and Fixes:**

**Issue 1: CTA Links Point to the Same Page**

If you're using this landing page as your main website, you have two options:

**Option A: Change Links to Contact Form or Phone**

Replace the href with a phone number:
```html
<a href="tel:+15035551234" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
    Get Started
</a>
```

Replace the href with an email:
```html
<a href="mailto:contact@yourcompany.com" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
    Get Started
</a>
```

**Option B: Change Links to Contact Section**

```html
<a href="#contact" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
    Get Started
</a>
```

Then create a contact section in the page.

**Option C: Link to External Website**

If you have a separate website for bookings:
```html
<a href="https://www.yourbookingsite.com" class="btn-primary bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
    Get Started
</a>
```

**Step-by-Step to Update All CTA Links:**

1. Decide on your link destination (phone, email, or external site)
2. Open Find and Replace (Ctrl+H or Cmd+Option+F)
3. Find: `https://www.freshfeelpaintingandcleaning.ca/`
4. Replace: Your new destination (e.g., `tel:+15035551234`)
5. Click "Replace All"

**Example: Change All CTAs to Phone Number**

1. Find: `https://www.freshfeelpaintingandcleaning.ca/`
2. Replace: `tel:+15035551234`
3. Click "Replace All"

Result: All CTA buttons now call your phone number when clicked.

### Footer Links

**Location**: Lines 575-635

#### Footer Service Links

**Current Code (Lines 584-590):**
```html
<h3 class="text-lg font-bold text-white mb-6">Services</h3>
<ul class="space-y-3">
    <li><a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Interior Painting</a></li>
    <li><a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Exterior Painting</a></li>
    <li><a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Deep Cleaning</a></li>
    <li><a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Commercial Services</a></li>
</ul>
```

**Issue**: These links point to `#` (nowhere). 

**To Fix - Option 1: Link to Service Sections**

If you have service sections on your page:
```html
<li><a href="#interior-painting" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Interior Painting</a></li>
<li><a href="#exterior-painting" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Exterior Painting</a></li>
<li><a href="#deep-cleaning" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Deep Cleaning</a></li>
<li><a href="#commercial-services" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Commercial Services</a></li>
```

**To Fix - Option 2: Link to External Pages**

```html
<li><a href="services/interior-painting.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Interior Painting</a></li>
<li><a href="services/exterior-painting.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Exterior Painting</a></li>
<li><a href="services/deep-cleaning.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Deep Cleaning</a></li>
<li><a href="services/commercial-services.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">Commercial Services</a></li>
```

#### Footer Contact Email

**Location**: Lines 599-601

**Current Code:**
```html
<li class="flex gap-3">
    <i class="fas fa-envelope text-purple-500 mt-1"></i>
    <a href="mailto:iainhmunro@gmail.com" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">iainhmunro@gmail.com</a>
</li>
```

**To Update Your Email:**

1. Find: `iainhmunro@gmail.com`
2. Replace: `your-email@yourcompany.com`
3. Click "Replace All"

**Important**: Change it in both places (the href and the display text).

#### Footer Website URL

**Location**: Lines 602-604

**Current Code:**
```html
<li class="flex gap-3">
    <i class="fas fa-globe text-purple-500 mt-1"></i>
    <a href="https://www.freshfeelpaintingandcleaning.ca/" class="text-gray-400 hover:text-purple-500 transition-colors duration-300">freshfeelpaintingandcleaning.ca</a>
</li>
```

**To Update:**

1. Find: `https://www.freshfeelpaintingandcleaning.ca/`
2. Replace: `https://www.yourwebsite.com`
3. Click "Replace All"

Also update the display text:
1. Find: `freshfeelpaintingandcleaning.ca`
2. Replace: `yourwebsite.com`
3. Click "Replace All"

#### Footer Social Media Links

**Location**: Lines 577-585

**Current Code:**
```html
<div class="flex gap-4">
    <a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-facebook"></i>
    </a>
    <a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-instagram"></i>
    </a>
    <a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-twitter"></i>
    </a>
    <a href="#" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-linkedin"></i>
    </a>
</div>
```

**To Add Your Social Media:**

Replace each `href="#"` with your social media URL:

```html
<div class="flex gap-4">
    <a href="https://www.facebook.com/yourpage" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-facebook"></i>
    </a>
    <a href="https://www.instagram.com/yourprofile" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-instagram"></i>
    </a>
    <a href="https://www.twitter.com/yourprofile" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-twitter"></i>
    </a>
    <a href="https://www.linkedin.com/company/yourcompany" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-linkedin"></i>
    </a>
</div>
```

**To Remove Social Media Icons You Don't Use:**

Simply delete the entire `<a>` tag for that platform. For example, to remove LinkedIn:

```html
<div class="flex gap-4">
    <a href="https://www.facebook.com/yourpage" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-facebook"></i>
    </a>
    <a href="https://www.instagram.com/yourprofile" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-instagram"></i>
    </a>
    <a href="https://www.twitter.com/yourprofile" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 text-xl">
        <i class="fab fa-twitter"></i>
    </a>
</div>
```

### Footer Policy Links

**Location**: Lines 617-619

**Current Code:**
```html
<a href="privacy.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Privacy Policy</a>
<a href="terms.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Terms of Service</a>
<a href="blog.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Blog</a>
```

**These links are set up correctly** ✓

They point to `privacy.html`, `terms.html`, and `blog.html` in the same folder as your `index.html` file.

**If your files are in a different location:**

For example, if your files are in a `pages` folder:
```html
<a href="pages/privacy.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Privacy Policy</a>
<a href="pages/terms.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Terms of Service</a>
<a href="pages/blog.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Blog</a>
```

### Link Troubleshooting Checklist

Before testing links, verify:

- [ ] All URLs are correct and use proper format (`https://`, `mailto:`, `tel:`, or `#`)
- [ ] Internal links (like `#features`) match section IDs in the page
- [ ] File paths are correct for relative links (like `privacy.html`)
- [ ] No spaces in URLs or file paths
- [ ] All links are within `<a>` tags with `href=` attributes

---

## Linking Privacy and Terms Pages

This section provides detailed instructions for creating and linking your Privacy Policy and Terms of Service pages.

### Understanding File Structure

Before creating new pages, understand how files are organized:

```
Your Website Folder/
├── index.html (your main landing page)
├── privacy.html (privacy policy - create this)
├── terms.html (terms of service - create this)
└── blog.html (blog - create this)
```

All files should be in the same folder for the links to work correctly.

### Step 1: Create the Privacy Policy Page

**Step 1A: Create a New File**

1. Open your text editor
2. Click File → New
3. Copy and paste the template below
4. Click File → Save As
5. Name it: `privacy.html`
6. Make sure it's in the same folder as `index.html`

**Step 1B: Privacy Policy Template**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Fresh Feel Painting and Cleaning">
    <title>Privacy Policy - Fresh Feel Painting and Cleaning</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');
        
        * {
            font-family: 'Poppins', sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        .text-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation (Same as index.html) -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-sm border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex items-center justify-between">
            <div class="flex items-center space-x-2">
                <div class="text-2xl font-bold text-gradient">
                    <i class="fas fa-paint-brush mr-2"></i>Fresh Feel
                </div>
            </div>

            <div class="hidden md:flex items-center space-x-8">
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Home</a>
                <a href="index.html#features" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Services</a>
                <a href="index.html#about" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
            </div>

            <div class="hidden md:block">
                <a href="tel:+15035551234" class="bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
                    Contact
                </a>
            </div>

            <button class="mobile-menu-button md:hidden text-white text-2xl hover:text-purple-400 transition-colors duration-300">
                <i class="fas fa-bars"></i>
            </button>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-bold mb-12">
                <span class="text-gradient">Privacy Policy</span>
            </h1>

            <div class="prose prose-invert max-w-none space-y-8">
                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Introduction</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Fresh Feel Painting and Cleaning ("we", "our", or "us") operates the website. This page informs you of our policies regarding the collection, use, and disclosure of personal data when you use our service and the choices you have associated with that data.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Information Collection and Use</h2>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        We collect several different types of information for various purposes to provide and improve our service to you.
                    </p>
                    <ul class="list-disc list-inside space-y-2 text-gray-300">
                        <li>Personal Data: Name, email address, phone number, address</li>
                        <li>Usage Data: Browser type, IP address, pages visited</li>
                        <li>Cookies and similar tracking technologies</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Use of Data</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Fresh Feel Painting and Cleaning uses the collected data for various purposes:
                    </p>
                    <ul class="list-disc list-inside space-y-2 text-gray-300 mt-4">
                        <li>To provide and maintain our service</li>
                        <li>To notify you about changes to our service</li>
                        <li>To allow you to participate in interactive features of our service</li>
                        <li>To provide customer support</li>
                        <li>To gather analysis or valuable information so that we can improve our service</li>
                        <li>To monitor the usage of our service</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Security of Data</h2>
                    <p class="text-gray-300 leading-relaxed">
                        The security of your data is important to us but remember that no method of transmission over the Internet or method of electronic storage is 100% secure. While we strive to use commercially acceptable means to protect your personal data, we cannot guarantee its absolute security.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Contact Us</h2>
                    <p class="text-gray-300 leading-relaxed">
                        If you have any questions about this Privacy Policy, please contact us at:
                    </p>
                    <ul class="list-disc list-inside space-y-2 text-gray-300 mt-4">
                        <li>Email: contact@yourcompany.com</li>
                        <li>Phone: (503) 555-1234</li>
                    </ul>
                </div>
            </div>

            <div class="mt-12 pt-8 border-t border-gray-700">
                <a href="index.html" class="inline-flex items-center gap-2 text-purple-400 hover:text-purple-300 transition-colors duration-300 font-semibold">
                    <i class="fas fa-arrow-left"></i> Back to Home
                </a>
            </div>
        </div>
    </section>

    <!-- Footer (Same as index.html) -->
    <footer class="bg-gray-950 border-t border-gray-800 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center text-gray-500 text-sm">
                <p>&copy; 2025 Fresh Feel Painting and Cleaning. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
```

**Customization Notes:**

1. Replace `contact@yourcompany.com` with your actual email
2. Replace `(503) 555-1234` with your actual phone number
3. Update the privacy policy content with your actual policies
4. Update the phone number in the contact link if different

### Step 2: Create the Terms of Service Page

**Step 2A: Create a New File**

1. Open your text editor
2. Click File → New
3. Copy and paste the template below
4. Click File → Save As
5. Name it: `terms.html`
6. Make sure it's in the same folder as `index.html`

**Step 2B: Terms of Service Template**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Fresh Feel Painting and Cleaning">
    <title>Terms of Service - Fresh Feel Painting and Cleaning</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');
        
        * {
            font-family: 'Poppins', sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        .text-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-sm border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex items-center justify-between">
            <div class="flex items-center space-x-2">
                <div class="text-2xl font-bold text-gradient">
                    <i class="fas fa-paint-brush mr-2"></i>Fresh Feel
                </div>
            </div>

            <div class="hidden md:flex items-center space-x-8">
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Home</a>
                <a href="index.html#features" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Services</a>
                <a href="index.html#about" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
            </div>

            <div class="hidden md:block">
                <a href="tel:+15035551234" class="bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
                    Contact
                </a>
            </div>

            <button class="mobile-menu-button md:hidden text-white text-2xl hover:text-purple-400 transition-colors duration-300">
                <i class="fas fa-bars"></i>
            </button>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-bold mb-12">
                <span class="text-gradient">Terms of Service</span>
            </h1>

            <div class="prose prose-invert max-w-none space-y-8">
                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Agreement to Terms</h2>
                    <p class="text-gray-300 leading-relaxed">
                        By accessing and using this website and our services, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Service Description</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Fresh Feel Painting and Cleaning provides professional painting and cleaning services for residential and commercial properties. Our services include interior painting, exterior painting, and deep cleaning protocols.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">User Responsibilities</h2>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        As a user of our services, you agree to:
                    </p>
                    <ul class="list-disc list-inside space-y-2 text-gray-300">
                        <li>Provide accurate information when requesting our services</li>
                        <li>Grant us access to your property at agreed-upon times</li>
                        <li>Inform us of any specific concerns or requirements</li>
                        <li>Comply with all applicable laws and regulations</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Limitation of Liability</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Fresh Feel Painting and Cleaning shall not be liable for any indirect, incidental, special, consequential, or punitive damages resulting from your use of or inability to use the services. Our liability is limited to the amount paid for the specific service that gave rise to the claim.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Cancellation Policy</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Cancellations must be made at least 48 hours in advance. Cancellations made with less than 48 hours notice may be subject to a cancellation fee equal to 50% of the estimated service cost.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Satisfaction Guarantee</h2>
                    <p class="text-gray-300 leading-relaxed">
                        We stand behind our work with a 100% satisfaction guarantee. If you are not satisfied with our service, please contact us within 7 days of service completion, and we will make necessary adjustments at no additional cost.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Changes to Terms</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Fresh Feel Painting and Cleaning reserves the right to modify these terms at any time. Changes will be effective immediately upon posting to the website. Your continued use of the service following the posting of revised terms means that you accept and agree to the changes.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">Contact Us</h2>
                    <p class="text-gray-300 leading-relaxed">
                        If you have any questions about these Terms of Service, please contact us at:
                    </p>
                    <ul class="list-disc list-inside space-y-2 text-gray-300 mt-4">
                        <li>Email: contact@yourcompany.com</li>
                        <li>Phone: (503) 555-1234</li>
                    </ul>
                </div>
            </div>

            <div class="mt-12 pt-8 border-t border-gray-700">
                <a href="index.html" class="inline-flex items-center gap-2 text-purple-400 hover:text-purple-300 transition-colors duration-300 font-semibold">
                    <i class="fas fa-arrow-left"></i> Back to Home
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center text-gray-500 text-sm">
                <p>&copy; 2025 Fresh Feel Painting and Cleaning. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
```

**Customization Notes:**

1. Replace `contact@yourcompany.com` with your actual email
2. Replace `(503) 555-1234` with your actual phone number
3. Update the terms content with your actual policies
4. Modify the cancellation policy to match your business practices

### Step 3: Verify the Links Are Working

**In index.html, the footer already contains:**

```html
<a href="privacy.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Privacy Policy</a>
<a href="terms.html" class="text-gray-400 hover:text-purple-500 transition-colors duration-300 font-medium">Terms of Service</a>
```

These links are correctly set up! ✓

**To verify everything works:**

1. Save all three files (`index.html`, `privacy.html`, `terms.html`) in the same folder
2. Open `index.html` in your web browser
3. Scroll to the footer
4. Click "Privacy Policy" - it should open `privacy.html`
5. Click "Terms of Service" - it should open `terms.html`
6. On the policy pages, click "Back to Home" to return to `index.html`

### Step 4: Create a Blog Page (Optional)

The footer also links to `blog.html`. Here's a basic template:

**Create blog.html:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Blog - Fresh Feel Painting and Cleaning">
    <title>Blog - Fresh Feel Painting and Cleaning</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');
        
        * {
            font-family: 'Poppins', sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        .text-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-sm border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex items-center justify-between">
            <div class="flex items-center space-x-2">
                <div class="text-2xl font-bold text-gradient">
                    <i class="fas fa-paint-brush mr-2"></i>Fresh Feel
                </div>
            </div>

            <div class="hidden md:flex items-center space-x-8">
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Home</a>
                <a href="index.html#features" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Services</a>
                <a href="index.html#about" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
            </div>

            <div class="hidden md:block">
                <a href="tel:+15035551234" class="bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 px-6 py-2 rounded-lg font-semibold shadow-lg hover:shadow-xl">
                    Contact
                </a>
            </div>

            <button class="mobile-menu-button md:hidden text-white text-2xl hover:text-purple-400 transition-colors duration-300">
                <i class="fas fa-bars"></i>
            </button>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-bold mb-12">
                <span class="text-gradient">Blog</span>
            </h1>

            <div class="space-y-12">
                <!-- Blog Post Example -->
                <article class="bg-gray-800 rounded-lg p-8 border border-gray-700">
                    <h2 class="text-3xl font-bold mb-4 text-white">Your First Blog Post Title</h2>
                    <p class="text-gray-400 mb-4">Published on January 15, 2025</p>
                    <p class="text-gray-300 leading-relaxed mb-6">
                        This is where your blog post content goes. Share your expertise, tips, and insights about painting and cleaning services. Engaging content helps with SEO and keeps visitors on your site longer.
                    </p>
                    <a href="#" class="text-purple-400 hover:text-purple-300 transition-colors duration-300 font-semibold">
                        Read More <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </article>
            </div>

            <div class="mt-12 pt-8 border-t border-gray-700">
                <a href="index.html" class="inline-flex items-center gap-2 text-purple-400 hover:text-purple-300 transition-colors duration-300 font-semibold">
                    <i class="fas fa-arrow-left"></i> Back to Home
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center text-gray-500 text-sm">
                <p>&copy; 2025 Fresh Feel Painting and Cleaning. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Summary: File Structure After Setup

After completing these steps, your file structure should look like:

```
Your Website Folder/
├── index.html (main landing page)
├── privacy.html (privacy policy)
├── terms.html (terms of service)
└── blog.html (blog page)
```

All files should be in the same folder, and all links should work correctly.

---

## Troubleshooting Common Issues

Even with careful setup, you might encounter issues. Here are the most common problems and how to fix them.

### Issue 1: Links Don't Work

**Symptom**: Clicking a link does nothing or shows an error page.

**Common Causes and Solutions:**

**Cause A: Incorrect File Path**

If your files are in different folders, the path needs to reflect that.

**Example:**
If your files are organized like this:
```
Website/
├── index.html
└── pages/
    ├── privacy.html
    ├── terms.html
    └── blog.html
```

Your links should be:
```html
<a href="pages/privacy.html">Privacy Policy</a>
<a href="pages/terms.html">Terms of Service</a>
<a href="pages/blog.html">Blog</a>
```

**Cause B: Typo in File Name**

Make sure the file name in the href exactly matches the actual file name (including capitalization).

**Correct:**
```html
<a href="privacy.html">Privacy</a>  <!-- File is named "privacy.html" -->
```

**Incorrect:**
```html
<a href="Privacy.html">Privacy</a>  <!-- File is named "privacy.html" (lowercase) -->
```

**Cause C: Anchor Links Don't Match Section IDs**

If using `#` links, the href must match the section ID exactly.

**Correct:**
```html
<!-- Link -->
<a href="#features">Features</a>

<!-- Section -->
<section id="features">
    ...
</section>
```

**Incorrect:**
```html
<!-- Link -->
<a href="#feature">Features</a>

<!-- Section -->
<section id="features">
    ...
</section>
```

### Issue 2: Page Layout Breaks After Editing

**Symptom**: After changing text or CSS classes, the page looks wrong.

**Common Causes and Solutions:**

**Cause A: Accidentally Deleted HTML Tags**

HTML tags work in pairs. If you delete one, the other becomes useless.

**Example:**
```html
<!-- Correct -->
<p class="text-white">Your text here</p>

<!-- Incorrect - missing closing tag -->
<p class="text-white">Your text here
```

**Solution**: Check that every opening tag (`<`) has a matching closing tag (`</`).

**Cause B: Removed Tailwind Classes**

If you accidentally removed all classes from an element, it loses its styling.

**Example:**
```html
<!-- Correct -->
<div class="bg-gray-800 border border-gray-700 rounded-xl p-8">

<!-- Incorrect - no classes -->
<div>
```

**Solution**: Always keep the class attribute, even if you're just changing one class.

**Cause C: Syntax Error in Custom CSS**

If you modified the `<style>` section, a syntax error can break everything.

**Common Mistakes:**
- Missing semicolons: `color: red` should be `color: red;`
- Missing braces: `.class { color: red` should be `.class { color: red; }`
- Unclosed comments: `/* comment` should be `/* comment */`

**Solution**: Check the `<style>` section carefully for these errors.

### Issue 3: Text Overflows or Looks Cramped

**Symptom**: Text appears cut off or squeezed on certain screen sizes.

**Common Causes and Solutions:**

**Cause A: Removed Responsive Classes**

The page uses responsive prefixes (`sm:`, `md:`, `lg:`) to adjust sizing for different screens.

**Example:**
```html
<!-- Correct - adjusts size on different screens -->
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl">

<!-- Incorrect - same size on all screens -->
<h1 class="text-4xl">
```

**Solution**: Keep the responsive classes to ensure the page works on all devices.

**Cause B: Changed Padding or Margin Too Much**

If you increase padding too much, content might overflow.

**Example:**
```html
<!-- Too much padding -->
<div class="p-64">Content</div>

<!-- Better -->
<div class="p-8">Content</div>
```

**Solution**: Use reasonable spacing values (4, 6, 8, 12, 16, 24).

### Issue 4: Colors Look Wrong

**Symptom**: After changing colors, the page doesn't look right.

**Common Causes and Solutions:**

**Cause A: Text Color Blends with Background**

If you use the same color for text and background, it becomes invisible.

**Example:**
```html
<!-- Wrong - white text on white background -->
<p class="text-white bg-white">Text</p>

<!-- Correct - white text on dark background -->
<p class="text-white bg-gray-900">Text</p>
```

**Solution**: Ensure text color contrasts with the background color.

**Cause B: Used Wrong Color Name**

Tailwind color names are specific. Typos won't work.

**Correct Colors:**
```
purple-500, purple-600, purple-700
pink-500, pink-600, pink-700
gray-300, gray-400, gray-800, gray-900
```

**Incorrect:**
```
purple (should be purple-500)
dark-purple (should be purple-900)
light-gray (should be gray-300)
```

**Solution**: Check the Tailwind color names in the existing code and use those.

### Issue 5: Images Don't Display

**Symptom**: Image placeholders show instead of actual images.

**Common Causes and Solutions:**

**Cause A: Broken Image URL**

The page uses external images from Unsplash. If the URL is wrong, images won't load.

**Current Code:**
```html
<img src="https://images.unsplash.com/photo-1552321554-5fefe8c9ef14?w=600&h=600&fit=crop" alt="Fresh Feel Team">
```

**If the image doesn't load:**
1. Visit the URL directly in your browser
2. If it doesn't work, the image may no longer exist
3. Replace it with a different Unsplash image

**Example:**
```html
<!-- Find a new image on unsplash.com -->
<img src="https://images.unsplash.com/photo-1581092918056-0c4c3acd3789?w=600&h=600&fit=crop" alt="Professional painting">
```

**Cause B: Missing alt Text**

While this doesn't prevent the image from displaying, it's important for accessibility.

**Correct:**
```html
<img src="image.jpg" alt="Description of the image">
```

### Issue 6: Mobile Menu Doesn't Work

**Symptom**: Mobile menu button doesn't open the menu on phones.

**Common Causes and Solutions:**

**Cause A: JavaScript is Disabled**

The mobile menu requires JavaScript. Make sure you haven't removed the JavaScript code at the bottom of the page.

**Check that this code is still present (around line 640):**
```html
<script>
    document.addEventListener('DOMContentLoaded', function() {
        const mobileMenuButton = document.querySelector('header nav .mobile-menu-button');
        const mobileMenu = document.querySelector('header nav .mobile-menu');
        
        if (mobileMenuButton && mobileMenu) {
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
                // ...
            });
        }
    });
</script>
```

**Cause B: Mobile Menu Classes Changed**

The JavaScript looks for elements with specific class names. If you changed these, it won't work.

**Required Classes:**
- `.mobile-menu-button` - the hamburger icon
- `.mobile-menu` - the menu that appears
- `.hidden` - the class that hides the menu

**Solution**: Don't change these class names.

### Issue 7: Smooth Scrolling Doesn't Work

**Symptom**: Clicking anchor links doesn't smoothly scroll to sections.

**Common Causes and Solutions:**

**Cause A: Removed smooth-scroll CSS**

The page has this CSS (line 9):
```css
html {
    scroll-behavior: smooth;
}
```

If you removed this, smooth scrolling stops working.

**Solution**: Make sure this CSS rule is still in the `<style>` section.

**Cause B: Browser Doesn't Support It**

Some older browsers don't support smooth scrolling.

**Solution**: This is normal and not a problem—the page still works, just without smooth animation.

### Issue 8: FAQ Accordion Doesn't Expand

**Symptom**: Clicking FAQ questions doesn't show the answers.

**Common Causes and Solutions:**

**Cause A: JavaScript Code Removed**

The FAQ requires JavaScript to work. Check that this code is still present (around line 640):

```html
<script>
    const faqItems = document.querySelectorAll('.faq-item');
    faqItems.forEach(item => {
        const question = item.querySelector('.faq-question');
        if (question) {
            question.addEventListener('click', () => {
                // ...
            });
        }
    });
</script>
```

**Cause B: Changed FAQ HTML Structure**

The JavaScript looks for elements with specific classes:
- `.faq-item` - the container
- `.faq-question` - the question button
- `.faq-answer` - the answer content
- `.faq-icon` - the chevron icon

If you changed these classes, the accordion breaks.

**Solution**: Don't change these class names.

### Troubleshooting Checklist

Before asking for help, check:

- [ ] All HTML tags are properly closed (`<` and `>`)
- [ ] File names match exactly (including capitalization)
- [ ] File paths are correct for your folder structure
- [ ] All Tailwind class names are spelled correctly
- [ ] Haven't accidentally deleted important code
- [ ] JavaScript code is still present at the bottom
- [ ] External resources (fonts, icons, Tailwind) are loading

---

## Best Practices

Following these best practices will make maintaining your landing page easier and prevent common issues.

### 1. Always Keep Backups

Before making changes, save a backup copy.

**How to Backup:**
1. Right-click `index.html`
2. Click "Copy"
3. Right-click in the same folder
4. Click "Paste"
5. Rename to `index-backup.html`

Do this for all files before major changes.

### 2. Make One Change at a Time

Don't make multiple changes before testing.

**Good Practice:**
1. Change one thing
2. Save the file
3. Refresh the browser
4. Verify it works
5. Move to the next change

**Avoid:**
1. Change 10 things
2. Save
3. Refresh
4. Nothing works and you don't know why

### 3. Use Consistent Formatting

Keep your HTML formatted consistently for easy reading.

**Good Practice:**
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
    <div class="card-hover bg-gray-800 border border-gray-700 rounded-xl p-8">
        <h3 class="text-2xl font-bold mb-4">Title</h3>
        <p class="text-gray-300">Description</p>
    </div>
</div>
```

**Avoid:**
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8"><div class="card-hover bg-gray-800 border border-gray-700 rounded-xl p-8"><h3 class="text-2xl font-bold mb-4">Title</h3><p class="text-gray-300">Description</p></div></div>
```

### 4. Test on Multiple Devices

Always test your changes on different devices.

**Test on:**
- Desktop (large screen)
- Tablet (medium screen)
- Mobile phone (small screen)

**How to Test on Desktop:**
1. Open the page in your browser
2. Press F12 to open Developer Tools
3. Click the device toggle (top-left of the developer tools)
4. Select different devices from the dropdown

### 5. Keep External Links Updated

Regularly check that all external links still work.

**Links to Check:**
- Social media profiles
- Contact email
- Website URL
- External resources

### 6. Use Meaningful Text

Make text clear and specific.

**Good:**
```html
<p class="text-gray-300">We provide professional interior painting services with guaranteed satisfaction.</p>
```

**Avoid:**
```html
<p class="text-gray-300">We do stuff</p>
```

### 7. Maintain Consistent Branding

Keep colors, fonts, and messaging consistent throughout.

**Consistent Branding:**
- Use the same colors throughout
- Use the same company name
- Keep the same tone and voice
- Use the same logo

### 8. Document Your Changes

Keep notes of what you changed and when.

**Example:**
```
January 15, 2025 - Updated hero headline and company email
January 10, 2025 - Changed primary color from purple to teal
January 5, 2025 - Added new testimonial from Sarah Liu
```

### 9. Keep the Code Organized

Organize your code logically.

**Good Structure:**
```
1. Head section (metadata, styles)
2. Header/Navigation
3. Hero section
4. Features section
5. Benefits section
6. Testimonials section
7. About section
8. FAQ section
9. CTA section
10. Footer
11. JavaScript
```

### 10. Validate Your HTML

Periodically check your HTML for errors.

**Free HTML Validator:** https://validator.w3.org/

Simply paste your HTML code and click "Check" to see if there are any errors.

### 11. Optimize Images

Use appropriately sized images to improve page speed.

**Image Optimization Tips:**
- Use web-friendly formats (JPG, PNG, WebP)
- Compress images before uploading
- Use appropriate dimensions
- Provide alt text for accessibility

### 12. Monitor Performance

Regularly check how fast your page loads.

**Free Performance Tools:**
- Google PageSpeed Insights: https://pagespeed.web.dev/
- GTmetrix: https://gtmetrix.com/

These tools suggest improvements to make your page faster.

---

## Quick Reference Guide

### Common Tasks

#### Update Company Name
Find: `Fresh Feel`
Replace: `Your Company Name`
Click: Replace All

#### Update Phone Number
Find: `+15035551234`
Replace: `+1XXXXXXXXXX`
Click: Replace All

#### Update Email
Find: `iainhmunro@gmail.com`
Replace: `your-email@company.com`
Click: Replace All

#### Update Main Website URL
Find: `https://www.freshfeelpaintingandcleaning.ca/`
Replace: `https://www.yourwebsite.com`
Click: Replace All

#### Change Primary Color (Purple to Blue)
Find: `purple`
Replace: `blue`
Click: Replace All

#### Change Accent Color (Pink to Red)
Find: `pink`
Replace: `red`
Click: Replace All

#### Make Text Larger
Change: `text-lg` to `text-xl`
Or: `text-4xl` to `text-5xl`

#### Add More Spacing
Change: `gap-8` to `gap-12`
Or: `p-8` to `p-12`

#### Make Cards More Rounded
Change: `rounded-lg` to `rounded-2xl`
Or: `rounded-xl` to `rounded-3xl`

---

## Additional Resources

### Learning Resources

- **Tailwind CSS Documentation**: https://tailwindcss.com/docs
- **HTML Tutorial**: https://www.w3schools.com/html/
- **CSS Tutorial**: https://www.w3schools.com/css/
- **Font Awesome Icons**: https://fontawesome.com/icons

### Tools

- **Visual Studio Code** (Free Text Editor): https://code.visualstudio.com/
- **Sublime Text** (Paid Text Editor): https://www.sublimetext.com/
- **Notepad++** (Free Text Editor): https://notepad-plus-plus.org/
- **Color Picker**: https://htmlcolorcodes.com/

### Getting Help

If you encounter issues:

1. **Check the Troubleshooting Section** - Most common issues are covered above
2. **Validate Your HTML** - Use https://validator.w3.org/ to check for errors
3. **Check Browser Console** - Press F12 and look for error messages
4. **Search Online** - Search for your specific error message
5. **Ask for Help** - Share your code and describe the issue

---

## Conclusion

You now have a comprehensive guide for maintaining and customizing your Fresh Feel Painting and Cleaning landing page. Remember:

- **Start small** - Make one change at a time
- **Always backup** - Save copies before major changes
- **Test thoroughly** - Check your changes on different devices
- **Keep it simple** - Don't overcomplicate things
- **Ask for help** - When in doubt, consult the resources provided

Good luck with your landing page! With these tools and knowledge, you're well-equipped to keep your website fresh, professional, and effective.