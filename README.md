# Overview of Project
In this project, we are helping Dana White about in-depth analysis of UFO sightings. She is creating a dynamic table and webpages that users will be using to filter for multiple criteria, publish her work online. In addition to the date, we will add table filters for the city, state, country, and shape.
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
1- There is no button search history.
2- The search is limited to the a few days from 1st to the 13th.
3- The countries filter is limited to US and Canada. 
### Recommendation
- Add a dropdown to choose date, city, state and shape from.
- Create a link for each event that will give you more details on a different page.
