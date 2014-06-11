#DC.js

[http://dc-js.github.io/dc.js/](http://dc-js.github.io/dc.js/) is a Javascript library.
It uses d3.js and crossfilter.js to provide a multi-dimensional charting library.

![alt](https://raw.githubusercontent.com/basilesimon/datajournalists-toolbox/master/public/img/dcjs.png)

##Typical use case

Building a dashboard, as the one shown on their homepage.
The library combines d3.js to draw charts and the power of crossfilter.js to ensure the multi-dimensionality.

In practice, the charts interact with each other.
For example, selecting a period of time on a line chart will take this period of time as reference to redraw all the other charts for this period. Magically.

##Examples online

* [Public Accounts of Canada 2009-2012 by Ted Strauss](http://tedstrauss.github.io/expenditures/)
* [Stock Market Selection Strategy by Lon Riesberg](http://www.acrodatics.com)
* [Earthquake Data Discovery by d3noob](http://bl.ocks.org/d3noob/6077996)
* [Texas Death Row visualization by Joe Nudell](http://joenoodles.com/2013/7/texecutions)
* [Scoring the European Parliament by Xavier Dutoit](http://www.score-ep.org/)

##Gist

*in progress*

##Installation and use

DC.js is available [via CDN](https://github.com/dc-js/dc.js#cdn-location) for handy quick access.
There's also a *npm* package: 
`` npm install dc ``
And finally, you can work locally by getting all the resources separately. [Head here](https://github.com/dc-js/dc.js#install-without-npm) for a short list.

##Docs

* [API reference for stable version](https://github.com/dc-js/dc.js/blob/master/web/docs/api-1.6.0.md)
* [FAQ](https://github.com/dc-js/dc.js/wiki/FAQ)
* [Complete example thoroughly annontated](http://dc-js.github.io/dc.js/docs/stock.html)

