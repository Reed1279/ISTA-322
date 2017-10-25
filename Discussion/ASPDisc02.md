# Course: ISTA-322
## Lesson Plan: 02
### Name: Tyler Reed
#### Date: 24 October 2017

1. Examine the following code. Then explain what this code does, line by line.
$(function () {
	$("#album-list img").mouseover(function () {
	$(this).animate({ height: '+=25', width: '+=25' }).animate({ height: '-=25', width: '-=25' });
	});
});

	-The first line calls a function. The second line binds an img from the albums list that runs when the mouse moves over it.  The third line sets the perameters of the action from line 2.  The mouseover funtion is a toggle that most likely switches the item between two visually distinct appearances.
1. Write the jQuery code that selects all the hyperlinks in the menu block level element (<dev> that are
descendants of the menu division. Write the jQuery code that selects all the hyperlinks in the menu
block level element (<dev> that are children of the menu division. What is the diiference between the
two?

	-
1. Describe the Document Object Model (DOM).

	-A cross-platform and language-independent application programming interface that treats an HTML, XHTML, or XML document as a tree structure wherein each node is an object representing a part of the document.
1. How do you write Unobtrusive JavaScript? Describe the process.

	-Through the process of creating web pages and applications using a collection of good programming practices. Keeping separate the JavaScript, CSS, and HTML elements of your application. Using JavaScript to progressively enhance your application—don't use JavaScript for core functions.  Maintaining your code structure in such a way that reduces repetition, is better organized, and is easier to read and maintain.  Adhering to web and accessibility standards.
1. How do you add a script reference to a web application in ASP.NET? How do you add a script bundle
to a web application in ASP.NET? What is the diference between the two?

	-By using a script manager.  You can use new ScriptBundle or ViewBag.
1. I you to write your own custom JavaScript, where in the application directory structure might you
place it?

	-In the Js/Lib directory
1. What is the main purpose of using AJAX in web applications? Explain why you would want to do so.

	-It eliminates the start-stop-start-stop nature of interaction on the Web by introducing an intermediary — an Ajax engine — between the user and the server. allows the user’s interaction with the application to happen asynchronously — independent of communication with the server.
1. What are data dash attributes? Why do we use them? Do web browsers render them? Why or why
not?

	-Attributes you can embed nearly anything inside, and they are easy to consume from jQuery. Some.  You have to monkey around with it a bit.
1. How do you activate client side jQuery validation? How do you activate server side validation wit
ASP.NET?

	-The RequiredField Validator for the TextBox can be enabled or disabled by checking or unchecking the CheckBox respectively. 
1. You have an 11 character product model code that consists of four upper case alphabetical characters,
four digits, and three upper case alphabetical characters. As example would be ABCD4567XYZ. Write
a custom validation method to validate user input as to your model code.

	-<h:inputText id="code" value="#{ProductModel.code}"
            size="11" ... >
    <f:validator validatorId="ABCD456XYZ" />
