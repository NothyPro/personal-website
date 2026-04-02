# Personal Portfolio – Nothando Ruwona

This is the source code for my personal portfolio website, showcasing my work as a UX/UI design intern candidate and web development student. The site is designed to be clean, accessible, and visually engaging, with a focus on purposeful motion and usability.

🔗 **Live site:** [nothandoruwona.ca](https://nothandoruwona.ca)

---

## Technologies Used

- **HTML5** – Semantic markup for structure and accessibility.
- **CSS3** – Custom styling with CSS variables, Flexbox, Grid, and animations.
- **JavaScript (ES6)** – Mobile navigation toggle and smooth scrolling.
- **Font Awesome** – Icon library for social links and UI elements.
- **GitHub Pages** – Hosting via the `main` branch.

---

## CSS Techniques & Effects

### CSS Variables (Custom Properties)

Centralised theming for colours, shadows, and spacing, making the site easy to maintain and consistent across components.

```css
:root {
  --primary: #14213d;
  --accent: #fca311;
  --bg-body: #e5e5e5;
  /* ... */
}
```

### Responsive Layout
- **Flexbox** – Used in the navigation bar and contact links.
- **CSS Grid** – Powers the skills and projects sections with repeat(auto-fit, minmax(...)) for fluid columns.
- **Media Queries** – Adjusts layout, font sizes, and navigation for mobile devices.

### Smooth Transitions

All interactive elements such as buttons, skill cards, and navigation links use transitions to provide subtle visual feedback on hover, improving usability.

```
.skill-card {
  transition: transform 0.3s;
}

.btn:hover {
  background-color: var(--accent-dark);
}
```

### Keyframe Animation – Hero Section Fade and Slide-Up

A self-directed CSS animation that runs on page load. The hero content fades in and moves upward, drawing attention to the main message without being distracting.

```
@keyframes fadeSlideUp {
  0% {
    opacity: 0;
    transform: translateY(30px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

.hero-content {
  animation: fadeSlideUp 0.8s ease-out forwards;
}
```

This animation was built by referencing the MDN documentation on @keyframes and adapting the example to create a unique vertical fade-in effect.

### Box Shadows & Visual Hierarchy

Cards, images, and the navigation bar use subtle box shadows to create depth and separate content sections, enhancing readability.

## Accessibility Features
- **Semantic HTML** – Headings and landmarks such as <header>, <main>, and <footer> provide structure for screen readers.
- **Alt Text** – All images include descriptive alt attributes.
- **Focus States** – Interactive elements have visible focus outlines.
- **High Contrast** – Text colours meet WCAG contrast guidelines, such as dark text on light backgrounds and white text on dark hero backgrounds.
- **Keyboard Navigation** – All links and buttons are reachable via keyboard; the mobile menu can be toggled with Enter or Space.
- **Smooth Scrolling** – JavaScript-enabled smooth scrolling respects prefers-reduced-motion by falling back to an instant jump if motion is disabled.

## Aesthetic Choices
- **Colour Palette** – Prussian blue (#14213d) conveys professionalism; orange (#fca311) adds energy and is used sparingly for accents.
- **Typography** – Clean sans-serif fonts such as Segoe UI and system fallbacks ensure readability across devices.
- **Whitespace** – Generous padding and margins give content room to breathe.
- **Subtle Motion** – Hover lifts on cards and gentle fade-ins on load provide delight without overwhelming.
- **Responsive Images** – The hero background and portrait use the modern .avif format for efficient loading.

## Project Structure

/
├── index.html          # Main HTML document
├── css/
│   ├── reset.css       # CSS reset for cross-browser consistency
│   └── style.css       # All custom styles (variables, animations, layouts)
├── js/
│   └── script.js       # Mobile menu toggle and smooth scrolling
├── img/                # Images (hero background, portrait)
└── resume.pdf          # Downloadable resume

### Running Locally
Clone the repository.
Open index.html in any modern browser.
No build steps or dependencies are required.

### Credits & References
MDN Web Docs – Used to understand HTML, CSS, @keyframes, and CSS animations.
Font Awesome – Icons.

### License

© 2026 Nothando Tapuwanashe Ruwona. All rights reserved.

Questions? Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/nothando-tapuwanashe-ruwona-82b7b726a) or [GitHub](https://github.com/NothyPro)
