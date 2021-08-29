Module 11 - UFO Challenge
--Overview

Dana has requested we build a website where users can access information regarding UFO sightings. However, because there are so many sightings, it can be difficult for a user to find specific information for specific dates and locations. To solve this problem, we write code that will create a table dynamically based upon our dataset. We also allow our users to filter the table data for specific values using only JavaScript, HTML, CSS, and D3.js on our web pages. 


--Results

The site is built using a basic HTML web page (index.html) that was created to display the dynamic table of UFO sightings. Using the UFO dataset that was provided in the form of an array of JavaScript objects, code was written in app.js that appends a table to the web page and then adds new rows of data for each UFO sighting with data pertaining to the date/time, city, state, country, shape, and comment of the event. (image:https://github.com/Roland791/UFO_Sightings/blob/main/static/images/Table.PNG )

Along the left hand side of the page, a simple filter form was created that allows users to input values for each field. A function called filterTable() was created using JavaScript that listens for events and searches through the each column to find rows that match user input and displays these to the webpage. (image: https://github.com/Roland791/UFO_Sightings/blob/main/static/images/filters.PNG)

A function called resetTable() clears the body of the table, populates the dropdown menu with unique date values from the dataset and displays all data to the table as a starting point.(image: https://github.com/Roland791/UFO_Sightings/blob/main/static/images/Filtered_Results.PNG)

--Summary

While the site now has a way to manage the dataset more easily, there are some limitations to what it can currently do, and issues with user friendliness. For example, the search fields can currently allow any input and are case sensitive, which means users could enter any number of options (example: US, us, United States) that would return different results, or none at all. A solution to this would be to set the search fields as dropdown fields that only contain the possible results for each field.  Additionally, allowing users to search for multiple criteria for each field (such as "us" and "ca" in the country field) would also make the search more flexible. 