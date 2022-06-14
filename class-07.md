# Class 07 - HTML Tables, OOP, and JS Constructor Functions

## Domain Modeling

Domain modeling = creates a model in code to address a specific problem.

According to Code Fellows, Domain Modelling:

> "describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.<br><br>A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams."

---<br>
Example of domain modeling below:

![Domain Model image]( domainmodel.png)

---

## HTML Tables

A table consists of both rows and columns. Table tags include:


    Table tags include:

    <table> table tag
    <td>    table data
    <tr>    table row
    <th>    table header
    <col>   column tag
    <colgroup> tag nests <col> tags within

    
    1. First of all, make a local copy of blank-template.html and minimal-table.css in a new directory on your local machine.
    2. The content of every table is enclosed by these two tags : <table></table>. Add these inside the body of your HTML.
    3. The smallest container inside a table is a table cell, which is created by a <td> element ('td' stands for 'table data'). Add the following inside your table tags:

    <td> Hi, I'm your first cell.</td>

[https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics#when_should_you_not_use_html_tables] (Link to Mozilla about this)

---

Javascript objects

### Defining a constructor + intitialize properties 
<br>

**Remember: objects are key/value pairs** 

<br>

While object literals are used for creating one object, constructors are used to creating multiple objects. While objects literals require all objects to be changed individually, constructors enable you to change properties for all objects. Example of a constructor below:

     1. Make function called "createPerson(name)". 
     2. Add two members: a property name and method "introduceSelf().
     See below example:


      function createPerson(name) {
        const obj = {};
        obj.name = name;
        obj.introduceSelf = function() {
        console.log(`Hi! I'm ${this.name}.`);
        }
        return obj;
      }
 "createPerson()" takes a parameter "name" to set the value of the name property, but the value of the introduceSelf() method will be the same for all objects created using this function. Then one can create many objects by reusing this. 

        const salva = createPerson('Salva');
        salva.name;
        salva.introduceSelf();

        const frankie = createPerson('Frankie');
        frankie.name;
        frankie.introduceSelf();

Constructors, by convention, start with a capital letter and are named for the type of object they create.

     function Person(name) {
     this.name = name;
     this.introduceSelf = function() {
     console.log(`Hi! I'm ${this.name}.`);
      }
    }

To call Person() as a constructor, we use new:

    const salva = new Person('Salva');
    salva.name;
    salva.introduceSelf();

    const frankie = new Person('Frankie');
    frankie.name;
    frankie.introduceSelf();

---

## Things I want to know more about

- How to use objects correctly
- How to use constructors efficiently

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-06)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-08) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
