# Accessibility Playground

This project demonstrates best practices for building accessible web pages using semantic HTML, ARIA attributes, and keyboard navigation techniques. The goal is to ensure the content is usable by as many people as possible, including those with disabilities.

## Features

### 1. Semantic HTML
- Used semantic elements like `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, and `<figure>` to structure the content meaningfully.
- Ensured headings (`<h1>` to `<h3>`) follow a logical order for better readability and screen reader support.

### 2. ARIA Attributes
- Added `aria-label` and `aria-labelledby` to provide additional context for screen readers.
- Used `role="region"` to define landmark regions for better navigation.
- Avoided unnecessary ARIA roles where native HTML elements already provide accessibility.

### 3. Keyboard Navigation
- Ensured all interactive elements (e.g., links, buttons) are focusable using the `Tab` key.
- Added `tabindex="0"` to ensure proper focus order for custom elements.
- Provided keyboard alternatives for mouse-based interactions using `onkeydown` events.

### 4. Accessible Forms
- Associated `<label>` elements with form inputs using the `for` attribute.
- Used `aria-describedby` to link inputs with additional instructions.
- Ensured error messages are clear and helpful.

### 5. Responsive Design
- Used Bootstrap 5 to create a responsive layout that works across devices.
- Applied utility classes like `container`, `row`, `col-*`, and `btn` for consistent styling.

## Key Sections

### Navigation
- **Main Navigation**: Includes links to key sections of the page with `aria-label="Main Navigation"` for screen readers.
- **Secondary Navigation**: Demonstrates the use of `aria-label` for additional navigation menus.

### Focusable Elements
- Demonstrates proper use of `tabindex` to ensure all elements are keyboard-accessible.
- Includes buttons and links styled with Bootstrap classes.

### Keyboard Alternatives
- Avoids `onmouseover` or `onclick` without keyboard alternatives.
- Provides `onkeydown` events to handle keyboard interactions (e.g., activating buttons with the `Enter` key).

### Accessible Forms
- Includes a form with labeled inputs and accessible instructions using `aria-describedby`.
- Ensures all form elements are focusable and usable with the keyboard.

