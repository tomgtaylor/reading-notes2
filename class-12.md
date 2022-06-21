# Class 12 - Docs for the HTML < canvas > Element & Chart.js

## Canvas

HTML5 Canvas element
HTML5 features the < canvas > element that allows you to draw 2D graphics using JavaScript.

The < canvas > element requires at least two attributes: width and height that specify the size of the canvas:

        <canvas width="500" height="300" id="canvas"></canvas>
Code language: HTML, XML (xml)
Like other elements, you can access the width and height properties of the < canvas > element via its DOM properties:

    const canvas = document.querySelector('#canvas');
    const width = canvas.width;// 500
    const height = canvas.height;// 300
    Code language: JavaScript (javascript)

And you can also change the width and height of the < canvas > element using the DOM methods:

    canvas.width = 600;
    canvas.height = 400;

Anitially, the canvas is blank. To draw something, you need to access the rendering context and use it to draw on the canvas.

The < canvas> element features the getContext() method that returns a render context object.

The getContext() takes one argument which is the type of context. For example, you use the "2d" to get a 2D rendering context object, which is an instance of the CanvasRenderingContext2D interface.

The 2D rendering context allows you to draw shapes, text, images, and other objects.

The following example shows how to select the canvas element using the querySelector() method and access the drawing context by calling its getContext() method:

    let canvas = document.querySelector('#canvas');
    let ctx = main.getContext('2d');

Fill and Stroke

- Fill fills in the shape with a specific style such as color, gradient, and image.
- Stroke adds colors to the edges of the shape.

The fillStyle and strokeStyle properties of the 2D drawing context will determine the fill and stroke styles.

You can set these properties to a string, a gradient object, or a pattern object. By default, they both set to a value of '#000000'.

The following illustrates how to set the fill and stroke styles for the 2D drawing context and draw a rectangle.

    (() => {
        const canvas = document.querySelector('#main');
        if (!canvas.getContext) {
            return;
        }

        // get the context
        let ctx = canvas.getContext('2d');

        // set fill and stroke styles
        ctx.fillStyle = '#F0DB4F';
        ctx.strokeStyle = 'red';

        // draw a rectangle with fill and stroke
        ctx.fillRect(50, 50, 150, 100);
        ctx.strokeRect(50, 50, 150, 100);

    })();

---

## Chart.js

Uses a < canvas > note to render the chart.

    <canvas id="myChart" width="400" height="400"></canvas>
    <script>
    const ctx = document.getElementById('myChart').getContext('2d');
    const myChart = new Chart(ctx, {
        type: 'bar',
        data: {
            labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
            datasets: [{
                label: '# of Votes',
                data: [12, 19, 3, 5, 2, 3],
                backgroundColor: [
                    'rgba(255, 99, 132, 0.2)',
                    'rgba(54, 162, 235, 0.2)',
                    'rgba(255, 206, 86, 0.2)',
                    'rgba(75, 192, 192, 0.2)',
                    'rgba(153, 102, 255, 0.2)',
                    'rgba(255, 159, 64, 0.2)'
                ],
                borderColor: [
                    'rgba(255, 99, 132, 1)',
                    'rgba(54, 162, 235, 1)',
                    'rgba(255, 206, 86, 1)',
                    'rgba(75, 192, 192, 1)',
                    'rgba(153, 102, 255, 1)',
                    'rgba(255, 159, 64, 1)'
                ],
                borderWidth: 1
            }]
        },
        options: {
            scales: {
                y: {
                    beginAtZero: true
                }
            }
        }
    });
    </script>

    Setting up
The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="utf-8" />
            <title>Chart.js demo</title>
            <script src='Chart.min.js'></script>
        </head>
        <body>
        </body>
    </html>
 

Drawing a line chart
To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:

    <canvas id="buyers" width="600" height="400"></canvas>
Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

    <script>
        var buyers = document.getElementById('buyers').getContext('2d');
        new Chart(buyers).Line(buyerData);
    </script>
    


---

## Things I want to know more about

- More about 
- Practical

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-11)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-13) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
