# Class 05 - HTML Images; CSS Color & Text

## HTML Media

### Common image file types include the following:

    APNG   Animated Portable Network Graphics   image/apng  .apng
    AVIF   AV1 Image Fir Format                 image/avif  .avif
    GIF    Graphics Interchange Format          image/gif   .gif
    JPEG   Joint Photo Expert Group image       image/jpeg  .jpg / .jpeg
    PNG    Portable Network Graphics            image/png   .png
    SVG    Scalable Vector Graphics          image/svg+xml  .svg
    WebP   Web Picture format                   image/webp  .webp

---

## CSS

### Applying Color to HTML elements

    color               defines foreground color of HTML elements
    background-color    defines the element's background color

### Text (CSS color properties): 

    color
    background-color
    text-shadow
    text-decoration-color
    text-emphasis-color
    caret-color

### Boxes (CSS color properties)

    border
    background-color
    column-rule-color
    outline-color

### Borders (CSS color properties)

    border-color
    border-left-color    border-right-color 
    border-top-color     border-bottom-color

    border-block-start-color    border-block-end-color

    border-inline-start-color   border-inline-end-color

### CSS Styling

    html {
      font-size: 10px;
    }

    h1 {
      font-size: 5rem;
    }

    p {
      font-size: 1.5rem;
      color: red;
      font-family: Helvetica, Arial, sans-serif;
    }

### Font style, font weight, text transform, text decoration:

    font-style      (normal / italic / oblique)

    font-weight     (normal / bold / lighter / bolder)

    text-transofrm  (uppercase / lowercase / captialize / full-width)

    text-decoration (underline / overline / line-through)

Example:

     html {
      font-size: 10px;
    }

    h1 {
      font-size: 5rem;
      text-transform: capitalize;
    }

    h1 + p {
      font-weight: bold;
    }

    p {
      font-size: 1.5rem;
      color: red;
      font-family: Helvetica, Arial, sans-serif;
    }

---

### Useful for letter, word, and text alignment

    text-align  (left / right / center / justify)
    line-height
    letter-spacing
    word-spacing

---

Other

Font styles:

    font-variant: Switch between small caps and normal font alternatives.
    font-kerning: Switch font kerning options on and off.
    font-feature-settings: Switch various OpenType font features on and off.
    font-variant-alternates: Control the use of alternate glyphs for a given font-face.
    font-variant-caps: Control the use of alternate capital glyphs.
    font-variant-east-asian: Control the usage of alternate glyphs for East Asian scripts, like Japanese and Chinese.
    font-variant-ligatures: Control which ligatures and contextual forms are used in text.
    font-variant-numeric: Control the usage of alternate glyphs for numbers, fractions, and ordinal markers.
    font-variant-position: Control the usage of alternate glyphs of smaller sizes positioned as superscript or subscript.
    font-size-adjust: Adjust the visual size of the font independently of its actual font size.
    font-stretch: Switch between possible alternative stretched versions of a given font.
    text-underline-position: Specify the position of underlines set using the text-decoration-line property underline value.
    text-rendering: Try to perform some text rendering optimization.

---

Text layout styles

Text layout styles:

    text-indent: Specify how much horizontal space should be left before the beginning of the first line of the text content.
    text-overflow: Define how overflowed content that is not displayed is signaled to users.
    white-space: Define how whitespace and associated line breaks inside the element are handled.
    word-break: Specify whether to break lines within words.
    direction: Define the text direction. (This depends on the language and usually it's better to let HTML handle that part as it is tied to the text content.)
    hyphens: Switch on and off hyphenation for supported languages.
    line-break: Relax or strengthen line breaking for Asian languages.
    text-align-last: Define how the last line of a block or a line, right before a forced line break, is aligned.
    text-orientation: Define the orientation of the text in a line.
    overflow-wrap: Specify whether or not the browser may break lines within words in order to prevent overflow.
    writing-mode: Define whether lines of text are laid out horizontally or vertically and the direction in which subsequent lines flow.    

## Things I want to know more about

- More about what properties are commonly used in CSS for real web pages / apps.

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-04)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-06) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
