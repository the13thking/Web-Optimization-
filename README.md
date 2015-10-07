P4
Website Performance Optimization

Steps to run the application:
-Open pizza.html in a Google Chrome browser

-Open Developer Tools (Ctrl + Shift + I), and go to Timeline

-Press the record button, and scroll from top to bottom and back to the top multiple times before pressing the record button again to stop recording.

-Wait for the recorded events timeline, and check to see if all colored bars are under the 6OFPS line.

-The application works as required(frame rate is 60FPS or better)

-Open index.html in the browser to view the page, and click on the links present to view other project pages

-To check the PageSpeed score, go to - https://developers.google.com/speed/pagespeed/insights/ and enter the page URL

-The application works as required if the score for both mobile and desktop versions is over 90 percent

Changes made to optimize the pizza page (main.js):
In main.js:

-In the updatePositions function, stored the value of document.body.scrollTop/1250 outside the for loop so it doesn't have to be recalculated with every iteration

-Reduced the number of pizzas from 200 to 120 in the final function that generates sliding pizzas.

-used getElementByClassName(faster) instead of querySelectorAll  


To optimize resizePizzas in main.js:

-got rid of DetermineDX and DX as well as other useless variables 

-got rid of px and just using % to make things faster

General:
-resized pizzeria with http://www.picresize.com/

-compressed all images using https://tinypng.com/

-Optimized CSS delivery by using internal stylesheets 

-took out Google webfont because it wasn’t making a huge difference

-Used the media attribute (print and portrait) in the css links where applicable

-Loaded JS files asynchronously where possible by using the async attribute

"I hereby confirm that this submission is my work and that I am abiding by guidelines within the Student Code of Conduct in the Nanodegree student handbook."