#Datamaps.js

[Datamaps](http://datamaps.github.io/) is an excellent Javascript library which leverages D3.js' power to create customizable and beginners-friendly SVG maps for the web. 

![datamaps](https://raw.githubusercontent.com/basilesimon/datajournalists-toolbox/master/datamaps.js/datamaps.png)

##Typical use case

You don't feel confident enough to go *full d3 mode* for this quick map you need to throw in your article. 

Then fill in the constructor with options from [DataMaps Docs](https://github.com/markmarkoh/datamaps/blob/master/README.md#getting-started) and set up your first d3 map!

##Examples online

* [Datamaps examples page](http://datamaps.github.io/)
* [How-to and same-sex marriage in the world example](http://blog.basilesimon.fr/2014/04/24/draw-simple-maps-with-no-effort-with-d3-js-and-datamaps-js/)
* [Bay area economic institute](http://europeconnections.bayeconfor.org/#home)

##Gist

```javascript
  // Getting the container's dimensions
  var width = document.getElementById('container').offsetWidth;
  var height = document.getElementById('container').offsetHeight;
  // Datamap constructor, fill in the options from the docs
  var map = new Datamap({
    element: document.getElementById('container'),
      fills: {
          YES: '#666666',
          UNKNOWN: 'rgb(0,0,0)',       // These are
          defaultFill: '#CDCCCC'       // the colours
      },
           data: {                     //Place data here
          ARG: {fillKey: 'YES'},
          BEL: {fillKey: 'YES'},
          BRA: {fillKey: 'YES'},
          CAN: {fillKey: 'YES'},
          DNK: {fillKey: 'YES'},
          FRA: {fillKey: 'YES'},
          ISL: {fillKey: 'YES'},
          MEX: {fillKey: 'YES'},
          NLD: {fillKey: 'YES'},
          ZAF: {fillKey: 'YES'},
          ESP: {fillKey: 'YES'},
          SWE: {fillKey: 'YES'},
          GBR: {fillKey: 'YES'},
          URY: {fillKey: 'YES'},
          USA: {fillKey: 'YES'},
          NOR: {fillKey: 'YES'},
      },
    setProjection: function(element, options) {
      var projection, path;
      projection = d3.geo.mercator()                          // The d3 projection
                     .translate([(width/2), (height/2)])      // And some options
                     .scale( width / 2 / Math.PI)
                     .center([-15.652173913043478, 17.2734596919573]);
      path = d3.geo.path()
               .projection( projection );
      return {path: path, projection: projection};
    }
  });
```

##Installation and docs

* [All versions: world, USA, and minified](https://github.com/markmarkoh/datamaps/tree/master/dist)
* [Getting started](https://github.com/markmarkoh/datamaps/blob/master/README.md#getting-started)
* [Guides](datamaps.markmarkoh.com)
