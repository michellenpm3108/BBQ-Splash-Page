**** some hints to build this ***

1/ background image: 
 - create a fallback in case the background image loading is too slow and doesn't appear (SOLUTION: background-color)
 - let the image covers whole background (SOLUTION: background-size)
 - choose the center part of the photo to be shown (SOLUTION: background-position) 
 - blend the background image with the blackground-color to let the wordings on it more appealing (SOLUTION: background-blend-mode)

2/ text's order: write the text in a logic order, change its order if the design requires (SOLUTION: set display flex for the parent element and set new order for the child element)

3/ break point for media queries: find the break point based on layout, not on devices sizes (how long is the line, leave it inviting to read)

4/ fit all information of the intro part within the viewport's height (on big screen), no need to scroll down when screen is shrunk to narrow 
SOLUTION:
- min-height: 100vh
- * { box-sizing: border-box; } (width/height of ANY element = the border+ padding+content)

5/ vertically center the main content (SOLUTION: flex box, justify-content)

6/ separate the content in the intro part:
- top word sucks to the top, bottom words suck to the bottom (justify-content: space-between)
- prevent words sticking together (min-height: 50vh, set margin for the center word -h1 )

7/ prevent the words getting too long in big screen  (SOLUTION: max-width: 400px) 

8/ FORM:
- scale the button to become a bit bigger in hover and focus status (SOLUTION: transform: scale(1.2) )
- make the transition smoother (SOLUTION: transition: .5s)
- button has gradient (SOLUTION: background-image: linear-gradient(to left, red, blue))

9/ decorate the border top of the text top: make it gradient (SOLUTION: border-image, border-image-slice)