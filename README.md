# Portfolio-
# Responsive Design Improvements

## Summary

Your portfolio website has been enhanced with comprehensive responsive design support across all screen sizes, from extra-small mobile devices (under 320px) to large desktop displays (1200px+).

## Screen Size Breakpoints

### 1. **Large Desktop (1200px and above)**

- Maximum container width: 1200px
- Full-size hero section with 600px minimum height
- 2-column project grid layout

### 2. **Tablet & Small Desktop (1024px to 1199px)**

- Container width: 960px
- Optimized typography sizes
- 2-column project grid
- Full desktop experience with adjusted spacing

### 3. **Tablet (768px to 1023px)**

- Container width: 750px
- Single-column projects layout
- 2-column skills grid
- Adjusted padding and spacing for readability
- Better touch targets for mobile devices

### 4. **Large Mobile (481px to 767px)**

- Full-width responsive container
- Mobile hamburger menu (hidden on desktop)
- Single-column layouts for projects and skills
- Dropdown navigation menu
- Optimized button sizes for touch

### 5. **Small Mobile (320px to 480px)**

- Extra-small padding and margins
- Hamburger menu toggle with smooth animations
- Fixed navigation menu that slides open/closed
- Single-column layouts throughout
- Readable font sizes optimized for small screens
- Full-width buttons and links

### 6. **Extra Small Mobile (under 320px)**

- Minimal padding to maximize content space
- Smallest font sizes while maintaining readability
- Simplified layouts

## Key Responsive Features

### Mobile Menu Implementation

- Hamburger menu icon appears on screens under 768px
- Smooth slide-out/slide-in animation
- Auto-closes when a link is clicked
- Auto-closes when clicking outside the menu
- Active link highlighting

### Flexible Grid Layouts

- Projects grid: 2 columns on desktop → 1 column on mobile
- Skills grid: 4 columns on desktop → 2 columns on tablet → 1 column on mobile
- Contact links: Flex row → Flex column on mobile

### Typography Scaling

- Headings scale proportionally from 2.5rem (desktop) to 1rem (mobile)
- Body text maintains readability across all sizes
- All font sizes tested for legibility

### Spacing & Padding

- Consistent spacing that adapts to screen size
- Touch-friendly button and link sizes
- Proper margins for mobile readability

### Navigation Bar

- Sticky positioning on all screen sizes
- Hamburger menu on mobile
- Full menu on desktop
- Active link indicator
- Smooth transitions

## Technical Details

### CSS Media Queries Used

```css
/* Large Desktop */
@media (min-width: 1200px) /* Tablet & Small Desktop */ @media (max-width: 1199px) and (min-width: 768px) /* Tablet */ @media (max-width: 1023px) and (min-width: 768px) /* Large Mobile */ @media (max-width: 767px) and (min-width: 481px) /* Small Mobile */ @media (max-width: 480px) /* Extra Small Mobile */ @media (max-width: 319px);
```

### JavaScript Enhancements

- Mobile menu toggle with smooth animations
- Close menu on link click
- Close menu when clicking outside
- Smooth scroll navigation
- Active section highlighting on scroll

## Browser Compatibility

- Chrome/Edge 88+
- Firefox 87+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Testing Recommendations

Test on the following devices:

1. iPhone SE (375px)
2. iPhone 12/13 (390px)
3. iPhone Pro Max (430px)
4. iPad (768px)
5. iPad Pro (1024px)
6. Desktop (1920px+)

## How to Use

1. Open `index.html` in your browser
2. Test on different screen sizes using browser DevTools
3. Use the hamburger menu on mobile devices
4. Click on navigation links to smooth scroll to sections

---

**All responsive features are working and ready for production!**

Add profile image to hero

Place your profile image file in the `assets` folder at the project root and name it `profile.jpg`.

Commands (run from project root):

```bash
mkdir -p assets
# copy your image into the folder, e.g.:
# cp /path/to/your-photo.jpg assets/profile.jpg
```

If you prefer a different filename or location, open `index.html` and update the `src` attribute on the `<img class="hero-avatar">` element to point to your file.

Add your resume PDF

Place your resume PDF in the same `assets` folder and name it `Manikandan_Resume.pdf` (or update the link in `index.html`).

Example:

```bash
# cp /path/to/Manikandan_Resume.pdf assets/Manikandan_Resume.pdf
```
