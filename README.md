# Overview of Project
In this project, we are helping Dana White about in-depth analysis of UFO sightings. She is creating a dynamic table and webpages that users will be using to filter for multiple criteria, publish her work online. In addition to the date, we will add table filters for the city, state, country, and shape.

## Resources
javascript, HTML, Bootstrap, Visual Code, Browser Edge
data for table from data.js, index.html

## Results
1- We first remove the list (<li></li>) element that creates the button in the index.html file.
2- We created four more list elements: city, state, country, and shape using this script(example of ):
<li class ="bg-dark">
   <label for = "city">Enter City</label>
   <input type="text" placeholder="benton" id="city" />
</li>
3- Next we created an empty filters variable in the app.py file. This allow us to keep track of all the elements that change when a search is entered. Then, we wrote the code with two functions: updateFilters() and filterTable().
The updateFilters() function update the filters variable we created.
The filterTable() function filter the table data by the value that is entered for the "id" that has changed.
4- We created a variable that saves the element that was changed using: d3.select(this).
5- We also created a variable that saves the value of the changed elements property 
usilet elementValue = changedElement.property("value");
                       console.log(elementValue);
6- Next, we created a variable that saves the attribute of the changed elements id.
7- Using the if-else statement, we checked if a value was changed by the user. If a value was changed, it will add the elements id as the property and the value that was changed to the filters variable. If a value was not entered, then clear the element id from the filters variable.
8- We called the filterTable() function inside updateFilters() function 
9- We wrote the code to filter the table based on the user input.
10- We also created a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.
11- Using the For loop, we look through the filters object and store the data that matches the filter values in the variable.
12- We finally rebuild the table with the filtered data by passing the variable. 

## Summary
### UFO drawbacks
We have limited data available with data from countries like US and Canada only.
The UFO sightings are pretty old and from the year 2010, that too from first 13 days only.
There is no clear button to clear the search.
The search is done by one at a time. 

### Recommendation
We could have added a chart also for better presentation.
instead of type in the values, we could have added a drop down and select from the list.
