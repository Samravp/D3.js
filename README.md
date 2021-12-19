# D3.js

In this project, I am analysing the current trends that are shaping people's lives to publish on a newspaper. 

Outcome of the analysis are visualised by creating charts, graphs, and interactive elements to help readers understand the findings.

The data set included with the project is based on 2014 ACS 1-year estimates: https://factfinder.census.gov/faces/nav/jsf/pages/searchresults.xhtml .

Please see the final visualisation [here](https://samravp.github.io/D3.js-Dashboard-Design/).


<img width="717" alt="Screen Shot 2021-12-19 at 14 49 34" src="https://user-images.githubusercontent.com/85004202/146663259-b97d8c7a-26db-4130-9a79-33737fb7b4eb.png">



## Analysis

Using the D3 techniques, I created a scatter plot that represents each state with circle elements.
I did code this graphic in the app.js file and pulled in the data from data.csv by using the d3.csv function. 

The scatter plot includes click events so that the users can decide which data to display. 
The transitions of the circles' locations are animated as well as the range of axes. 

I binding all of the CSV data to the circles, which enabled hme to easily determine their x or y values when clicking the labels.

While the ticks on the axes allow users to infer approximate values for each circle, it's impossible to determine the true value without adding another layer of data. 

I added tooltips to the circles and displayed each tooltip with the data that the user has selected, I used the d3-tip.js plugin developed by Justin Palmer.

I used [David Gotz's example](http://bl.ocks.org/davegotz/bd54b56723c154d25eedde6504d30ad7) to understand how I should implement tooltips with d3-tip.
