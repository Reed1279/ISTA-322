# Course: ISTA-322
## Lesson Plan: 02
### Name: Tyler Reed
#### Date: 18 September 2017

1. What is a controller? What does it do?

	-A C# Class that allows you to invoke it from the Web.  Mediates between the module and the view
1. Explain the relationship between URLs and controller methods.

	-They both depend on the ASP.NET routing system to decides how URLs map to controllers and actions. They have a direct 1-1 corospondance.
1. What does it mean to say that, The web is stateless?"

	-Treats each request as an independent transaction
1. Where in the directory structure of an ASP.NET MVC application do controllers live?

	-In the Controllers folder/System.Web.Mvc.Controller, 
1. What programming constructs do controllers contain?

	-The methods
1. Where are action methods? What do they do?

	-In the controller class/Return an instance of a class that derives from ActionResult.
1. What are query parameters?

	-Placeholders for a value when a query runs
1. How do action methods receive HTTP query parameters?

	-They are retrieved from the request's data collection and located on the HTTP header.