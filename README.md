# Christening Invitation - Vinz Gadiel

A beautiful, premium, mobile-first Christening Invitation website optimized for Android mobiles with a magical, elegant, and joyful theme using pure HTML and CSS, featuring sophisticated animations and a vertical interactive storytelling experience.

## Features

- **Cinematic Entrance**: WOW opening sequence with staggered fade, scale, blur, and glow animations
- **Vertical Storytelling**: Scroll-triggered animations for each section (Welcome, Christening, Event Details, Location Guide, Parents, Health Protocols, Gift Guide, Dress Code, Message)
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
5. **Location Guide**: Visual journey from church to reception with animated pathway
6. **Parents**: Romantic display with parents' names
7. **Health Protocols**: Friendly health guidelines with icons (kiss, smoke, sanitize, mask)
8. **Gift Guide**: Gift suggestions with product images and QR code for monetary gifts
9. **Dress Code**: Color palette display (WHITE → SKY BLUE)
10. **Message**: Heartfelt quote-style layout
11. **Final**: Grand finale with balloons, particles, and interactive buttons

## Customization

The invitation is designed to be easily customizable. Edit the `INVITATION_CONFIG` object in `index.html` (lines 12-78) to change:

```javascript
const INVITATION_CONFIG = {
    baby: {
        firstName: 'Vinz',
        lastName: 'Gadiel',
        fullName: 'Vinz Gadiel'
    },
    event: {
        date: 'October 05 2026',
        day: 'Monday',
        time: '11 AM',
        church: '[Church Name]',
        churchAddress: '[Church Address]',
        reception: '[House / Reception Name]',
        receptionAddress: '[Reception Address]'
    },
    parents: {
        father: '[Father\'s Name]',
        mother: '[Mother\'s Name]'
    },
    location: {
        church: '[Church Name]',
        house: '[House / Reception Name]'
    },
    healthProtocols: {
        kiss: {
            title: 'Please Do Not Kiss Baby\'s Face',
            message: 'Please avoid kissing the baby\'s face. Let\'s help protect our little one from unwanted germs.'
        },
        smoke: {
            title: 'No Smoking or Vaping',
            message: 'For baby\'s comfort and safety, please keep the celebration smoke-free and avoid smoking or vaping near the baby.'
        },
        sanitize: {
            title: 'Please Sanitize Your Hands',
            message: 'Please sanitize your hands before touching or holding the baby. Thank you for helping us keep our little one safe.'
        },
        mask: {
            title: 'Please Wear a Face Mask',
            message: 'When needed, please wear a face mask when interacting closely with the baby. We truly appreciate your care and consideration.'
        }
    },
    gifts: {
        johnsons: {
            name: 'Johnsons Baby Bath Cleanser',
            description: 'A gentle baby bath cleanser for keeping our little one\'s bath time fresh, clean, and comfortable.'
        },
        unilove: {
            name: 'Unilove Baby Clothes Detergent',
            description: 'A baby-friendly laundry essential for keeping little clothes fresh and clean.'
        },
        wipes: {
            name: 'Poomsoft Unscented Wipes',
            description: 'Unscented wipes are a practical everyday essential for our little one.'
        },
        diaper: {
            name: 'Kukumi Diaper XL',
            description: 'Diapers are always a thoughtful and useful gift for our growing little one.'
        }
    },
    designer: {
        name: 'John Lloyd Gracilla'
    }
};
```

Update the HTML placeholders with your actual information:
- Event section: Replace `[Church Name]`, `[House / Reception Name]`
- Location Guide section: Replace `[Church Name]`, `[House / Reception Name]`
- Parents section: Replace `[Father's Name]`, `[Mother's Name]`
- Final section: Replace `[Father's Name] & [Mother's Name]`

## Required Image Assets

Place these images in the project root directory:

### Baby
- `baby.png` - Baby portrait (recommended: 400x400px or larger)

### Clouds
- `cloud1.png` - Cloud decoration
- `cloud2.png` - Cloud decoration (different shape)
- `cloud3.png` - Cloud decoration (different shape)

### Teddy Bears
- `teddy1.png` - Teddy bear decoration
- `teddy2.png` - Teddy bear decoration (different pose)
- `teddy3.png` - Teddy bear decoration (different pose)

### Health Protocol Icons
- `kiss.png` - No kissing icon
- `smoke.png` - No smoking icon
- `sanitize.png` - Hand sanitizer icon
- `mask.png` - Face mask icon

### Gift Guide Images
- `johnsons.png` - Johnsons Baby Bath Cleanser
- `unilove.png` - Unilove Baby Clothes Detergent
- `wipes.png` - Poomsoft Unscented Wipes
- `diaper.png` - Kukumi Diaper XL
- `qrgcash.png` - QR code for monetary gifts

### Location Guide
- `church.png` - Church location image
- `pathway.png` - Pathway from church to reception
- `house.png` - House/reception location image

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
├── teddy3.png          # Teddy bear decoration
├── kiss.png            # Health protocol icon
├── smoke.png           # Health protocol icon
├── sanitize.png        # Health protocol icon
├── mask.png            # Health protocol icon
├── johnsons.png        # Gift image
├── unilove.png         # Gift image
├── wipes.png           # Gift image
├── diaper.png          # Gift image
├── qrgcash.png         # QR code for monetary gifts
├── church.png          # Location image
├── pathway.png         # Location image
└── house.png           # Location image
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
