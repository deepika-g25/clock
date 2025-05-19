🕰️ Analog Clock – HTML, CSS, JavaScript

This is a functional Analog Clock built using HTML, CSS, and JavaScript, which dynamically updates the current time based on the system clock. The project visually represents the clock face with hour, minute, and second hands, rotating smoothly to reflect real-time changes.

✅ Features

Real-time updates based on system time
Smooth rotation of hour, minute, and second hands
Classic clock design with a clean, circular interface
Fully responsive layout using flexbox and absolute positioning

💡 Concept Used

This project replicates a traditional analog wall clock using web technologies:
A circular dial (styled with border-radius: 100%)
Number markers at 12, 3, 6, and 9 positions using absolute positioning
Three rotating hands representing hours, minutes, and seconds
Continuous real-time updates using JavaScript

🛠️ How It Works

HTML (index.html)

Defines the structure:
.clock div wraps all elements
.numbers div positions the static numbers (12, 3, 6, 9)
.arrows contains the hour, minute, and second hands

CSS (style.css)

Styles and positions elements:
Clock styled with a circular border and shadow
Numbers positioned using position: absolute and transform rules
Hands are styled rectangles with transform-origin: bottom center to rotate around the center
Animations are controlled with JavaScript via inline transform: rotate() updates

JavaScript (index.js)

Controls the logic:
Uses new Date() to fetch the current system time
Calculates rotation angles:

js

secondDegree = (seconds / 60) * 360;
minuteDegree = (minutes / 60) * 360;
hourDegree = (hours / 12) * 360;
Updates the .style.transform of each hand every second using setInterval()

📁 Project Structure
analog-clock/
├── index.html     # HTML structure of the clock
├── style.css      # Styling for layout and design
└── index.js       # Clock logic and time updates

🚀 How to Run

Download or clone this repository
Open index.html in your web browser
Watch the analog clock work in real-time!

🧠 Technologies Used

HTML5 – Layout and structure
CSS3 – Styling, positioning, and appearance
JavaScript (ES6) – Time logic and dynamic hand rotation
