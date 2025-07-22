CSS Homework 01 - My Reflections
Here's my submission for the CSS Challenge Mode homework. It was a great project that put some important concepts into practice. I've put all three exercises into the same HTML and CSS files, as requested.
What I Learned and How I Approached It
Exercise 1: Building the Profile Cards
This first part was a fun warm-up and a good way to get back into some of the trickier selectors.
Selectors: I tried to use a good mix of selectors here. I used a child selector (.team > .profile-card) to target the cards directly, and a descendant selector (.social-links a) for the icons. The attribute selector, a[href^="mailto"], was pretty cool for singling out the email link and giving it a different color.
Making it Interactive: To make the page feel more alive, I added a :hover effect that lifts the cards up a bit. For the pseudo-element requirement, I added a "Leader" ribbon to the first card with ::before. Getting that ribbon rotated and positioned just right took a bit of trial and error with position: relative on the card itself. I also had to use overflow: hidden on the card to make sure the ribbon didn't poke out past the rounded corners.
Layout: I went with Flexbox for the .team section because it's just so good for creating neat, flexible grids. Using the gap property made spacing the cards out way easier than messing with individual margins.
Exercise 2: The Pricing Table
I found this exercise really interesting. It was a great practical example of how the CSS box model works.
The Box Model: The main challenge here was using content-box for the first plan and border-box for the other two. I had to remember that the total width of the content-box element would include its padding and border, while the border-box elements would keep everything inside their set width. Seeing them all line up correctly really made the concept click. I definitely prefer border-box—it just feels more straightforward.
Making a Plan Stand Out: I made the middle plan pop by making it slightly bigger with transform: scale(1.05) and giving it a blue border. The "Most Popular" badge was done with ::before and absolute positioning, which worked just like the ribbon in the first exercise. The key was remembering to set position: relative on the plan's container so the badge would be positioned correctly.
Bonus Tooltip: The CSS-only tooltip was a fun little puzzle. I made a <span> in the HTML that was hidden by default (visibility: hidden and opacity: 0). Then, just by using :hover on the parent container, I could make it fade in. It's awesome what you can do without any JavaScript.
Exercise 3: The Hero Section
This last part was all about positioning and responsive design for a component you see on almost every website.
Layout with Flexbox: I used Flexbox again to get the main content perfectly centered in the hero section. It handles both horizontal and vertical alignment so easily.
The Background Image: The instructions had the <img> tag after the text content, so I took that as a chance to make a cool, full-width background image. I set the main .hero container to position: relative and then absolutely positioned the image to fill it. The magic trick was z-index: -1, which pushed the image behind all the text and buttons. I also darkened the image a bit with a filter so the white text was easy to read.
Sticky Nav: position: sticky is one of my favorite CSS properties. It's so simple to make the navigation bar scroll down with the page and then "stick" to the top of the screen.
Making it Responsive: The site needed to work on mobile, so I added a media query for smaller screens (max-width: 768px). This just stacked the profile cards and pricing plans vertically. I also made the navigation links stack into a column so they were easier to use on a phone.
Overall, this was a fantastic set of exercises. It was challenging in all the right ways and did a great job covering some of the most useful concepts in modern CSS.
