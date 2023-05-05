Download Link: https://assignmentchef.com/product/solved-cse270e-assignment10-extend-the-weather-temperature-application
<br>



In this assignment you will extend the weather/temperature application from Chapter 3 so that it also has a second page that displays the daily summary.




<ul>

 <li>Copy over the temperature application from the book to your nodejs working copy. Call this directory AssigmentModule10. Note: This working copy should NOT be in put /var/www/html since we do not want the apache server to be able to “serve” it. This working copy should be in your /home/ubuntu directory.</li>

 <li>In index.ejs add an “id” field to the form. The code in the book uses the tag $(form) to access the form. This is somewhat bad practice since this will add the on submit handler to all forms. We want to modify this so it has a specific form it references. In index.ejs add the id “indexform”, &lt;form id=”indexForm”…  Now in the public/the.js file modify the code so it uses this new name. Change $(form) to $(“#indexForm”)….</li>

 <li>Go ahead and test that it still works.</li>

 <li>Now add a second page. Copy over index.ejs to summary.ejs and

  <ol>

   <li>modify summary.ejs’s form id to be “summaryForm”</li>

   <li>Add links to index.ejs and summary.ejs to each other. Add these links just before the closing body tag.</li>

  </ol></li>

 <li>Modify app.js so it has a handler for /summary that calls summary.ejs</li>

 <li>Extend the existing app.js ajax code so that it returns a field called daily.summary to the JSON.</li>

 <li>In the code the.js copy over the submit handler and make a new submit handler for summaryForm. In this form replace code that displays the temperature with code that will display the daily summary.</li>

 <li>Make sure to add comment blocks to all your code with your name, date, class and assignment.</li>

 <li>Run this server on port 3010</li>

</ul>

10)Submit a clickable link to

<ol>

 <li>your git repo.</li>

 <li>your running instance</li>

</ol>