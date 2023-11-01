# FactorEarth Interview Technical Challenge
### Alexa VanSchaardenburg

## Prompt
The task is to create a responsive layout using HTML and CSS to display four boxes in a 2x2 grid on larger screens and have them stack in a single column when the screen size is reduced. Using the provided html file, complete this task. 

## Preview 
![FE-TechChallenge-Preview](https://github.com/AlexaVanSchaardenburg/tech_challenge_factorearth/assets/125763236/3293eef3-abb0-4580-b547-a2d230d19f05)

## Process
In order to complete this challenge, I took the following steps:

1. Created a repository using the given HTML file, with a new CSS file, and a README.
2. Created and styled a basic 2x2 grid and a page header in HTML and CSS.
3. Made the design responsive using a media query that looks at the screen width in pixels and adjusts accordingly.
4. Styled the page to include the FactorEarth logo and colors.
5. Created a README to document what I did and added inline comments explaining the decisions I made in the code.

## The 'Why' Behind My Decisions
Why media queries?
- I chose to use media queries primarily because they give me the most control over exactly what a page looks like at specific screen widths. Another way I could have accomplished this task is by using the flex-wrap property in CSS. This would have required setting a max width to the parent container with the class `class="boxes"`. In my opinion this gives me less direct control over how many columns and rows there are, so I chose to use the grid-template-columns CSS property which allows me to directly specify how many columns there are. 
  
Why I used ems rather than pxs?
- In my experience, ems are a better unit to work in when making a design responsive. When I first learned CSS I worked primarily in pixels, but as I learned to  make design responsive ems became a better unit because it is relative. This means it scales better to other screen sizes and is not as 'set in stone' as px.

## Making Sure the Application Works as Anticipated
I wanted to ensure the grid changed as expected across all screen sizes. In order to test this I manually changed the size of my window on my laptop, and used the Chrome Dev Tools. In the Chrome Dev Tools I used the responsive feature to test across a wide range of screen sizes, down to 100px in width. I also checked the design on all of the sample screen sizes in the Dev Tools. 

The reason I tested in so many ways is because in my experience the way an application scales can change based on what tool I am using. Sometimes an application will look good when I only size down my window or use the Responsive feature in the Dev Tools, but then when I switch to a phone screen sample in the Dev Tools it will break. By testing all of these edge cases I ensure that users get a good experience regardless of what type of device they are using. 

## Other thoughts on Creating a Responsive Design
When I am working in a more complex application with more information, it is easier to make a design responsive when I know what the designer would like the application to look like across different screen sizes. This helps me write more through JSX/HTML with the appropriate divs/sections that will allow me to move elements around with media queries when I make the page responsive. In my personal projects I typically start with a mobile version first and then make adjustments as the screen size goes up, I have found this to make responsive design smoother, especially when the application is designed to work primarily on a mobile device. 
