# Course: ISTA-322
## Lesson Plan: 03
### Name: Tyler Reed
#### Date: 19 September 2017

1. What is a view?

	-The UI and part of Three-Tier Architecture./An engine which is the component responsible for processing a view in order to generate a response for the browser./Used to render some part of the model as a user interface.
1. What is the similarity between view names and controller names? What is the diffrence between the two?

	-They are a part of the MVC pattern./Views contain the logic required to display elements of the model to the user—and nothing more, where Controllers are the bridge between views and the model
1. Where in the directory structure of an ASP.NET MVC application do
views live?

	-In the views folder
1. What is a ViewBag object? What does it do?

	-It is a Controller base class which can assign arbitrary properties, making those values available in whatever view is rendered.
1. What does the at symbol (@) do? Can you excape it? If so, how?

	-The magic character that precedes code instructions./Yes, by using // and /* *? comment delimiters
1. What are view conventions and how do they work?

	-Reverse of the default settings
1. What is a ActionResult object? How do these objects interact with views?

	-It is a class that lets you encapsulate and reuse common responses in actions.
1. What are strongly typed views?

	-A view intended to render a specific domain type, with shortcuts created by MVC.
1. How does Razor combine HTML and C# code?

	-by using markups, @ or <text> tags(varial interpulation)
1. Where do layouts live in the directory structure of an ASP.NET MVC application?

	-In the shared folder of the Views folder.
1. What are the dfferences between a partial view and a \full view?"

	-Partial view returns only the view content