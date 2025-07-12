# JamSai Family Foundation Website Documentation

## Overview

The JamSai Family Foundation website is a static, multi-page site for a charity organization based in The Gambia. It is designed to inform visitors about the foundation's mission, showcase its programs and events, collect donations, and facilitate contact and volunteering.

---

## Table of Contents

1. [Structure](#structure)
2. [Key Features](#key-features)
3. [Technical Details](#technical-details)
4. [How to Update](#how-to-update)
5. [External Integrations](#external-integrations)
6. [Contact & Social](#contact--social)
7. [Miscellaneous](#miscellaneous)

---

## 1. Structure

### Main Pages

- **index.html**: Home page with overview, carousel, about, programs, causes, events, team, testimonials, contact, and footer.
- **about.html**: Detailed information about the foundation, its mission, vision, and current programs.
- **causes.html**: Highlights ongoing and future programs and initiatives.
- **event.html**: Lists upcoming charity events and testimonials.
- **donate.html**: Provides multiple ways to donate (ModemPay, Mobile Money, Bank Transfer) and encourages volunteering.
- **contact.html**: Contact form and foundation contact details.
- **volunteer.html**: Volunteer sign-up form and encouragement.
- **service.html, single.html, team.html**: Additional pages, likely for services, blog posts, and team details.

### Assets

- **css/style.css**: Main stylesheet, customizes Bootstrap and adds unique branding.
- **js/main.js**: Handles UI interactions (carousel, modals, counters, navigation, etc.).
- **lib/**: Third-party libraries (Bootstrap, FontAwesome, OwlCarousel, Animate.css, etc.).
- **img/**: All images used for the site (team, events, causes, etc.).
- **mail/**: Contact form validation and backend (PHP) for sending emails.

---

## 2. Key Features

### Navigation

- Responsive navbar with links to all main pages.
- Social media links (Facebook, Instagram, WhatsApp, news).

### Home Page (index.html)

- **Carousel**: Rotating banners with images and calls to action.
- **About Section**: Tabbed interface for About, Mission, and Programs.
- **Programs/Services**: Future and current initiatives (Cloth Donation, School Supply, Health Support).
- **Facts**: Animated counters for countries, volunteers, goals, and funds raised.
- **Causes**: Carousel of featured causes (Clean Water, Maternal Health, Youth Empowerment).
- **Events**: Upcoming events with images and descriptions.
- **Team**: Profiles of key team members with modal bios.
- **Testimonials**: Carousel of community feedback.
- **Contact**: Contact form and image.
- **Footer**: Contact info, quick links, newsletter, copyright.

### About Page

- Expanded about section with mission, vision, and detailed program descriptions.
- Facts about members, programs, funds raised, and people helped.

### Causes Page

- Details on current and future programs.
- Carousel of popular causes.

### Events Page

- Upcoming events with images and descriptions.
- Testimonials section.

### Donate Page

- Multiple donation methods (ModemPay, Mobile Money, Bank Transfer).
- Volunteer/partner call-to-action.
- Donation encouragement and form.

### Contact & Volunteer Pages

- Contact/volunteer forms with validation.
- Contact details and social links.

---

## 3. Technical Details

### Styling

- Uses Bootstrap 4 for layout and responsiveness.
- Custom colors: blue (#87CEEB), dark blue (#4a4c70), white backgrounds.
- Animations via Animate.css and custom CSS.

### JavaScript

- jQuery for DOM manipulation.
- OwlCarousel for carousels.
- CounterUp for animated counters.
- Parallax and Easing for visual effects.
- Custom scripts for modals, navigation, and form handling.

### Forms

- Contact and volunteer forms use jqBootstrapValidation for client-side validation.
- AJAX POST to `mail/contact.php` for backend email sending.
- EmailJS integration for some forms (API key in code).

### Images

- All images are stored in the `img/` directory and used for carousels, team, events, etc.

### Accessibility

- Uses semantic HTML and ARIA attributes for modals.
- Responsive design for mobile and desktop.

---

## 4. How to Update

### Content Updates
- **Text**: Edit the relevant HTML files for text changes.
- **Images**: Add new images to the `img/` directory and reference them in HTML.
- **Navigation**: Update the navbar links in all HTML files.

### Styling Updates
- **Custom Styles**: Update `css/style.css` for custom styles.
- **Bootstrap**: The site uses Bootstrap 4, so you can use Bootstrap classes.

### Functionality Updates
- **JavaScript**: Update `js/main.js` for custom JS functionality.
- **Forms**: Update `mail/contact.js` and `mail/contact.php` for form logic and backend email.

### Adding New Pages
1. Create a new HTML file following the existing structure.
2. Include the same header and footer as other pages.
3. Update the navigation in all pages to include the new link.

---

## 5. External Integrations

- **EmailJS**: For sending emails from the contact form.
- **OwlCarousel**: For carousels and sliders.
- **Bootstrap**: For layout and components.
- **FontAwesome**: For icons throughout the site.

---

## 6. Contact & Social

### Foundation Contact Information
- **Email**: jamsaifamilyfoundation@gmail.com
- **Phone**: +220 7438242 / 3799053
- **Location**: Gambia, West Africa

### Social Media Links
- **Facebook**: https://www.facebook.com/share/153FfkrMJL/
- **Instagram**: https://www.instagram.com/jamsai_foundation
- **WhatsApp**: https://wa.me/447887516012
- **News**: https://www.voicegambia.com/?s=jamsai

---

## 7. Miscellaneous

### Features
- Newsletter form in the footer (no backend logic by default).
- Pre-loader animation on page load.
- "Back to top" button for easy navigation.
- Team member bio modals with detailed information.

### Donation Methods
- **ModemPay**: Secure online payment system
- **Mobile Money**: Wave (3799053) and APS (7013415)
- **Bank Transfer**: AGIB BANK LTD - Account: 003101020236146164

### Programs
- **Clothing Reuse and Upcycling Campaign**: Collecting and distributing clean, gently used clothing
- **School Supply Campaign**: Providing essential school supplies to students
- **Ramadan Food Supply Campaign**: Food packages during the holy month of Ramadan

---

## File Structure

```
Jamsai/
├── index.html              # Home page
├── about.html              # About page
├── causes.html             # Causes/programs page
├── event.html              # Events page
├── donate.html             # Donation page
├── contact.html            # Contact page
├── volunteer.html          # Volunteer page
├── service.html            # Services page
├── team.html               # Team page
├── single.html             # Single post page
├── css/
│   └── style.css          # Main stylesheet
├── js/
│   └── main.js            # Main JavaScript file
├── img/                   # All website images
├── lib/                   # Third-party libraries
│   ├── animate/
│   ├── counterup/
│   ├── easing/
│   ├── flaticon/
│   ├── owlcarousel/
│   ├── parallax/
│   └── waypoints/
├── mail/                  # Contact form backend
│   ├── contact.js
│   ├── contact.php
│   └── jqBootstrapValidation.min.js
└── video.mp4              # Video file
```

---

## Development Notes

- The website is built as a static site using HTML, CSS, and JavaScript.
- All pages follow a consistent structure with shared header and footer.
- The site is responsive and works on mobile and desktop devices.
- Contact forms use both traditional PHP backend and EmailJS for redundancy.
- The design uses a blue color scheme (#87CEEB) with clean, modern styling.

---

## Credits

- **Designed By**: [Sundiata Keita](https://sundiata.gm/)
- **Foundation**: JamSai Family Foundation
- **Location**: Gambia, West Africa

---

*Last Updated: [Current Date]* 