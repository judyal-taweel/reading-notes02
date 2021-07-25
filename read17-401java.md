# Spring Boot and OAuth2

 several samples building:

 - simple :a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties.
 - click :adds an explicit link that the user has to click to login.
 - logout : adds a logout link as well for authenticated users.
 - two-providers: adds a second login provider so the user can choose on the home page which one to use.
 - custom-error: adds an error message for unauthenticated users.

 Google APIs use the OAuth 2.0 protocol for authentication and authorization. Google supports common OAuth 2.0 scenarios such as those for web server, client-side, installed, and limited-input device applications.
To begin, obtain OAuth 2.0 client credentials from the Google API Console. Then your client application requests an access token from the Google Authorization Server, extracts a token from the response, and sends the token to the Google API that you want to access. For an interactive demonstration of using OAuth 2.0 with Google (including the option to use your own client credentials), experiment with the OAuth 2.0 Playground.
This page gives an overview of the OAuth 2.0 authorization scenarios that Google supports, and provides links to more detailed content. For details about using OAuth 2.0 for authentication, see OpenID Connect.
