# Solar System Explorer

An interactive educational website designed to explore the Solar System, learn about the eight planets, and understand their positions and movements around the Sun!

This project is designed for anyone interested in astronomy who wants to learn about our planetary neighborhood through interactive visualizations rather than static information alone. Users can watch the planets orbit the Sun, adjust animation speed, reveal planet labels, access scientific facts, and test their knowledge through an integrated quiz. The entire website is built using HTML, CSS, and JavaScript, combining web page structure, visual styling, and interactive programming into a single file, making it accessible to run and modify without installing additional software or external libraries.

# Quick Start:

If you want to explore this website, open the `solarsystem.html` file in a modern web browser such as Google Chrome, Microsoft Edge, or Firefox. Simply double-clicking the file should launch the website, allowing you to access the interactive Solar System visualization, planet information, and knowledge quiz immediately.

If you want to publish the project online, you can upload the file to a GitHub repository and enable **GitHub Pages** in the repository's settings. This allows you to share the website through a public link that others can access without downloading the source code.

# Core Features:

**Interactive Solar System Visualization** Built using HTML elements and CSS positioning, the visualization displays the Sun at the center with eight planets arranged around it. Circular orbit paths provide a visual reference for planetary movement, while individual CSS styles distinguish each planet through its size and color. Saturn includes a custom CSS pseudo-element to represent its ring system. The visualization is designed for educational purposes, with orbital distances, sizes, and speeds represented as visual approximations rather than exact astronomical scale.

**Dynamic Planetary Animation Engine** Utilizes JavaScript's `requestAnimationFrame()` function to continuously update the position of each planet. Trigonometric functions, including `Math.cos()` and `Math.sin()`, calculate horizontal and vertical positions along circular paths around the Sun. Each planet is assigned an individual orbital radius, speed, and starting angle, allowing the animation to represent different planetary movement rates while keeping the Sun at the center.

**Real-Time Animation Controls** Features interactive controls that allow users to pause or resume planetary movement, adjust animation speed to 0.5×, 1×, 2×, or 4×, and toggle planet labels on or off. JavaScript event listeners respond to button clicks and selection changes, updating the animation and interface without reloading the webpage.

**Dynamic Planet Information System** Stores planetary information in a structured JavaScript object containing each planet's classification, diameter, day length, moon information, and a scientific fact. A reusable `showPlanet()` function updates the information panel whenever a user selects a planet. The Sun is also interactive and displays its own information, allowing users to explore the central star as well as the eight planets.

**Automated Star Generation** Creates 100 stars dynamically using JavaScript's `document.createElement()` and `Math.random()` functions. Each star receives a randomized horizontal position, vertical position, and opacity, producing a varied background without requiring external image files. The stars are generated when the page loads and remain in place while the planetary animation runs.

**Dynamic Planet Index** Automatically generates a planet directory from the same JavaScript data object used by the information system. Using `Object.keys()` and `forEach()`, the website creates an individual entry for each planet, displaying its name and classification. Selecting an entry updates the information panel and smoothly scrolls the page back to the interactive visualization, connecting the reference directory with the main exploration interface.

**Knowledge Assessment and Scoring System** Implements an interactive multiple-choice quiz containing four astronomy questions about planetary size, planetary identification, Saturn's rings, and distance from the Sun. JavaScript stores the questions, answer choices, and correct answers in an array of objects. The quiz checks user selections, provides immediate feedback, tracks correct responses, and displays a final score after all four questions have been answered before restarting the question sequence.

**Responsive Web Interface** Uses CSS Flexbox, CSS Grid, flexible sizing, and `@media` queries to adapt the layout to different screen sizes. Navigation links, planet information cards, quiz options, and animation controls adjust to available screen space. On smaller screens, the orbital display and orbit paths are reduced to help the visualization fit mobile devices. Smooth scrolling and interactive hover effects provide additional navigation and interface feedback.

**Self-Contained Web Architecture** Combines HTML structure, CSS styling, and JavaScript functionality in a single `solarsystem.html` file. The project does not require a backend server, database, external JavaScript framework, or third-party library to run its core features. This structure makes the website straightforward to share, host through static website services, and modify as new educational features are added.

Have fun exploring the Solar System and enjoy the learning experience!
