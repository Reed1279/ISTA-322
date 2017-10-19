# Course: ISTA-322
## Lesson Plan: 01
### Name: Tyler Reed
#### Date: 18 October 2017

1. What is the difference between authentication and authentication?

	-Authentication means verfying the user is a valid user with username and password. Authorization is the permissions of a valid user. So once the user is authenticated, his permissions are assigned using authorization so the access over resources is controlled.
1. What three conditions does the ObAuthorization method check?

	-AuthorizeCore, IAuthorizationFilter, AuthorizationContext
1. How do you register the AuthorizeAttribute as a global filter?

	-You have to set the authetication to a controller class
1. How do you activate the authorization filter in ASP.NET MVC 5?

	-Apply authentication filters 
1. What is the difference between OAUTH and OPENID? Explain.

	-OpenID is a protocol for authentication while OAuth is for authorization. Authentication is about making sure that the guy you are talking to is indeed who he claims to be.
1. How are authorization providers configured?

	-Through security realms
1. How do you prevent user log in information from being intercepted during log in?

	-Scripting
1. How do you carry out an attack by XSS?

	-By injecting malicious scripts into trusted sites
1. How do you carry out an attack by XSRF?

	-You trick a victim into performing actions on behalf of the hacker.
1. How do you carry out an attack by cookie stealing?

	-You need to exploit the page using XSS
1. How do you carry out an attack by over posting?

	-??
1. How do you carry out an attack by open redirection?

	-You modify the returnUrl to inject any URL address into the parameter to conduct an open redirection attack.