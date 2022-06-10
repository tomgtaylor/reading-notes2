# Class 04 - HTML Links, CSS Layout, JS Functions

## HTML - Creating Hyperlinks

The basic way of creating a hyperlink in HTML starts by using the < a > tag (anchor), and adding in the href (hypertext reference) attribute to link to the web address. See below

    <p>
    <a href="https://www.Google.com"> Name of the link </a>
    </p>

    Actual example of this Google hyperlink is seen below:

<p>
<a href="https://www.Google.com"> Example: Google Link here </a>
</p>

Another way to do this is using the attribute title.

    <a href="https://www.Mozilla.org" title="Best place to learn about code"> 
    </a>

**Using Images with hyperlinks:**

Within < a > tags, use an < img >

    <a href="https://Google.com"> 
    <img src="Google-image.png" alt-"Google logo that links to home page.">
    </a>

---

## CSS Layout

Normal flow: 
- This refers to the layout in which elements behave in the flow.
- Normal flow is meant to make a document readable.
- Elements are laid out using a "Box Model"

Example of a Basic document flow below.

---

    <h1>Basic document flow</h1>

    <p>I am a basic block level element. My adjacent block level elements sit on new lines below me.</p>

    <p>By default we span 100% of the width of our parent element, and we are as tall as our child content. Our total width and height is our content + padding + border width/height.</p>

    <p>We are separated by our margins. Because of margin collapsing, we are separated by the width of one of our margins, not both.</p>

    <p>Inline elements <span>like this one</span> and <span>this one</span> sit on the same line along with adjacent text nodes, if there is space on the same line. Overflowing inline elements will <span>wrap onto a new line if possible (like this one containing text)</span>, or just go on to a new line if not, much like this image will do: <img src="long.jpg"></p>

    body {
      width: 500px;
      margin: 0 auto;
    }

    p {
      background: rgba(255,84,104,0.3);
      border: 2px solid rgb(255,84,104);
      padding: 10px;
      margin: 10px;
    }

    span {
      background: white;
      border: 1px solid black;
    }

### CSS Positioning

Positioning enables one to override the normal flow of a document. There are varrious types of positioning that can be used on HTML Elements, such as:

- Static Positioning
    - default position. Puts elements in normal poistion in document flow.
- Relative Positioning
    - once the positioned element has taken its place in the normal flow, you can then modify its final position, including making it overlap other elements on the page.
- Absolute Positioning
    - sits on its own layer separate from the normal document flow.
- Fixed Positioning
    - fixes an element in place relative to the visible portion of the viewport.
- Sticky Positioning
    - hybrid between relative and fixed position. It allows a positioned element to act like it's relatively positioned until it's scrolled to a certain threshold, and then becomes fixed.

Examples:

    Static Positioning

        <p class="positioned"> ... </p>

        Now add the following rule to the bottom of your CSS:

        .positioned {
        position: static;
        background: yellow;
        }

    Relative Positioning

        position: relative;

    Absolute Positioning

        position: absolute;

    Fixed Positioning:

        h1 {
        position: fixed;
        top: 0;
        width: 500px;
        margin-top: 0;
        background: white;
        padding: 10px;
        }

    Sticky Positioning:

        .positioned {
        position: sticky;
        top: 30px;
        left: 30px;
        }

---

## JavaScript - Functions 

**Functions** are essentially reusable blocks of code. Here's what they look like: <br>

![image](functions.png) <br>

    Simple example of a function:

    function myFunction() {
        alert('hello');
    }

### Invoking Functions

Afer the function is declared and defined, we have to run it. Often called invoking, calling, or running the function.

    Invoking a function is done by including name of function followed by ()

    Example:
        function myFunction() {
        alert('hello');
        }

        myFunction();
            // calls the function once

Function Parameters

Parameters are values that need to be included inside function parentheses ().

    const myText = 'I am a string';
    const newString = myText.replace('string', 'sausage');

## Things I want to know more about

- Functions. I want to know more about practical usage.
- CSS positioning. This seems really useful to learn more about.

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-03)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-05) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
