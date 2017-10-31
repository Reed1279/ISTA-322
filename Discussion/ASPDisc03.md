# Course: ISTA-322
## Lesson Plan: 03
### Name: Tyler Reed
#### Date: 24 October 2017

1. In a nutshell, what is Chapter 9 about? A one word answer \routing" is not a suficient answer.
Explain what routing is, what it does, and its role in ASP.NET MVC.

	-Mapping logical URLs to action methods on controllers. It matches incoming requests that would not otherwise match a fi le on the fi le system and it maps the requests to a controller action.
2. What is the difference (as described in the book) between traditional web applications and applications
built with MVC frameworks?

	-These frameworks generally take a different approach by mapping the URL to a method call on a class, rather than some physical fi le.
3. What two approaches to routing does ASP.NET take? Explain the difference between them.

	-It matches incoming requests that would not otherwise match a fi le on the fi le system and it maps the requests to a controller action. It constructs outgoing URLs that correspond to controller actions.
4. What are the two locations for the placement of attribute routes?

	-Attribute routes, traditional routes
5. Where is the RegisterRoutes method deffned? What is its type and parameters? What is its visibility
and scope?

	-Application_Start, RegisterRoutes method, MapMvcAttributeRoutes registration method
6. At its core, what is the job of a route?

	-To map a request to an action.
7. How do you code dynamic behavior into routes? Be specific.

	-Edit the config/routes.rb file to replace the catch-all route with a call on the DynamicRouter.load
8. What are route constraints? Be specific. Give an example of the usage of a constraint and include the
program code for the constraint.

	-Constraints allow you to apply a regular expression to a path segment to restrict whether the route will match the request. With attribute routing, constraints were specifi ed inline in the route template using a syntax such as {id:int}. traditional routing has a different approach. Instead of putting information like this inline, traditional routing uses a separate parameter. For example:
		routes.MapRoute("blog", "{year}/{month}/{day}",
			new { controller = "blog", action = "index" },
			new { year = @"\d{4}", month = @"\d{2}", day = @"\d{2}" });
9. What are route defaults? Be specific. Give an example of the usage of a constraint and include the
program code for the constraint.

	-Regular expression strings to perform matching on a request URL, but if you look carefully, you’ll notice that the constraints dictionary is of type RouteValueDictionary, which implements IDictionary<string, object>.
10. What are optional route patterns? Be specific. Give an example of the usage of a constraint and
include the program code for the constraint.

	-You can use either attribute routing, traditional routing, or both. To use attribute routing, you need to have the following line in your RegisterRoutes method (where traditional routes live).
11. Where is the central location for placement of traditional routes?

	-RouteValueDictionary
12. What purpose do lioteral values serve in specifying routes?

	-Saying they must have a match for each of the route parameter values when matching the request URL.
13. In traditional routing, how do you specify that a route parameter is optional. Be specific | include
the name of the variable or method.

	-Make the {id} parameter optional by changing it to {id?}
inline in the route template.
14. (Not in the book) Write a regular expression that would recognize all of these dates as a valid route
parameter: 2017/10/31, 17/10/31, 2017/OCT/31, 17/Oct/31, and 17/October/31.

	-mysite/Controller/Action?date=2017-10-31
15. How do you combine traditional routing and attribute routing?

	-Instead of putting this information inline as part of the route template, traditional routing puts it in a separate argument after the route template.
16. How do you dynamically generate a hyperlink from within a view using named routes?

	-@Html.RouteLink("to Test", new {controller="section", action="Index", id=123})
	 @Html.RouteLink("to Default", new {controller="Home", action="Index", id=123})
17. How would you create a web application more than two layers deep? Note that the controller/action
syntax only permits two layers of the application. Suppose you wanted four layers, such as (for example)
Catalog/Books/Technology/Microsoft/id?.

	-The Web Forms layer, comprising server controls, ViewState, and so on. The plumbing, which supplies the basic web stack, including modules, handlers, the HTTP stack, and so on
18. What is the difference between the way that traditional routing and attribute routing handle multiple
route parameters in a segment?

	-Both options work well, and both are fl exible enough to handle complex routing scenarios. Which option to choose is largely a matter of style and preference, but attribute routing is simpler and keeps your route URLs together with your controller code.