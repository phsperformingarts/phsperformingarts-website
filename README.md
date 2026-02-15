# Philomath High School Performing Arts Website

Welcome to the Philomath High School Performing Arts website! This modern, professional website showcases our Jazz Band, Choir, and Wind Ensemble programs.

## Quick Start

The website consists of 7 HTML pages:
- **index.html** - Home page
- **general-info.html** - Program information and Remind 101
- **jazz-band.html** - Jazz Band details
- **choir.html** - Choir details
- **wind-ensemble.html** - Wind Ensemble details
- **calendar.html** - Events calendar
- **contact.html** - Contact information

## Editing Content

### Finding What to Edit

Look for comments in the HTML files that say `<!-- TO EDIT: -->`. These mark sections you can safely edit. The text you should change is between HTML tags.

**Example:**
```html
<!-- TO EDIT: Update band director information -->
<p><strong>Name:</strong> [Director Name]</p>
```

Change to:
```html
<!-- TO EDIT: Update band director information -->
<p><strong>Name:</strong> John Smith</p>
```

### Updating Text Content

1. Open the appropriate HTML file in a text editor (Notepad++, VS Code, or even Notepad)
2. Find the section marked with `<!-- TO EDIT: -->`
3. Update the text between the HTML tags
4. Save the file
5. Refresh your web browser to see the changes

### Adding Calendar Events

**File:** `calendar.html`

1. Find the `<tbody>` section in the table
2. Copy an existing row:
```html
<tr>
    <td>March 15, 2026</td>
    <td>Spring Concert</td>
    <td>All Ensembles</td>
    <td>PHS Auditorium</td>
</tr>
```
3. Paste it below and update the information
4. Save the file

### Updating Contact Information

**File:** `contact.html`

Find each contact card and update the bracketed placeholders:
- `[Director Name]` - Replace with actual name
- `[email]` - Replace with actual email address
- `[Phone Number]` - Replace with actual phone number
- `[Street Address]` - Replace with actual address
- `[ZIP Code]` - Replace with actual ZIP code

### Updating Rehearsal Schedules

**Files:** `jazz-band.html`, `choir.html`, `wind-ensemble.html`

Find the Rehearsal Schedule section and replace:
- `[Add days here]` - e.g., "Monday, Wednesday, Friday"
- `[Add time here]` - e.g., "3:00 PM - 4:30 PM"

### Adding Images

#### Hero Images (Top of Each Page)

1. Place your image file in `assets/images/backgrounds/`
2. Name it appropriately (e.g., `hero-jazz.jpg`, `hero-choir.jpg`)
3. In the HTML file, update the background-image URL:

```html
<div class="heading-content" style="background-image: url('./assets/images/backgrounds/hero-jazz.jpg');">
```

**Recommended image size:** 1920x600 pixels, JPEG format, compressed to ~200KB

#### Content Images

1. Place image in `assets/images/`
2. Add to HTML where you want it to appear:

```html
<img src="./assets/images/your-photo.jpg" alt="Description" class="img-responsive">
```

### Changing Colors

**File:** `css/styles.css`

1. Open `css/styles.css`
2. Find the `:root` section at the top (around line 17-27)
3. Modify the color hex codes:

```css
:root {
    --warriors-orange: #ff6600;    /* Navigation, headers */
    --warriors-black: #1a1a1a;     /* Dark sections, text */
    --accent-yellow: #FDD10C;      /* Buttons, highlights */
    --light-cream: #faefcf;        /* Light backgrounds */
    --off-white: #F4F4F4;          /* Main background */
}
```

4. Save and refresh your browser

## File Structure

```
phs-website/
├── index.html                  # Home page
├── general-info.html           # Program information
├── jazz-band.html             # Jazz Band page
├── choir.html                 # Choir page
├── wind-ensemble.html         # Wind Ensemble page
├── calendar.html              # Events calendar
├── contact.html               # Contact information
├── css/
│   └── styles.css             # All styling
├── js/
│   └── script.js              # Interactive features
├── assets/
│   ├── images/
│   │   ├── backgrounds/       # Hero images for each page
│   │   └── logo/              # School logo
│   └── icons/                 # Favicon and icons
└── README.md                  # This file
```

## Tips for Editing

### DO:
✅ Change text between HTML tags
✅ Update bracketed placeholders like `[Director Name]`
✅ Add images to the `assets/images/` folder
✅ Copy/paste table rows for new calendar events
✅ Test changes by opening the HTML file in a web browser

### DON'T:
❌ Delete HTML tags like `<p>`, `<div>`, `<section>`
❌ Remove CSS class names (e.g., `class="contact-card"`)
❌ Edit the navigation menu structure
❌ Change the Bootstrap CDN links
❌ Modify the `<!-- TO EDIT: -->` comments (they help you find sections)

## Common Tasks

### Task 1: Update All Contact Information
1. Open `contact.html`
2. Find the three contact cards (Band Director, Choir Director, School Address)
3. Replace all bracketed placeholders
4. Save the file

### Task 2: Add an Event to the Calendar
1. Open `calendar.html`
2. Find the `<tbody>` section
3. Copy an existing `<tr>` row
4. Paste it and update the date, event, ensemble, and location
5. Save the file

### Task 3: Update Rehearsal Schedule
1. Open the appropriate file (`jazz-band.html`, `choir.html`, or `wind-ensemble.html`)
2. Find "Rehearsal Schedule"
3. Update days, time, and location
4. Save the file

### Task 4: Replace Hero Images
1. Find/create a performing arts photo (1920x600px recommended)
2. Save it to `assets/images/backgrounds/` with a descriptive name
3. Open the appropriate HTML file
4. Find the `<div class="heading-content"` line
5. Update the `background-image: url(...)` path
6. Save and test

## Technical Details

### Built With
- **Bootstrap 4.5.0** - Responsive CSS framework
- **jQuery 3.5.1** - JavaScript library for Bootstrap
- **Custom CSS** - Warriors orange/black color scheme
- **Vanilla JavaScript** - Auto-updating copyright year and active page highlighting

### Features
- ✅ Fully responsive (works on desktop, tablet, mobile)
- ✅ Fixed navigation bar with dropdown menus
- ✅ Professional hero sections with background images
- ✅ Alternating section backgrounds for visual interest
- ✅ Auto-updating copyright year
- ✅ Active page highlighting in navigation
- ✅ Warriors orange (#ff6600) and black (#1a1a1a) color scheme
- ✅ Easy-to-edit content with clear markers

### Browser Support
- Chrome (recommended)
- Firefox
- Safari
- Edge
- Modern browsers with JavaScript enabled

## Getting Help

### For Content Updates
Contact the band or choir directors

### For Technical Issues
Contact Philomath High School IT Department

### For Website Hosting
This website can be hosted on any web server. Simply upload all files maintaining the folder structure.

## Backup

**Important:** Before making major changes, create a backup:
1. Copy the entire `phs-website` folder
2. Rename it to `phs-website-backup-[date]`
3. Make your changes to the original
4. If something breaks, restore from backup

---

**Last Updated:** February 2026
**Version:** 2.0 (Multi-page redesign)
**Based on:** PHRED Robotics Website Framework

For questions about using this website, please refer to this README or contact your IT department.
