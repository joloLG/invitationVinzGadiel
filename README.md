# Christening Invitation Website

A beautiful, premium, mobile-first Christening Invitation website designed primarily for Android smartphones.

## Image Assets Required

Place the following image files in the root directory:

### Baby
- `baby.png` - The baby's photo (will be displayed in a circular frame)

### Clouds
- `cloud1.png` - Decorative cloud element

## Features

- **Cinematic Entrance**: WOW opening sequence with staggered fade, scale, blur, and glow animations
- **Vertical Storytelling**: Scroll-triggered animations for each section (Welcome, Christening, Event Details, Parents, Godparents, Message)
- **Parallax Effects**: Subtle parallax on clouds and decorations
- **Performance Optimized**: GPU-friendly transform/opacity animations for smooth Android performance
- **Fully Responsive**: Optimized for 360px-430px Android screens, scales to desktop
- **Accessible**: ARIA attributes, keyboard navigation, reduced motion support, skip links
- **Loading Screen**: Elegant loading experience with floating clouds

## Sections

1. **Hero**: Baby portrait, name, date/time with cinematic entrance
2. **Welcome**: Multi-line animated invitation message
3. **The Christening**: Baptism introduction with clouds, teddy, heavenly light
4. **Event Details**: DATE, TIME, CHURCH, RECEPTION with elegant cards
5. **Parents**: Romantic display with parents' names
6. **Godparents**: Card-based layout with teddy decorations
7. **Message**: Heartfelt quote-style layout
8. **Final**: Grand finale with balloons, particles, and interactive buttons

## Customization

The invitation is designed to be easily customizable. Edit the `INVITATION_CONFIG` object in `index.html` (lines 12-46) to change:

```javascript
const INVITATION_CONFIG = {
    baby: {
        firstName: 'Vinz',
        lastName: 'Gadiel',
        fullName: 'Vinz Gadiel'
    },
    event: {
        date: 'Sunday, January 15, 2026',
        time: '10:00 AM',
        church: '[Church Name]',
        churchAddress: '[Church Address]',
        reception: '[Reception Venue]',
        receptionAddress: '[Reception Address]'
    },
    parents: {
        father: '[Father\'s Name]',
        mother: '[Mother\'s Name]'
    },
    godparents: {
        godfather: '[Godfather\'s Name]',
        godmother: '[Godmother\'s Name]'
    },
    contact: {
        rsvpDate: '[RSVP Date]',
        phone: '[Phone Number]',
        email: '[Email Address]'
    },
    designer: {
        name: 'John Lloyd Gracilla'
    }
};
```

Update the HTML placeholders with your actual information:
- Event section: Replace `[Date]`, `[Time]`, `[Church Name]`, `[Reception Venue]`
- Parents section: Replace `[Father's Name]`, `[Mother's Name]`
- Godparents section: Replace `[Godfather's Name]`, `[Godmother's Name]`
- Final section: Replace `[Father's Name] & [Mother's Name]`

## Required Image Assets

Place these images in the project root directory:

- `baby.png` - Baby portrait (recommended: 400x400px or larger)
- `cloud1.png` - Cloud decoration
- `cloud2.png` - Cloud decoration (different shape)
- `cloud3.png` - Cloud decoration (different shape)
- `teddy1.png` - Teddy bear decoration
- `teddy2.png` - Teddy bear decoration (different pose)
- `teddy3.png` - Teddy bear decoration (different pose)

*Note: Placeholder SVG images are included for immediate preview. Replace them with your actual images.*

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Custom properties, animations, flexbox, grid
- **JavaScript (Vanilla)**: Intersection Observer API, scroll events, no frameworks
- **Google Fonts**: Great Vibes (script), Cormorant Garamond (serif), Inter (sans-serif)

## Performance

- Uses `transform` and `opacity` for GPU-accelerated animations
- `will-change` hints for smooth rendering
- Reduced motion support for accessibility
- Optimized for Android mobile performance
- No external JavaScript libraries

## Accessibility

- Semantic HTML structure
- ARIA attributes for decorative elements
- Skip to main content link
- Keyboard accessible buttons
- Focus styles for navigation
- Reduced motion support via `prefers-reduced-motion`
- High contrast mode support
- Proper alt text for meaningful images

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (Android Chrome, iOS Safari)

## File Structure

```
invitation/
├── index.html          # Main HTML file with configuration
├── styles.css          # All styles and animations
├── README.md           # This file
├── baby.png            # Baby portrait
├── cloud1.png          # Cloud decoration
├── cloud2.png          # Cloud decoration
├── cloud3.png          # Cloud decoration
├── teddy1.png          # Teddy bear decoration
├── teddy2.png          # Teddy bear decoration
└── teddy3.png          # Teddy bear decoration
```

## Deployment

Simply upload all files to any static hosting service:
- GitHub Pages
- Netlify
- Vercel
- Any web server

## License

This project is created for personal use. Feel free to customize for your own Christening invitation.

## Credits

Designed by John Lloyd Gracilla
