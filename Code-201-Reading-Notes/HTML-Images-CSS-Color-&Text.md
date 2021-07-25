# HTML Images

## Adding Images

```
<img>- to add an image to the page, you will need to use
an <img> element. This is an empty tag, which means
there is no closing tag
<br />

src- another component of the image element is src,
which tells the browser where to get the image file.
<br />

alt- this is where you can provide a text description
of the image which describes the image if you can not
see it
<br />

* title- you can also use the title attribute to the 
<img> element if you want to provide additional information
about the image. Most browsers will display this text
when the user hovers over the image
```
Below, you can see example of the syntax that is used to
add an image to a page in HTML:

```
<img src="your-image-url-here.jpg" alt="A text description of your image goes here" title="Your image title goes here"/>
```

Definitions in this section were derived from Chapter 5: “Images” (pp.94-125)
of the textbook *HTML & CSS Design And Build Websites* By Jon Duckett


# CSS Color

There are four ways to specify color in CSS:

1. **RGB Values:** These express color in terms of how much red,
green, and blue are used to make it up. For example- rgb(100,100,90)

2. **Hex Codes:** These are six-digit codes that represent the amount
of red, green, and blue in a color preceded by a hash sign. 
For example- #ee3e80

3. **Color Names:** There are 147 predefined color names that are
recognized by browsers. For example- DarkCyan

4. **RGBA Values:** CSS3 introduced the RGBA property which allows
you to specify a color the same way you would with an RGB value, but
adds a fourth value to indicate opacity. The RGBA value will only 
affect the element on which it is applied. (Not the child elements.)


Definitions in this section were derived from Chapter 11: “Color” (pp.246-263)
of the textbook *HTML & CSS Design And Build Websites* By Jon Duckett

# CSS Text 

## Typeface Terminology

- **Serif:** These fonts have extra details on the ends of the main strokes
of the letters. These details are known as serifs.

- **Sans-Serif:** These fonts have straight ends to letters

- **Monospace"** Every letter in monospace (or fixed-width) fonts are the 
same width. (Non-monospace fonts have different widths)

- **Weight:** Font weight adds emphasis and affects the amount of white space
and contrast on a page

- **Style:** Italic fonts have a cursive style to some of the lettering. Oblique
font styles take the normal style and put it on an angle.

- **Stretch:** In condensed (or narrow) versions of the font, letters are thinner
and closer together. In expanded versions they are thicker and further apart.

## Specifying Typeface

The **font-family** property allows you to specify the typeface that should be used 
for any text inside the element(s) to which a CSS rule applies. The Value of this property is the typeface you want to use.

## Size Of Typeface

The **font-size** property lets you choose a size for the font. There are several ways you
can specify the size of a font. The most common are:

* **Pixels: Pixels** are the most common way to specify font-size because they allow
web designers very precise control over how much space their text takes up. The number
of pixels is followed by px. For example- font-size: 12px;

* **Percentages:** The default size of text in browsers is 16px. So a size of 75% would equal
12px and a size of 200% would equal 32px. 

* **EMS:** Allow you to change the size of text relative to the size of the text in the parent element. 

## Font Formats

Because different browsers support different formats for font, you will need to provide the font in several different variations to reach all browsers. The various font formats should appear in your code in this order:

1. eot
2. woff
3. ttf/otf
4. svg




Definitions in this section were derived from Chapter 12: “Text” (pp.264-299)
of the textbook *HTML & CSS Design And Build Websites* By Jon Duckett

