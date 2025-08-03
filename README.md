# 💼 Wycliffe Mitunda — Personal Portfolio Website

Welcome to my personal portfolio website built with **HTML and CSS only** as part of a hackathon challenge. This project showcases my web development skills, projects, education, and contact information in a clean and responsive design.


## 🚀 Live Demo

 View Live Site https://babulele.github.io/My-portfolio-website/


## 📱 Responsive Preview

| Desktop View | Mobile View |
|--------------|-------------|
| ![Desktop Preview](./images/Desktop%20view.PNG) | ![Mobile Preview](/images/mobile%20view.PNG) |

*Screenshots are located in the `/screenshots/` directory.*

---

# Features

- Fully responsive layout using pure HTML & CSS
- Sectioned layout: About, Projects, Education, Contact
- Accessible, keyboard-navigable form
- CV download functionality
- Clean, semantic code structure

---

# Accessibility Audit Results

Audit performed using **Lighthouse (Chrome DevTools)**:

| Category       | Score   |
|----------------|---------|
| Performance    | 100 ✅  |
| Accessibility  | 100 ✅  |
| Best Practices | 100 ✅  |
| SEO            | 100 ✅  |

### ✔️ Accessibility Highlights

- All heading tags follow a logical structure (H1 > H2 > H3)
- Buttons and links have proper labels and roles
- Sufficient contrast between text and background
- Form elements include associated `<label>` tags

---

## 💡 Code Comments for Complex CSS

You’ll find **inline comments** in `style.css` explaining:

- **Responsive Layouts**: Use of `@media queries` for mobile/tablet/desktop breakpoints
- **Animations & Transitions**: Smooth hover effects, entrance animations using `transform` and `transition`
- **Navigation & Layout**: CSS Flexbox for aligning navbar, contact form, and grid-based project layout
- **Underline Alignment**: Custom `::after` pseudo-elements for consistent underline styling across sections
- **Download Button Centering**: Flexbox utilities applied to parent containers to center elements

Example:
```css
/* Project section underline */
#projects h2::after {
  content: '';
  display: block;
  width: 60px;
  margin: 8px auto;
  border-bottom: 3px solid #00bcd4; /* Accent color */
}
