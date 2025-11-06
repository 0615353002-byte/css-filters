# css-animations

## Learning Target
- I am learning how to work with images in CSS

## Success Criteria
- I can use the ```filter:``` to apply filters to an image (```blur()```, ```grayscale()```, etc.)
- I can set images as the background for an element using ```background: url('image.jpg')'```
- I can create animations using filters



# Get started
1. Install Live Server and Go Live to view how the webpage looks with no styling
2. Follow directions below

# Filters
```css
selector {
    filter: blur(px) | grayscale(%) | sepia(%) | invert(%) | opacity(%);
}
```
See [W3Schools](https://www.w3schools.com/cssref/css3_pr_filter.php) for more filters and information

# Background Images
```css
selector {
  background-image: url("background.jpg");
  background-repeat: no-repeat | repeat;
  background-position: center | top | top left | top right | bottom | bottom left | bottom right;
  background-size: cover | auto | contain | width px height px;
  background-color: #f0f0f0; /* Fallback color if image fails to load */
}
```
## Gradients
```css
selector {
    background-image: linear-gradient(color1, color2, color3, ... ) | radial-gradient(color1, color2, ...);
}
```

# Practice Assignment
1. Make the elephant "disapper" when clicked (shrink and fade the opacity to 0)
2. Make the giraffe "dance" when clicked (maybe rotate back and forth while moving up and down a little)
3. Make the hippo "jump" when clicked (move a little down, then way up and back)
4. Do something creative with the tiger. See what you can come up with


# Animation Properties
## 1. Define animations with ```@keyframes```
Define values at specific percentages of the animation. You can specify any percentage values for steps in the animation.
```css
@keyframes animation-name {
    0% {
        /* starting properties */
    }
    25% {
        /* properties after 25% of time as elapsed */
    }
    50% {
        /* properties at 50% */
    }
    75% {
        /* properties at 75% */
    }
    100% {
        /* properties at 100% (the end) */
    }
}
```

## 2. Apply animation to a selector
```css
selector {
    animation: name duration timing-function;
}
```