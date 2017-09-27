# Course: ISTA-322
## Lesson Plan: 05
### Name: Tyler Reed
#### Date: 26 September 2017

1. What elements does an HTML form contain?

	-Input elements like buttons, checkboxes, text inputs...
1. What attributes does the HTML form element take?

	-An action attribute that tells the browser where to send the information and a method attribute that tells the browser how to send the information.
1. What does HTTP GET do? When is it used?

	-Takes the input names and values inside the form and puts them in the query string./Often
1. What does HTTP POST do? When is it used?

	-The browser places input inside the body of the HTTP request./You should not use this if possible.
1. How does an ASP.NET action method know what the query parameters are? How does it know what the parameter values are?

	-When you use a HTTP POST./Automatically
1. How does the dynamic calculation of the route path work in the HTML helper BeginForm?

	-It asks the routing engine how to reach the Search action of the HomeController. 
1. What is HTML encoding? How does it work? Why is it necessary?

	-Converts your code into HTML./Helps you to avoid cross-site scripting attacks (XSS).
1. What is URL encoding? How does it work? Why is it necessary?

	-Process that replaces reserved characters in the URL with other charactera like (%)./Prevents users from injecting malicious code.
1. What is JavaScript encoding? How does it work? Why is it necessary?

	-JavaScript encoding encodes the JavaScript on the page to prevent malicious attacks.
1. (Not in book) What is the JavaScript library jQuery? What does it contain, and why do we use it?

	-A cross-platform JavaScript library designed to simplify the client-side scripting of HTML./Designed to make it easier to navigate a document, select DOM elements, create animations, handle events, and develop Ajax applications.
1. (Not in book) What is the JavaScript library jQueryUI ? What does it contain, and why do we use it?

	-A curated set of user interface interactions, effects, widgets, and themes built on top of the jQuery JavaScript Library./jQuery UI is built for designers and developers alike.
1. (Not in book) What is the JavaScript library AngularJS ? What does it contain, and why do we use it?

	-A JavaScript framework designed for creating one-page web applications. Since it is a framework, it uses code templates and specific commands to perform special features such as filters and data-binding within HTML pages.