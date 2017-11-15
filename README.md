# nostreetsChartistScrollPlugIn.js
A Plugin For chartist.js that allow the user to across the x axis of the chart.

#### Example
```javascript

<script src="~/nostreetsChartistScrollPlugIn.js"></script>

<script type="text/javascript">

        var options = {
            lineSmooth: false,
            width: "1500px",
            axisX: {
                labelOffset: {
                    x: 0,
                    y: 0
                }
            },
            plugins: [
                chartistScroll( { 
                      height: "8px",
                      width: "15px", 
                      scrollbarColor: "red"
                 })
            ]
        };

        var renderedChart = new Chartist.Line('.ct-chart', {
            labels: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday'],
            series: [
                [12, 9, 7, 8, 5],
                [2, 1, 3.5, 7, 3],
                [1, 3, 4, 5, 6]
            ]
        }, options);

    </script>

```

