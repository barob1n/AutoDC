# AutoDC
Create one-time use [DC.js](https://dc-js.github.io/dc.js/) charts from csv files.

## Try the [Demo](https://dstreet26/AutoDC)

## Some pictures

**Initial page load. Pick an example data set or upload your own. Then click the "Load Data" or "Use this example" buttons.**

![Initial page load](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Initial%20page%20load.png "Initial page load")

![Example Datasets](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Example%20Datasets.png "Example Datasets")

**Use the table to choose which type of dc.js chart to create for each column detected in the csv file. Row charts work for most data types, Bar charts require numerical data, and Time charts require Dates. Click the "Go" button to create the actual charts.**

 ![Config Table](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Config%20Table.png "Config Table")

**To follow along, just select them all for charting by checking all the "Chart it?" buttons.**

 ![Selecting all](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Selecting%20all.png "Selecting all")

**Here, 10 charts were created that are all Row charts. However, some of this data would be better suited for a numerical bar chart, so go back to the table and select "Number" and "Bar" for 8 of the columns.**

![Generated charts 1](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Generated%20charts%201.png "Generated charts 1")

![Changing chart types](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Changing%20chart%20types.png "Changing chart types")

**Click the "Go!" button again to see the new charts**

![Generated charts 2](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Generated%20charts%202.png "Generated charts 2")

**Let's filter for fast cars (low 0-60s time) and from that selection, lets pick the least economical ones (low mpg)**

![Filtering fast cars](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Filtering%20fast%20cars.png "Filtering fast cars")

![Filtering economic cars](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Filtering%20economic%20cars.png "Filtering economic cars")

**While filtering, the other charts update in instantly**

**Below the charts is a counter showing on how many data points match the cross-filter criteria out of the total number of data points. Here you can download a copy of the filtered data.**

**Finally, the table at the bottom shows the filtered data in table-format. It also groups the data by what was selected from the creation table.**

![Filtered Datatable](https://github.com/Weatherproof/AutoDC/raw/master/doc/images/Filtered%20Datatable.png "Filtered Datatable")


## Run it yourself

1. Get [npm](https://nodejs.org/en/)
2. Install bower `npm install -g bower` (might need admin privileges)
3. Get a static file-server like [http-server](https://github.com/indexzero/http-server), [Apache](https://www.apache.org/), [nginx](https://www.nginx.com/resources/wiki/), [Caddy](https://caddyserver.com/), or use Python's built-in [SimpleHTTPServer](https://docs.python.org/2/library/simplehttpserver.html)
4. Get the code, install dependencies, and serve the directory (this is using http-server)

```shell
git clone https://github.com/Weatherproof/AutoDC
cd AutoDC
npm install
bower install 
http-server .
```

## Example Data Sets
The example data sets were plucked from [PivotTable.js](http://nicolas.kruchten.com/pivottable/examples/) and [Raw.js](http://raw.densitydesign.org/)

## Future Features

- An "advanced" view for creating a chart that has more grouping options, allows the user to pick the x-axis and y-axis dimensions, etc.
- More chart types. DC.js has documentation for donut/pie, line, bubble, scatter, heatmap, choropleth, and boxplot.
