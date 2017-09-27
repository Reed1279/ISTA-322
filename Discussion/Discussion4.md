# Course: ISTA-322
## Lesson Plan: 04
### Name: Tyler Reed
#### Date: 24 September 2017

1. What is scaffolding?

	-A template that automates code generation.
1. What is a navigational property? What is a foreign key property?

	-Used to navigate to the object using the dot operator./Allows the object to be referenced from multiple database tables.
1. What is a virtual property? Why does the book use virtual properties?

	-Give Entity Framework (EF) a hook into your plain C# classes and enable features such as an efficient change-tracking mechanism. The EF needs to know when a property value on a model changes, because it might need to issue a SQL UPDATE statement to reconcile those changes with the database.
1. Explain eagar loading. Explain lazy loading. What is the difference between the two?

	-An eager loading strategy attempts to load all data using a single query. With lazy loading, EF loads only the data for the primary object in the LINQ query, and leaves the other properties unpopulated. Lazy loading is convenient, but can be expensive.
1. What is meant by seeding a database? Explain.

	-Enables you to create initial data for an application.
1. What is meant by the happy path? What is meant by the sad path? Give examples of each that are not in the book.

	-Executed code in a valid state and you can save the object in the database./A path the action takes if the model is invalid./When someone enters a valid email address is happy and if they leave the required field blank or in-valid email address, then that is sad :(
1. In HTTP POST, what happens when action parameters are passed by the query request? What happens to the parameters and how are they expressed?

	-It will use a model binder to build the parameter./Will automatically convert and move values from the request into an object. 
1. What is implicit model binding? Explain.

	-Works when you have an action parameter./The aggressive search behavior of the model binder can have unintended consequences. Occasionally there is a property you don't want (or expect) the model binder to set, and you need to be careful to avoid an “over-posting” attack. 
1. What is explicit model binding? Explain.

	-Throws an exception if something goes wrong during model binding and the model is invalid./Has an override allowing you to specify an includeProperties parameter. 