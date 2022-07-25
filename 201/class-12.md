# Chart.js, Canvas

## JavaScript Canvas

<canvas> element that allows you to draw 2D graphics using JavaScript.

requires height and width to specify canvas size 

chnage width and height using DOM

canvas requires opening and closing tag

Use the HTML5 canvas element for drawing 2D graphics.

Use the getContext('2d') to get the 2D drawing context for drawing 2D graphics on canvas.

Use the fillStyle and StrokeStyle properties to set the styles for the 2D drawing context.
(references: https://www.javascripttutorial.net/web-apis/javascript-canvas/)

## Questions

1. What does the <canvas> allow a developer to acheive?

allows to draw 2D graphics using js

2. What is the importance of the closing `</canvas> tag?

allows any code inbetween opening and closing canvas tag to be rendered if browser unsupports the canvas element 

3. Explain what the getContext() method does.

returns the rednderd context object, in this case the 2D drawing made by canvas 

## Chart.js Documentation

(references: https://www.chartjs.org/docs/latest/ )

## Questions

1. What is Chart.js and how it can be brought into your project?

a generator for creating canvas graphs, using a js file thats manipulatable; for yesterday lab I can create the graph the client is asking for  

2. List 3 different Chart types you can create using Chart.js.

area chart, bar chart, bubble chart

## Easily Create Stunning Animated Charts with Chart.js

chart.js - a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy

Drawing a line chart: 

<canvas id="buyers" width="600" height="400"></canvas>

<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>

var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}

How a graph look in HTML:

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <!-- import plugin script -->
        <script src='Chart.min.js'></script>
    </head>
    <body>
        <!-- line chart canvas element -->
        <canvas id="buyers" width="600" height="400"></canvas>
        <!-- pie chart canvas element -->
        <canvas id="countries" width="600" height="400"></canvas>
        <!-- bar chart canvas element -->
        <canvas id="income" width="600" height="400"></canvas>
        <script>
            // line chart data
            var buyerData = {
                labels : ["January","February","March","April","May","June"],
                datasets : [
                {
                    fillColor : "rgba(172,194,132,0.4)",
                    strokeColor : "#ACC26D",
                    pointColor : "#fff",
                    pointStrokeColor : "#9DB86D",
                    data : [203,156,99,251,305,247]
                }
            ]
            }
            // get line chart canvas
            var buyers = document.getElementById('buyers').getContext('2d');
            // draw line chart
            new Chart(buyers).Line(buyerData);
            // pie chart data
            var pieData = [
                {
                    value: 20,
                    color:"#878BB6"
                },
                {
                    value : 40,
                    color : "#4ACAB4"
                },
                {
                    value : 10,
                    color : "#FF8153"
                },
                {
                    value : 30,
                    color : "#FFEA88"
                }
            ];
            // pie chart options
            var pieOptions = {
                 segmentShowStroke : false,
                 animateScale : true
            }
            // get pie chart canvas
            var countries= document.getElementById("countries").getContext("2d");
            // draw pie chart
            new Chart(countries).Pie(pieData, pieOptions);
            // bar chart data
            var barData = {
                labels : ["January","February","March","April","May","June"],
                datasets : [
                    {
                        fillColor : "#48A497",
                        strokeColor : "#48A4D1",
                        data : [456,479,324,569,702,600]
                    },
                    {
                        fillColor : "rgba(73,188,170,0.4)",
                        strokeColor : "rgba(72,174,209,0.4)",
                        data : [364,504,605,400,345,320]
                    }
                ]
            }
            // get bar chart canvas
            var income = document.getElementById("income").getContext("2d");
            // draw bar chart
            new Chart(income).Bar(barData);
        </script>
    </body>
</html>

(references: https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

## Questions

1. What are some advantages to displaying data via a chart over a table?

although more difficult to set up, data displayed by charts is more visually apealing for a user and easier to understand than a table 

2. How could Chart.js aid your previously created applications visually?

its like reset.CSS, it gives perametres for desired 2D rendered graph 

## Things I want to know more about 
- understand principles of canavs, however can't visualize how to actually draw 2D rendered object 
- why is making a grpah harder than a table using JS