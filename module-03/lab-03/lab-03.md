# Lab 03: Adding Markers for City Locations with Population Data

**Instructions:** First, be sure you've copied over the contents of */map672-s16/module-03/lab-03/* into the root directory of your *map672-s16* Git repository. Modify the index.html within the *lab-03-data* directory to fulfill the requirements listed below. The goal of this lab is to create 3 markers on the map for 3 different Kentucky cities, and provide information about those cities on a clickable popup. 

The *lab-03/index.html* file contains a lot of code that you won't recognize yet. Here we're "black boxing" the Leaflet code that actually makes the map work, for now.

Edit and save your changes to your *index.html* file and **commit changes to your local GitHub repository** as you work. 

To begin editing the code, open the *module-03/* directory using Brackets, double-click on the *index.html* file, and view the rendered page within Chrome using Live Preview. Remember, it's easiest to just open the entire *module-03/* directory within Brackets and then open the individual files you want within Brackets' **Working Files**. 

Open your JavaScript Console within your web browser and note that there is an Uncaught ReferenceError. This script is looking for values referenced by variables that do not yet exist. You will need to write these variables and values. Modify the JavaScript within the section beginning the code comment "begin writing Lab 03 code here" and ending with "end writing Lab 03 code here."

To start, declare a variable named `city1Name` and assign it a string value of "Lexington", like so (**.5pt**):

```javascript
var city1Name = "Lexington";
```

Now continue writing JavaScript and complete the following:

1. Declare a variable named `city1Lat`, determine the latitude of this city (e.g., using a Google search) and assign this number value to it. Do the same for a variable named `city1Lon` (**.5pt**).
2. Declare a variable named `city1Pop`, short for the population of the city, which you should also determine using a web search, and assign this numeric value to the variable (**.5pt**).
3. Declare a variable named `city1Capital` and assign a Boolean variable of either true or false, depending on whether this city is in fact the capital of the commonwealth of Kentucky (**.5pt**).
4. Save your changes, refresh your browser, and verify a marker has been correctly placed on Lexington and the popup information is correct. Look for errors in the JavaScript Console and return to your code to fix these errors.
5. Repeat this process for two more cities, Frankfort and another of your choosing. Name the related variables `city2` (i.e., `city2Name`, etc) and `city3`. **Note that you'll need to uncomment the code toward the bottom of the script for each city** for the script to run correctly (**2pts**).
6. Declare a variable named `totalPop` and assign it the sum total of the three city's populations, using their variables and the plus operator. Output this total to the JavaScript Console, preceded by the text, "The total population of these cities is: " (**1pt**). 
7. Next, declare a variable named `averagePop` and assign it a value of the cities' population average using a division operator (i.e., do not simply do the math yourself and hard code this value into the script). The numeric value should be preceded by the text, "The average population of these cities is: " (**1pt**).
8. Declare a variable named `cities` and assign it an array literal containing the three city names in their order created. On the next line, log the last item within the array to the Console using bracket notation (**1pt**).
9. Finally, change the `h1` and `h2` tags to update your web document with an appropriate (even fun!) title and subtitle, and edit the text at the bottom of the page (e.g., author and meta information) (**1pt**).

Also, be sure that the *map672-s16/module-03/lesson-03-data/index.html* file is complete with the examples detailed in the *lesson-03.md* instructions and Synced up with your GitHub repo (**2pts**)

Sync your final solutions with your remote repository and provide a link to your repository within Canvas by the due date: **Friday, February 5th by 11:59pm**.

Your final solution should look like this (with a meaningful yet fun title and subtitle!):
![Animated GIF of Lab 03 Solution](lab-03-graphics/lab-03-solution.gif)
