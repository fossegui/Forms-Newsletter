# Newsletter Subscription Page

A lightweight, responsive web page for a programming newsletter featuring a dynamic light/dark theme toggle and auto-updating copyright year.

## 🚀 Features

* **Dark/Light Mode Toggle:** Switches themes using CSS custom variables controlled via JavaScript.
* **Auto-Updating Year:** Dynamically inserts the current year into the footer.
* **Responsive Layout:** Flexbox and CSS Grid layout that adapts gracefully to different screen sizes.
* **Semantic HTML:** Built using proper semantic HTML5 tags (`<header>`, `<main>`, `<section>`, `<footer>`).

## 📁 File Structure

```text
├── index.html        # Main HTML structure
├── css/
│   └── styles.css    # Custom CSS styles and dynamic theme variables
└── js/
    └── app.js        # JavaScript for theme toggling and dynamic year insertion
```
🛠️ Key Components Explained

1. HTML (index.html)
Header (<header>): Contains the project title and the theme toggle button (#btnTema).

Subscription Form (<form>): Includes input fields for the user's name and email with clear visual labels.

Footer (footer): Contains a dynamic <span> tag (#ano) where the current year is populated via script.

Script Optimization: The JavaScript file is linked in the <head> using the defer attribute to ensure DOM elements load prior to script execution.

2. CSS (styles.css)
CSS Custom Properties (Variables): Standardized color scheme defined under :root for Light Mode and overridden under [data-tema="escuro"] for Dark Mode.

Flexbox Layout: Utilizes a sticky footer layout pattern (display: flex; flex-direction: column; min-height: 100vh;) keeping the footer anchored to the bottom.

Form Grid: Employs display: grid; gap: .5rem; on the form elements for consistent vertical spacing and alignment.

3. JavaScript (app.js)
Dynamic Year: Uses new Date().getFullYear() to automatically populate #ano in the footer.

Theme Switching Logic: Toggles the data-tema="escuro" attribute on the root HTML element (<html>) upon clicking the #btnTema button.---------------
