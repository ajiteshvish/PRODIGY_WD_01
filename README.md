# PRODIGY_WD_TASK_01

# Interactive Navigation Menu

This project demonstrates an **Interactive Navigation Menu** built using HTML, CSS, and JavaScript. The menu has dynamic features such as hover effects, color changes when scrolling, and a fixed position to ensure it remains visible on all pages.

## Features

- **Fixed Navigation Bar**: The navigation bar stays at the top of the viewport while scrolling.
- **Scroll-Based Interactivity**: The background color of the navigation bar changes when the user scrolls.
- **Hover Effects**: Menu items change color when hovered over.
- **Responsive Design**: The menu adapts to different screen sizes.
- **Footer**: Includes a copyright notice for Ajitesh Vishwakarma.

## Project Structure

The project consists of three main files:

1. **`index.html`**: Contains the structure of the navigation menu and webpage content.
2. **`styles.css`**: Provides styling for the navigation bar, hover effects, sections, and footer.
3. **`script.js`**: Adds interactivity, such as detecting scroll events and changing the navbar style dynamically.

---

## File Details

### `index.html`

This file contains the basic structure of the webpage:

- A `header` element for the navigation bar.
- Multiple `section` elements for the webpage content.
- A `footer` element displaying the copyright notice.

#### Key Snippet:
```html
<header id="navbar" class="navbar">
  <nav>
    <ul class="nav-menu">
      <li class="nav-item"><a href="#home">Home</a></li>
      <li class="nav-item"><a href="#about">About</a></li>
      <li class="nav-item"><a href="#services">Services</a></li>
      <li class="nav-item"><a href="#portfolio">Portfolio</a></li>
      <li class="nav-item"><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>
```

---

### `styles.css`

This file contains styles for the navigation menu, sections, and footer:

- **Navbar**: Styled with a dark background and white text. Includes a hover effect to change text color.
- **Scroll Interaction**: The `scrolled` class dynamically changes the navbar's background color.
- **Sections**: Each section has a unique background color to differentiate content visually.
- **Footer**: Displays copyright information with a fixed position at the bottom.

#### Key Snippet:
```css
.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  background-color: #333;
  display: flex;
  justify-content: center;
  padding: 10px 0;
  z-index: 1000;
  transition: background-color 0.3s ease;
}

.navbar.scrolled {
  background-color: #555;
}
```

---

### `script.js`

This file adds interactivity using JavaScript:

- Detects the user's scroll position with the `scroll` event listener.
- Adds or removes the `scrolled` class from the navbar to dynamically update its background color.

#### Key Snippet:
```javascript
window.addEventListener("scroll", () => {
  const navbar = document.getElementById("navbar");
  if (window.scrollY > 50) {
    navbar.classList.add("scrolled");
  } else {
    navbar.classList.remove("scrolled");
  }
});
```

---

## How to Run

1. Clone this repository or download the files.
2. Open the `index.html` file in your web browser.
3. Scroll and hover over the menu items to see the interactivity.

---

## Screenshots

### Navigation Menu (Default)
![img_1](#)

### Navigation Menu (Scrolled)
![img_2](#)

---

## Acknowledgment

This project was created as part of the Web Development Internship Program at **Prodigy InfoTech**.

**Author:** Ajitesh Vishwakarma  





