#Chart.js

[Chart.js](http://www.chartjs.org/) is a charting Javascript library. It is based on HTML5 *<canvas>* element.

![alt-tag](https://raw.githubusercontent.com/basilesimon/datajournalists-toolbox/master/chart.js/chartjs.png)

##Typical use case

Chart.js is a lightweight solution for those times when you need a quick and simple graph.
It is heavily customisable, and embeds models for line charts, bar charts, radar charts, pie charts, polar area charts, and doughnut charts.

The data has to be passed as an array, containing labels, numeric values, and a couple of elements required for styling.

Note: as Chart.js uses canvas, the charts created with it will NOT be interactive. If interactivity is a requirement, you might as well look for SVG libraries, such as d3.js.

##Examples online

##Gist

Data structure for a line chart:
```
  var data = {
    labels : ["January","February","March","April","May","June","July"],
    datasets : [
      {
        fillColor : "rgba(220,220,220,0.5)",
        strokeColor : "rgba(220,220,220,1)",
        pointColor : "rgba(220,220,220,1)",
        pointStrokeColor : "#fff",
        data : [65,59,90,81,56,55,40]
      },
      {
        fillColor : "rgba(151,187,205,0.5)",
        strokeColor : "rgba(151,187,205,1)",
        pointColor : "rgba(151,187,205,1)",
        pointStrokeColor : "#fff",
        data : [28,48,40,19,96,27,100]
      }
    ]
  }
```

Data structure for a doughnut chart:
```
  var data = [
    {
      value: 30,
      color:"#F7464A"
    },
    {
      value : 50,
      color : "#E2EAE9"
    },
    {
      value : 100,
      color : "#D4CCC5"
    },
    {
      value : 40,
      color : "#949FB1"
    },
    {
      value : 120,
      color : "#4D5360"
    }
  
  ]
```
##Installation and use

* Chart.js is available on [CDNJS.com](http://cdnjs.com/libraries/chart.js)
* Alternatively, you can download [the source](https://raw.githubusercontent.com/nnnick/Chart.js/master/Chart.js) (or its [minified version](https://raw.githubusercontent.com/nnnick/Chart.js/master/Chart.min.js) ) and include it in your HTML *<head>*

##Docs

* [Comprehensive documentation with code templates](http://www.chartjs.org/docs/)
* As Chart.js is not under development anymore, irs [Issues tracker on Github](https://github.com/nnnick/Chart.js/issues) will direct you to numerous forks with added functionalities.

