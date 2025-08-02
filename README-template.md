# Frontend Mentor - REST Countries API with color theme switcher solution

This is a solution to the [REST Countries API with color theme switcher challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/rest-countries-api-with-color-theme-switcher-5cacc469fec04111f7b848ca). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View all countries fetched from the REST Countries API
- Search for a country using a keyword input
- Filter countries based on regions (e.g., Africa, Asia)
- View detailed information of a selected country on a separate page
- Explore bordering countries by clicking on their names in the detail view
- Toggle between dark and light themes (optional feature)

### Screenshot

![](./screenshot.jpg)


### Links

- Live Site URL: [https://your-live-site-url.com](http://127.0.0.1:5500/project_5/Country_part_1/Country_part_2/index.html)

## My process

### Built with

- HTML5
- CSS3
- JavaScript (ES6+)
- [REST Countries API](https://restcountries.com/)
- Responsive Design Principles
- Theme toggling using CSS variables
- LocalStorage for persisting theme state

### What I learned

This project helped me understand how to:

- Fetch and manipulate API data dynamically
- Handle asynchronous operations using `async/await`
- Implement client-side routing/navigation
- Use `localStorage` to persist user preferences (like dark mode)
- Apply CSS custom properties for theme switching
- Create reusable and modular code structure

```js
const fetchCountries = async () => {
  try {
    const response = await fetch('https://restcountries.com/v3.1/all');
    const data = await response.json();
    displayCountries(data);
  } catch (error) {
    console.error('Error fetching countries:', error);
  }
};
````

### Continued development

In future iterations, I would like to:

* Add animations for theme switching
* Improve accessibility (ARIA roles and keyboard navigation)
* Implement pagination for performance with large data
* Migrate to a frontend framework like React or Vue

### Useful resources

* [REST Countries API Documentation](https://restcountries.com/) – for understanding API data structure.
* [CSS-Tricks: Dark Mode](https://css-tricks.com/a-complete-guide-to-dark-mode-on-the-web/) – helped implement theme switching.
* [MDN Web Docs](https://developer.mozilla.org/) – reference for JavaScript, CSS, and DOM operations.

## Author

* GitHub – [sohammorchapure](https://github.com/sohammorchapure)

## Acknowledgments

Thanks to Frontend Mentor for providing this project. Also, gratitude to online communities and dev articles that guided parts of this implementation.


📝 **To use it**:
1. Open `README-template.md` in your repo.
2. Delete the existing content.
3. Paste the above content.
4. Save and commit:
   ```bash
   git add README-template.md
   git commit -m "Updated README template with project details"
   git push origin main

