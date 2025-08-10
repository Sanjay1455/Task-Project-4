# Task-Project-4
Include with HTml and CSS
Project: Make a Website Mobile-Friendly Using CSS Media Queries
Objective:
Convert a desktop-only webpage into a mobile-friendly layout using CSS media queries.

**Tools Used:**

HTML5

CSS3 (Media Queries)

VS Code

Chrome DevTools for testing

**Steps Followed:**

Opened the HTML page in VS Code.

Identified fixed-width elements and large images causing layout issues.

Wrote media queries targeting screens with a max-width of 768px.

Adjusted layout for smaller devices by stacking columns vertically.

Reduced font sizes for better readability on mobile screens.

Made the navigation menu stack vertically on small viewports.

Tested responsiveness using Chrome DevTools device toolbar.

Fixed any overflow and scrolling issues.

Ensured all images scale within their containers.

**Features:**

Responsive navigation bar

Flexible content and sidebar layout

Mobile-friendly typography
Images scale automatically without distortion

**Interviwe Questions:**

**1. What are media queries?**
Media queries are CSS rules that apply styles only when certain conditions are met, such as screen width, height, resolution, or device type.
Example:

@media (max-width: 768px) {
  body { background: lightblue; }
}
This will change the background color when the screen width is 768px or less.

**2. Explain mobile-first vs desktop-first CSS design.**
Mobile-first: Start designing for smaller screens, then use min-width media queries to adjust for larger screens.

Desktop-first: Start designing for large screens, then use max-width media queries to adjust for smaller screens.

**3. How do you test responsiveness?**
Chrome DevTools (Device Toolbar mode)

Resizing browser window manually

Testing on actual devices (mobile, tablet, desktop)

Online tools like BrowserStack or Responsinator

**4. What units are best for responsive layouts?**
% (percentage) → flexible sizing

em / rem → scalable typography

vw / vh → viewport-based sizing

fr → CSS Grid fractional unit

**5. What is viewport meta tag?**
It tells the browser how to control page scaling and dimensions on mobile devices.
Example:

<meta name="viewport" content="width=device-width, initial-scale=1.0">
Without it, a mobile browser might zoom out to show the desktop version.

**6. How does flexbox help in responsive design?**
Flexbox allows elements to automatically adjust and wrap based on available space. You can easily change the direction, alignment, and spacing without fixed widths.

**7. Difference between absolute and relative units?**
Absolute units: Fixed size, not affected by parent/container (e.g., px, cm, in).

Relative units: Adjust based on context or viewport (e.g., %, em, rem, vw).

**8. How to handle images in responsive design?**
Use max-width: 100%; height: auto; so images shrink if needed.

Use srcset for different resolutions.

Optimize and compress images for faster loading.

**9. What is adaptive vs responsive design?**
Responsive: One flexible layout that adjusts fluidly to any screen size.

Adaptive: Several fixed layouts that switch at specific breakpoints.

**10. Explain CSS grid responsiveness.**
CSS Grid allows you to create layouts that adapt using fractional units (fr), minmax(), and auto-fit/auto-fill with repeat() for dynamic resizing.
Example:
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
}
This makes the grid automatically fit as many columns as possible.
