# charts in javascript ( visually analyze the results)
We have 3 charts :
1. line charts
2. pie Charts
3. bar charts 


We can create charts using predefined library called **Chart.js**

to setting up :
1. create html element called ``<canvas>`` , it has no contents just attrbutes 
``<canvas id="" width="" height="" style=""></canvas>``
this is the syntax for html canvas element  in the body tag

2. call chart.js predefined library in html in this way 
``<script sec='chart.min.js'></script>`` in the head 
i used this one
 ``  <script src="https://cdn.jsdelivr.net/npm/chart.js@2.9.4/dist/Chart.min.js"></script>``

script CDN for big data  // call chart.min.js


At first sight a ``<canvas>`` looks like the ``<img>`` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the ``<canvas>`` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

Note: If your renderings seem distorted, try specifying your width and height attributes explicitly in the ``<canvas>`` attributes, and not using CSS.



