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

[Mozilla Link to Email Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)

---

< li > tag used to structure our code.
Attribute "type" is important because it defines how < input > appears/behaves.

## Intro to Events

---

## Things I want to know more about

- More about how to use Dom properly.
- Practical usage of objects for web pages / apps.

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-08)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-10) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
