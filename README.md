# P4-mobile
Project 4-Cameron Pittman: Portfolio Website Optimization
Goal
The PageSpeed score of 90 is for index.html (both mobile and laptop scores should be at least 90).
The frame rate of 60fps should be obtained for the pizza page (views/pizza.html). The file you need to study and change is views/js/main.js.
The original project is available at https://github.com/udacity/frontend-nanodegree-mobile-portfolio.
I have tried to optimize the files to try and meet the goals stated above.
Optimizations
Images
•	Reduced resolution for large files
•	Moved images locally
•	Created thumb nails
•	Compressed file size with Photoshop
JavaScript
•	Scripts not critical to build the DOM are loaded asynchronously
•	Moved non-critical scripts to bottom of html
CSS
•	CSS for print taken out of the critical rendering path
•	stylesheet minimized and loaded inline
•	removed unused id & class selectors rom bootstrap framework
Fonts
•	Fonts are loaded with @font-face vs link rel
Pizza page - FPS optimizations
•	Used the suggestion of a colleague refer to http://www.webreference.com/programming/javascript/jkm3/index.html  for help. As such the scroll-position is now stored in a variable outside of loop and no longer calculated for each pizza. (Idea adapted from http://www.webreference.com/programming/javascript/jkm3/index.html)
•	Local function variables used to improve performance. (Idea adapted from http://www.webreference.com/programming/javascript/jkm3/index.html)
•	Rewrote for loop for pizza sizes (calculations are now done outside of loop)
•	Removed unnecessary function requestAnimationFrame & unused variable currentScrollY
•	Reduced amount of pizzas by spacing them further apart
Resources Used
•	Help from colleague P. Stewart (mentioned above)
•	CSS Newbie
•	Webreference Javascript Optimization Tips
•	https://developers.google.com/speed/pagespeed/insights_extensions
•	https://developers.google.com/speed/docs/insights/rules
