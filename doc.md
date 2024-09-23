### Method 1: Using CSS with a class toggle

You can use CSS to define the animation, and then apply the class via JavaScript when the user interacts with the page.

#### HTML:
```html
<svg id="mySvg" width="100" height="100" viewBox="0 0 100 100">
  <rect id="rect" x="10" y="10" width="80" height="80" fill="blue"/>
</svg>

<button id="animateBtn">Animate</button>
```

#### CSS:
```css
@keyframes rotate-scale {
  0% {
    transform: rotate(0deg) scale(1);
  }
  100% {
    transform: rotate(360deg) scale(1.5);
  }
}

.animated {
  animation: rotate-scale 2s ease-in-out forwards;
}
```

#### JavaScript:
```javascript
document.getElementById('animateBtn').addEventListener('click', function() {
  document.getElementById('rect').classList.toggle('animated');
});
```

### Method 2: Using JavaScript with inline `transform` property

If you need more control over the animation or want to change the transform dynamically based on user input, you can directly manipulate the `transform` property of the SVG element using JavaScript.

#### HTML:
```html
<svg id="mySvg" width="100" height="100" viewBox="0 0 100 100">
  <rect id="rect" x="10" y="10" width="80" height="80" fill="blue"/>
</svg>

<button id="animateBtn">Animate</button>
```

#### JavaScript:
```javascript
document.getElementById('animateBtn').addEventListener('click',

It seems I got cut off! Here's the continuation of the JavaScript example:

#### JavaScript:
```javascript
document.getElementById('animateBtn').addEventListener('click', function() {
  const rect = document.getElementById('rect');
  rect.style.transition = 'transform 2s ease-in-out';
  rect.style.transform = 'rotate(360deg) scale(1.5)';
});
```

### Summary of Steps:

1. **HTML**: Create an SVG and a button.
2. **CSS Animation**: Define a `@keyframes` rule for transformations (e.g., rotate, scale).
3. **JavaScript**: Add an event listener to the button that triggers either adding a CSS class (with the animation defined) or directly manipulating the SVG's `transform` property via inline styles.

Let me know if you need more details!
