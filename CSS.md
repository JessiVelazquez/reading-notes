# What is CSS?

CSS pairs with HTML to stylize each HTML element.

## CSS works with "rules"

- Each rule has a selector and a declaration.

- A selector says which HTML element the rule applies to.

- A declaration indicates what the element looks like.

- Examples are things like font sieze, font, color, background, etc.

- Declarations have two parts: a property and a value. A property indicates what property of the element are changing, and value indicates what you are changing it to. Example: font would be a property and size 12 would be a value.

## Separate Document

- Often it is best to place your CSS code in a seperate document, and then use the HTML element *link* to link to it.

- CSS can be inside an HTML file, but for SOC reasons, better to keep it separate.

# Color

## Specifying Colors

- You can specify using RBG, hex code color, or color name (page 249)

- For foreground color, use property (color:)

- For background color, use property (background-color:)

```
h1 {
    color: rgb(100,100,90);)
}
```

## Color Terminology

- RGB is red, green, and blue values. like this (100,100,88)

- Hex Codes are RGD in hexadecomal code. RGB(102, 205, 170) renders to #66cdaa.

- Color names - there are 147 color names spported by browsers. Hard to remember though, and limiting, so not commonly used.

#### HSL Colors

- In CSS3, we have HSL. This indicates hue (on a color wheel in dgrees out of 360), saturation (1-100), and lightness (0-100) - page 255



## Contrast

- Important to contrast foreground and background.

- High contrast is good for headers, they pop. But big text blocks can be hard to read with high contrast.

- Use medium contrast for long text blocks.

- CSS3 has an opacity property, called RGBA where "a" is alpha value for opacity. Also can be used with HSL as HSLA. (page 254)
