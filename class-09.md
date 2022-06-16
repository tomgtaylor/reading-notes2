# Class 09 - Forms and Events

## Web Forms

These web forms allow an interaction between a uswer and a web site/application, often to let users enter data, which is then sent to a web server.

Web form HTML includes form controls (widgets), and elements that structure its form (HTML forms). These can look like any of the following:

    dropdown boxes, checkboxes, buttons, radio butons, etc.
    These use the <input> tag to use. 

We will use these HTML tags to create forms:

    <form>, <label>, <input>, <textarea>, and <button>


All forms start with a < form > element, like this:

    <form action="/my-handling-form-page" method="post">
    </form>

    Action attribute: defines URL location where form's data should be sent.

    Method attribute: defines which HTTP method to send data with (usually get or post).

Next, we look at the data entry, which use the < label > tag.

**Input field for name** is single line text field.<br>
**Input field the email** is an input of type email. Single line text field that only accepts email addresses. <br>
**Input field for the message is a < textarea >, multiline text field.

    <form action="/my-handling-form-page" method="post">
    <ul>
     <li>
       <label for="name">Name:</label>
        <input type="text" id="name" name="user_name">
      </li>
      <li>
        <label for="mail">E-mail:</label>
       <input type="email" id="mail" name="user_email">
      </li>
      <li>
        <label for="msg">Message:</label>
        <textarea id="msg" name="user_message"></textarea>
      </li>
     </ul>
    </form>
    Example below:

< li > tag used to structure our code.
Attribute "type" is important because it defines how < input > appears/behaves.

---

Last but not least, note the syntax of < input > vs. < textarea > < /textarea >. This is one of the oddities of HTML. The < input > tag is an empty element, meaning that it doesn't need a closing tag. < textarea > is not an empty element, meaning it should be closed with the proper ending tag.

    <input type="text" value="by default this element is filled with this text">

    On the other hand, if you want to define a default value for a <textarea>, you put it between the opening and closing tags of the <textarea> element, like this:

 The < fieldset> and < legend> elements
The < fieldset> element is a convenient way to create groups of widgets that share the same purpose, for styling and semantic purposes. You can label a < fieldset> by including a < legend> element just below the opening < fieldset> tag. The text content of the < legend> formally describes the purpose of the < fieldset> it is included inside.

Here is a little example:

Here is a little example:

    <form>
      <fieldset>
        <legend>Fruit juice size</legend>
        <p>
          <input type="radio" name="size" id="size_1" value="small">
          <label for="size_1">Small</label>
        </p>
        <p>
          <input type="radio" name="size" id="size_2" value="medium">
          <label for="size_2">Medium</label>
        </p>
        <p>
          <input type="radio" name="size" id="size_3" value="large">
          <label for="size_3">Large</label>
        </p>
      </fieldset>
    </form>


<form>
  <fieldset>
    <legend>Fruit juice size</legend>
    <p>
      <input type="radio" name="size" id="size_1" value="small">
      <label for="size_1">Small</label>
    </p>
    <p>
      <input type="radio" name="size" id="size_2" value="medium">
      <label for="size_2">Medium</label>
    </p>
    <p>
      <input type="radio" name="size" id="size_3" value="large">
      <label for="size_3">Large</label>
    </p>
  </fieldset>
</form>


[Mozilla Link to Email Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)

---

## Intro to Events

---

An event refers to an action that happens in the system when the system fires (or produces) a signal.

Examples of this include

- Selecting, clicking, or hovering the mouse cursor over an element.
- User chooses a key on keyboard.
- Web page finishes loading.
- Form is submitted.
- Error happens.

---

Example of event:

    < button>Change color< /button>
    
    The JavaScript looks like so:

          const btn = document.querySelector('button');

          function random(number) {
            return Math.floor(Math.random() * (number+1));
          }

          btn.addEventListener('click', () => {
            const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
            document.body.style.backgroundColor = rndCol;
          });

We also define a function that returns a random number.

The third part of the code is where we define and register the event handler. The < button> element has an event called 'click' that fires when the user clicks the button. Objects that can fire events have an addEventListener() method, that takes at least two arguments: the name of the event and a function to handle the event. So we call the button's addEventListener() method, passing in:

Other Events:

- focus and blur - color changes when button is focused and unfocused.
- dblclick - color changes when button is double-clicked.
- mouseover/mouseout - the color changes when mouse pointer hovers over button.

## Things I want to know more about

- More about how to use Dom properly.
- Practical usage of objects for web pages / apps.

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-08)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-10) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
