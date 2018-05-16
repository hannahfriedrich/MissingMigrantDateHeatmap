# Missing Migrants Calendar Heatmap

**Calendar Heatmap** | **Last updated: May 2018** | **Applicable data types: CSV or JSON** | **Author: [Hannah Friedrich]**

![](img/cal.png)

This tutorial will walk through how to create a calendar heatmap of CSV data using D3. This calendar heatmap shows frequency of
reported migrant deaths or missing people that have been reported since 2014.

## 1\. Set up the workspace

## 2\. Data Sources
The data source used for this geovisualization is the [Missing Migrants] database. The database contains dates of events
that involved migrant deaths or injuries that have been reported.

## 3\. A function-by-function Tutorial
### CSS

    <style>

    body {
        font: 12px sans-serif;
        shape-rendering: crispEdges;
        width: 70%;
    }

    .day {
        fill: #fff;
        stroke: #ccc;
    }

    .month {
        fill: none;
        stroke: #000;
        stroke-width: 1px;
    }

    #info, text, p {
        font-family: 'Josefin Sans', sans-serif;
    }

    .container {
        color: grey;
        text-align: right;
        position: absolute;
        right: 20px;
        padding-top: 120px;
        padding-left: 80px;
        width: 20%;
        height: 20%;
    }

    #info {
        color: grey;
        text-align: right;
        position: absolute;
        right: 20px;
        padding-top: 80px;
        padding-left: 80px;
        width: 20%;
        height: 20%;
    }
    .title {
        text-align: right;
        position: absolute;
        right: 20px;
        padding-top: 10px;
        padding-left: 80px;
        width: 20%;
        height: 20%;
    }

    a{
        color: green;
    }

    h1{
        font-family: 'Josefin Sans', sans-serif;
    }

    .RdYlGn .q0-5{fill:rgb(220, 219, 219)}
    .RdYlGn .q1-5{fill:rgb(232, 203, 139)}
    .RdYlGn .q2-5{fill:rgb(243, 187, 59)}
    .RdYlGn .q3-5{fill:rgb(232, 128, 32)}
    .RdYlGn .q4-5{fill:rgb(220, 68, 4)}

    </style>

- html
- javascript
- css

## 4\. More examples of similiar geovisualizations
[Resuable Calendar Heatmap] allows the user to hover over individual cells which update the header information with
the cell value and date
[Heatmap with key] consists of a heatmap with a color key legend
[Vertical heatmap] is a similar construction of the heatmap with
[Alternative Calendar View] is a heatmap

## Acknowledgement
Thanks to Bo Zhao for helping me debug displaying the value in the mouse over function.

## References
This tutorial is based on the calander heatmap examples created by [Micah Stubbs] and [Mike Bostock], which were made
with Version 4 of D3.

[Hannah Friedrich]: https://github.com/hannahfriedrich/MissingMigrantDateHeatmap
[Missing Migrants]: http://missingmigrants.iom.int/
[Micah Stubbs]: https://gist.github.com/micahstubbs/89c6bd879d64aa511372064c6cf85711
[Mike Bostock]: https://bl.ocks.org/mbostock/4063318
[Resuable Calendar Heatmap]: http://bl.ocks.org/eesur/5fbda7f410d31da35e42
[Heatmap with key]: https://bl.ocks.org/alansmithy/6fd2625d3ba2b6c9ad48
[Vertical heatmap]: https://bl.ocks.org/danbjoseph/13d9365450c27ed3bf5a568721296dcc
[Alternative Calendar View]: http://bl.ocks.org/KathyZ/c2d4694c953419e0509b
