# Lab 05: Using JavaScript Functions

To begin, first open the *lab-05-data/index.html* file within the Working Files in Brackets. Then open the file in your web browser using the Live Preview (and as usual open your web developer toolbar/Console as well). You'll see the script currently prompts you to enter the area of Lexington (~285.5 square miles), and then does nothing.

The goal of this task is to finish writing a map script that:

1. prompts the user to enter two additional areal units for two additional cities
2. stores this information within an array data structure, along with other hard-coded values of cities' names, populations, and geographic coordinates 
3. . uses a looping structure to populate the map with markers while building a popup that displays the name of the city and its population density

We'll be encapsulating our code within **3 functions** to achieve this.

Save changes to your *index.html* file and **commit changes to your local GitHub repository** as you work. Begin your coding beneath line 84 containing the JavaScript comment `begin writing/editing Lab 05 code here`. The instructions below will guide you through this process. Note that, beyond the instructions below, the comments within the script also inform you of where and what you should be coding.

1. Note that there is already one variable that is assigned the result of a [JavaScript prompt function](https://developer.mozilla.org/en-US/docs/Web/API/Window/prompt). This prompt function is an old-school way of collecting user information in a web page. The code also converts (or "casts") the string type entered by the user into a numeric type using the [Number function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number). You should create a second and third variable to reference the area of a second and third city entered by the user (i.e., copy this statement and paste/modify two more times). (**.5pt**)

2. Next, you'll notice the script calls a function named `prepareData` and passes the `lexArea` variable as an argument. Modify this statement to additionally pass, as 3 separate arguments, all 3 variables referencing the city areas. (**.5pt**)

3. Modify the `prepareData` function's definition so that it accepts the two additional  of the appropriate parameters (i.e., the three variables referencing the cities' areas) within the function's parentheses. (**.5pt**)

4. Finish populating the 4 arrays within the `prepareData` function's body with information from your 2nd and 3rd cities. The final array, referenced by the `cityAreas` variable, **should hold variable names and not hard-coded values like the other arrays**. (**.5pt**)

5. At the bottom of the `prepareData` function's body, modify the statement calling the function named `mapCities` to pass all four Arrays as arguments. (**.5pt**)

6. Complete the `mapCities` function to accept the 4 Arrays as parameters. These parameter names should match those used within this function's body. (**.5pt**)

7. Uncomment and then complete the statement assigning a value to the variable `density`. This statement should call a function named `calcPopDensity` and pass 3 arguments: 1) the city's population, 2) the city's area, and 3) the `units` variable, which has been initially defined as *'miles'*. Note that you'll be continuing to modify the script so this value can be changed to 'km'. (**2pt**)

8. Now write a new function named `calcPopDensity` (outside of the `mapCities` function's body). This function needs to accept 3 values as parameters: a city's population, its area, and the variable `units` designated within the `mapCities` function (i.e., 'miles' or 'units'). (**3 pts**)Write code within the function's body to first:

    a. determine whether the units are in miles or kilometers and, using conditional logical, then
    
    b. calculate population density using the population and area values before returning the result to the caller (i.e., this value will be assigned to the `density` variable within the `mapCities` function). Your conditional (if/else) statements will need to mathematically convert the miles to kilometers if the value of `units` is changed to be 'km'.
    
9. Finally, uncomment the rest of the popup to now include the calculated value of the population density.

10. Change the `h1` and `h2` tags to update your web document with title and subtitle, and edit the text at the bottom of the page (e.g., author and meta information) 

Be sure that your code is clean and uniformly indented (the Lab 05 Starter Template exemplifies such clean code) (**1pt**).

Additionally, include the *lesson-05-data/index.html* file with the examples demonstrated within the lesson saved in the file (**1pt**).

**Additional challenge:** Note how if the user enters information incorrectly, either a alpha/string value for the area, or a value of something other than 'miles' or 'km' for the unit, the script essentially breaks and the page must be reloaded. How would you go about catching these errors and again prompt the user to enter the correct information? Hint: consider using a looping mechanism. Also read about the JavaScript [try ... catch statement](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/try...catch).

Sync your final solutions with your remote repository and provide a link within Canvas by the due date: **Friday, February 19th, 11:59pm**.
