# Class 06 - JS Object Literals; The DOM

## Javascript - What are Object Literals?

Object Literal:

- Object Literal is a data structure similar to arrays.
- Like Arrays, they store values (strings, numbers, booleans, null, undefined)

An object includes a comma-separated list of name-value pairs inside of curly braces. Some ways to practice are using the following object values:

    person.name
    person.name[0]
    person.age
    person.bio()
    person.introduceSelf()

**Example of this below.** Let the below object refer to a person:

    let person = {
        name: ["Tom", "Veronica],
        age: [36, 41],
        bio: function {

            console.log(`${this.name[0]} ${this.name[0]} is ${this.age} years old.`);
        },
        introduceSelf: function() {
            console.log(`Hi, I'm ${this.name[0]}.`);
        }
    } ;

We can shorten bio: function () to simply bio(). See below.

    const person = {
        name: ['Tom', 'Veronica'],
        age: 32,
        bio() {
          console.log(`${this.name[0]} ${this.name[1]} is ${this.age} years old.`);
        },        //this is just a s
        introduceSelf() {
            console.log(`Hi! I'm ${this.name[0]}.`);
        }
    };

Each name/value pair must be separated with a comma, and the name and value in each case are separated by a colon. Example

    const objectName = {
      member1Name: member1Value,
      member2Name: member2Value,
      member3Name: member3Value
    };

## Dot Notation

- In short, the dot allows you to access the object's properties.

        person.age

        person = object
        .age = object's property

## Bracket Notation

Bracket notation is another way to access object properties.

Instead of:

    person.age
    person.name.first

You can use:

    person['age']
    person['age']['first']

---

## What is DOM?

    Document Object Model (DOM)
    
    DOM is NOT a programming language.
    DOM is an application programming interface (API) for HTML.

    It basically connects web pages to scripts or programming languages, like JS.

According to Mozilla on the DOM, they state that:

> "A web page is a document that can be either displayed in the browser window or as the HTML source. In both cases, it is the same document but the Document Object Model (DOM) representation allows it to be manipulated. As an object-oriented representation of the web page, it can be modified with a scripting language such as JavaScript."<br> <br> "All of the properties, methods, and events available for manipulating and creating web pages are organized into objects. "

The DOM uses multiple APIs (app programming interfaces) that work together.

### How to access DOM.

    You can access the DOM by using an API in Javascript within a "script," which is just a program run by a browser. You can used inline <script> tag to access DOM.

Fundamental Data Types (interface):

    Document        When one returns a document object, object is the root Document object.

    Node            Every object within a document is a node of some form.   

    Element         objects implement the DOM Element interface and the Node interface,

    NodeList        Array of elements.    

    Attr            Attributes are nodes in the DOM just like elements are.

    NamedNodeMap    like an array, but the items are accessed by name or index.

---

## Things I want to know more about

- More about how to use Dom properly.
- Practical usage of objects for web pages / apps.

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-05)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-07) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
