# xspider
## A new and improved version with animations, jukebox, and extreme play
____
<br>
This is an improved version of Spider Solitaire which is an improved version of spider solitaire.  I wrote it this last year (starting i dont know when) and it was a smash success.  Main problems I encountered were:<br>
  1. Although the tableu information was stored in script, the engine read and processed the HTML.  This gave me primarily problems with my head.  The new goal is to have all of the engine and scripting happen in javascript and only push the display whats necessary, hoping that adding features will be easier and the game state will be much more condensed and more easily save-able as a cookie or txt file, bugs and error checks will be easier to see, and animations will be very easy to do.
  2. Stringify is nice but should not be relied upon for encoding.  Too many read errors.
  3. Cards will be fully rendered in SVG.  This means I can spin them, enlarge them, add fancier designs anytime, custom whatever.  SVG is surprisingly quick and universal.  Then you can burn my designs onto leather coasters and sell them at craft fairs for exorbident prices without asking my permission and stealing my art.
  4. I had a lot of redundancy that I should condense.  A lot of things happened in the background that would only show up at some point in the distant future.
  5. I know it is bad practice to put all the functions in one file however my goal is to make a single self contained file that can be executed in any browser environment.
<BR>
<BR>
Alpha coming maybe next decade.
