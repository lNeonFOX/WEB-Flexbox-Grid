# Assignment #2. Advanced CSS (Flexbox & Grid)

**Name:** Torekhan Taimas
**Group:** IT-2503

## Part 1. Flexbox

### Task 0. Navigation Bar
Create a header with a logo on the left and a list of links on the right. Make the header a flex container, align the logo and links horizontally, add spacing between the links with Flexbox, and center everything vertically.

Implementation: `display: flex`, `justify-content: space-between` and `align-items: center` on the header. The list of links is a second flex container with `gap: 30px`.

<img width="1071" height="586" alt="изображение" src="https://github.com/user-attachments/assets/459c6fb0-1cfe-4e3e-a610-74124364a3e5" />


### Task 1. Card Row
Create a container with at least three cards (image, title, text, button). Show the cards in a row, make all cards the same height, add equal gaps, and add a hover effect.

Implementation: the container uses `display: flex`, `flex-wrap: wrap` and `gap`. Each card is `flex: 1 1 260px`. Equal height comes from the default `align-items: stretch`. Inside each card, `flex-direction: column` and `flex: 1` on the text keep the buttons at the bottom. The hover effect uses `transform: translateY(-8px)` and a larger shadow.

<img width="1067" height="1052" alt="изображение" src="https://github.com/user-attachments/assets/f80b0713-9f5c-42af-ade6-9bbcfff0c0ef" />


## Part 2. Grid System

### Task 2. Page Layout with Grid Areas
Create a layout with a header, sidebar, main content and footer. Use a grid container, define rows and columns, and assign grid areas so the header and footer span the full width, the sidebar is on the left and the main content is on the right.

Implementation: `grid-template-columns: 240px 1fr`, `grid-template-rows: 80px 1fr 60px` and `grid-template-areas` with the names header, sidebar, main and footer. Each element is placed with `grid-area`.

<img width="287" height="436" alt="изображение" src="https://github.com/user-attachments/assets/e37fd2e6-50ca-41da-8d87-163d33e6303b" />


### Task 3. Image Gallery
Place at least nine images in a gallery container. Use a grid with equal columns and rows, add gaps, and add a hover effect that shows a caption overlay.

Implementation: `grid-template-columns: repeat(3, 1fr)`, `grid-template-rows: repeat(3, 240px)` and `gap: 16px`. Images use `object-fit: cover`. Captions are absolutely positioned inside each `figure` and their opacity changes on hover.

<img width="1067" height="962" alt="изображение" src="https://github.com/user-attachments/assets/6a8a1c55-1075-473d-bd95-cb5149f7b267" />

### Task 4. Portfolio Page
Create a page with a header, main section, sidebar and footer. Use Flexbox for the header navigation, Grid for the main section (projects on the left, info on the right), Flexbox inside each project card, and make the footer span the bottom of the page.

Implementation: the header is a flex container. `.main-grid` uses `grid-template-columns: 2fr 1fr`. The projects area is a nested grid with `repeat(auto-fit, minmax(240px, 1fr))`. Each project card is a flex column with the title, description (`flex: 1`) and button. The body is a flex column with `min-height: 100vh`, so the footer stays at the bottom.

<img width="1063" height="963" alt="изображение" src="https://github.com/user-attachments/assets/f050fcaf-bd89-4e30-a2b7-4d3510f95b27" />


## Summary of the work process
I completed the assignment in five separate tasks, each in its own folder with its own HTML and CSS files. I first learned the basics of Flexbox and Grid from the W3Schools guides, then built the tasks in order, from the simple navigation bar to the combined portfolio page. I tested every page in the browser and in responsive mode, fixed alignment and spacing problems, and added media queries so the layouts work on smaller screens. Finally, I took screenshots of each task and uploaded the project to GitHub.
