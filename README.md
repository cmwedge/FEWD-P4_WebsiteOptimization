Front-End Web Developer Nanodegree Project 4
============================================
##Part 1 - Portfolio Main Page Optimization:

###index.html
- Inlined style.css
- Inlined referenced Google Font
- Set print CSS stylesheet link to use media query
- Moved non-critical JavaScript files to end of file and made async

###assets
- Minified CSS
- Minified JS
- Compressed and reduced size of pizzeria thumbnail


##Part 2 - Pizzeria Page Optimization:

###assets
- Minified CSS
- Compressed pizza.png
- Compressed and resized pizzeria.jpg

###pizza.html
- Added viewport meta tag

###main.js
- global
 - Moved nouns / adjective arrays to global scope to avoid recreating them every time a pizza was generated
 - Moved sizeSwitcher function outside of changeSliderLabel function
 - Removed determineDx function
 - Moved randomPizza selector out of pizza append loop
- changePizzaSizes
 - Moved .randomPizzaContainer selector outside loop
 - Added necessary determineDx functionality
 - Resize uses percentages instead of pixels
- updatePositions
 - Moved scrollTop reference out of loop
 - Moved phase calculation out of loop
 - Translate X to move pizzas rather than changing left style
 - Translate Z 0px to encourage browser to move pizzas to separate layer
- DOMContentLoaded handler
 - Changed pizza.png dimensions to reflect actual dimensions
 - Removed basicLeft property and simply set left
 - Moved #movingPizzas1 selector out of loop
 - Rather than create 200 pizzas, calculate number required (8 per column, enough rows to fill screen)
