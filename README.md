Front-End Web Developer Nanodegree Project 4
============================================
Part 1 - Portfolio Main Page Optimization:

- index.html
 - Inlined style.css
 - Inlined referenced Google Font
 - Set print CSS stylesheet link to use media query
 - Moved non-critical JavaScript files to end of file and made async

- assets
 - Minified CSS
 - Minified JS
 - Compressed and reduced size of pizzeria thumbnail


Part 2 - Pizzeria Page Optimization:

- assets
 - Minified CSS
 - Compressed pizza.png
 - Compressed and resized pizzeria.jpg

- pizza.html
 - Added viewport meta tag

- main.js
 - global
  1 Moved nouns / adjective arrays to global scope to avoid recreating them every time a pizza was generated
  2 Moved sizeSwitcher function outside of changeSliderLabel function
  3 Removed determineDx function
  4 Moved randomPizza selector out of pizza append loop
 - changePizzaSizes
  1 Moved .randomPizzaContainer selector outside loop
  2 Added necessary determineDx functionality
  3 Resize uses percentages instead of pixels
 - updatePositions
  1 Moved scrollTop reference out of loop
  2 Moved phase calculation out of loop
  3 Translate X to move pizzas rather than changing left style
  4 Translate Z 0px to encourage browser to move pizzas to separate layer
 - DOMContentLoaded handler
  1 Changed pizza.png dimensions to reflect actual dimensions
  2 Removed basicLeft property and simply set left
  3 Moved #movingPizzas1 selector out of loop
  4 Rather than create 200 pizzas, calculate number required (8 per column, enough rows to fill screen)
