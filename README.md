# Color Markers


## Overview

This simple project from [freecodecamp](https://www.freecodecamp.org/) demonstrated the different ways to apply colours in CSS by creating simple colour markers.

## What I learnt

### Primary, Secondary and Tertiary Colours 

Red, Green and blue make up primary colours. Secondary colours are created by mixing 2 primary colours in equal meassures whilst tertiary colours are a combination of all 3 primary colours.

### Colour Theory

Colour is important when creating web pages. It can bring structure to a page by drawing a users attention to important content, convey emotion or visually separate areas of a page.

Colour wheels are useful for showing the relationship between colours. Similar colours will be near each other whilst different ones are further apart. 2 opposite colours are known as ***complimentary colours***

It is best practice to limit the number of different colours to 1 primary colour and 1-2 complimentary colours.

### How to apply colours

There are 4 basic methods to apply colour.

1. ***named colours*** A list of built in colours can be found at [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)
2. ***hex***. 1st two chars = red 2nd two chars = green 3rd two chars = blue
3. ***rgb***. Values are given in a range between 0-255
4. ***hsl***. hue = 0-360 saturation and lightness given as a %

### Opacity

Opacity is the measure of how transparent a colour is and can be set by either using the ```opacity``` property of setting the ***alpha value*** within hex | rgba | hsla.

Values provided to opacity and alpha are either 0-1.0 | 0%-100%

```#00FF00CC``` last 2 chars represent alpha value

```rgba(r, g, b, alpha)``` | ```hsla(h, s, l, alpha)```

### linear-gradient

Apply smooth transitions between colours.

linear-gradient is a css function that takes at least 3 arguments ***gradientDirection*** | colour-1 | colour-2 | colour-3 | colour-nnn.

***gradientDirection*** given in degrees ***(default = 180deg)***.

***colour*** can be any of the CSS colour methods.

```linear-gradient(90deg rgb(255, 0, 0) rgb(0, 255, 0))```

The position where one color ends and another one starts is called ***colour-stop**** these are given as either ***px*** | ***%***

```linear-gradient(180deg rgb(255, 0, 0) 75%)rgb(0, 255, 0))```

In the above example the red colour will start at 0 and tack up 75% of its parent element.

### box-shadow

Use box-shadow to add more depth the colours using the following arguments:

```offsetX``` ```offsetY``` ```blurRadius``` ```spreadRadius``` ```color```

offsetX and offsetY default is 0 if no value is given. Values are either ***positive*** X = move shadow ***right*** Y = move shadow ***down*** | ***negative*** X = move shadow ***left*** Y = move shadow ***up***

blurRadius and spreadRadius are optional.

Color can be given as any of the CSS colour methods.

>[!example]+ Syntax

```css
box-shadow: offsetX offsetY blurRadius spreadRadius color;
```