# Class 13 - Local Storage

Local storage and how to use it.

As a developer, one needs to store their state of interface. Normally, this is done server-side.

Cookies: a text file hosted on user's computer, and connected to the domain the website runs on.

Cookies have limitations:

- they add to the load of every document accessed on the domain.
- only allow 4 kb of data storage

Using local storage is pretty easy. Just have to modify the "localStorage" object in javascript. One modifies this by using the "setItem()" and "getItem()" method:

    localStorage.setItem('favoriteflavor','vanilla');
    
If you read out the favoriteflavor key, you will get back “vanilla”:

    var taste = localStorage.getItem('favoriteflavor');
    // -> "vanilla"

To remove the item, you can use — can you guess? — the removeItem() method:

    localStorage.removeItem('favoriteflavor');
    var taste = localStorage.getItem('favoriteflavor');
    // -> null

One annoying shortcoming of local storage is that you can only store strings in the different keys.

You can work around this by using the native JSON.stringify() and JSON.parse() methods:

    var car = {};
    car.wheels = 4;
    car.doors = 2;
    car.sound = 'vroom';
    car.name = 'Lightning McQueen';
    console.log( car );
    localStorage.setItem( 'car', JSON.stringify(car) );
    console.log( JSON.parse( localStorage.getItem( 'car' ) ) );

[View more info at this link](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

---

## Things I want to know more about

- More about how to use this effectively.


[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-12)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-14a) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
