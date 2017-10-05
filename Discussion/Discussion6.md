# Course: ISTA-322
## Lesson Plan: 06
### Name: Tyler Reed
#### Date: 04 October 2017

1. Why do we want to validate user input on the client? Why do we want to validate user input on the server?

	-So that we can give feedback to the user after input./ Because the server retireves input from multiple users, to we want to confirm specific user input.
1. In ASP.NET MVC, what data items are the focus of validation?

	-Model values.
1. Where do data annotations live in the .NET framework?

	-In the namespace
1. Can you stack multiple validation attributes with regard to actions? If so, how many can you stack?

	-Yes./ Unlimited.
1. Explain the syntax of [remote]. What does it do?

	-The Remote attribute enables you to perform client-side validation with a server callback.
1. What is a server callback?

	-A server callback is when you send a value to the server, and compare the value against the values in the database.
1. What is a model builder? When does it run?

	-The process that works when an action method is bing executed.
1. What is the model state? When is it created? How is it created? What does it contain?

	-Contains all the errors associated with each property./ If any errors exist in model state, ModelState.IsValid returns false.
1. What does the controller action method generally do if the model state is not valid?

	-Re-renders the same view that posted the model values. 
1. What are the two options for custom validation? Explain your answer.

	-Value and validationContext./ The IsValid method accepts two parameters, the first is an object named value and the second is a ValidationContext object named validationContext. Value refers to the actual value from the field that your custom validator is validating.