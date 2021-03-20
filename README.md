# UFO Sightings with JavaScript
<img src="static/images/readme_header.png" width="1100" height="300">

## Project Overview
My best friend, Dana, is a journalist who is at a point in her career where she has the freedom to choose the topic she wants to write about. Since she's been a UFO enthusiast for as long as she can remember, she's decided to write about UFO sightings. For this assignment, she has a JavaScript file filled to the brim with sighting information. Since I'm a JavaScript whiz and know how to utilize its visual functionality, Dana has enlisted my help. I plan to use JavaScript to display Dana's sightings file as a table. However, since there is so much data, sifting through it without any adjustments would be a challenge. Thankfully, JavaScript provides a way to manipulate the data by adding filters. It's a little tricky to add more than one filter but I'm up to the challenge. Additionally, Dana and I will be working together to put everything online in a tidy HTML page - her article, the table of data, and easy-to-use filters to fine tune the results. Dana and I are looking forward to seeing the website come to life!

## Resources
- **Data Sources**: `data.js` file
- **Software and Tools**: JavaScript, HTML/CSS, Bootstrap, VS Code & Git Bash

## Challenge Deliverable and Results
The advanced website looks like this:

<img src="static/images/Delv 1_UFO Sightings website.PNG">

- There are now five list elements for filtering in the `index.html` file: date, city, state, country, and shape.

	<img src="static/images/Delv 1_list elements.PNG">

- I added an event listener to detect changes to each filter element in the `app.js` file. When a web visitor enters their input into any of these filter elements, the website detects the change and calls the `updateFilters()` function.

	<img src="static/images/Delv 1_event listener.PNG">

- The `updateFilters()` function saves the element, value, and the id of the filter that was changed based on the web visitor's input and calls the `filterTable()` function. 

	<img src="static/images/Delv 1_updateFilters().PNG">

- The `filterTable()` function loops through all of the filters, keeps any data that matches the filter values, and rebuilds the displayed table. 

	<img src="static/images/Delv 1_filterTable().PNG">

- Below are website screenshots of examples that demonstrate what happens to the table results when you input filter criteria. 
  - for a date of 1/7/2010: 
  
  	<img src="static/images/Delv 1_web filter_date.PNG">
  
  - for a date of 1/8/2010 and state of Texas (tx):
  
  	<img src="static/images/Delv 1_web filter_date and state.PNG"> 

## Challenge Summary
I think Dana and I have a lot to be proud about with how this website turned out! However, the dataset it relies on is very limited. Since it only emcompasses sightings for the first two weeks of January 2010, a major drawback to this new design is it doesn't take much filtering to yield no results.

Two recommendations for further development are:

1. Adding a tailored message when no results are found for various search criteria.
2. A current limitation of the search filters is they are case sensitve. Therefore, a key feature for further development would be to allow capitalized text, especially for the city and state fields.
