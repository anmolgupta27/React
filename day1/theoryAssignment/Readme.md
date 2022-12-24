What is Emmet?
 - Emmet is a free add-on to a text editor which is being used to write a small piece of code or abbreviation which is then expanded into a full piece of code.

 For Ex: -> div#page>div.logo+ul#navigation>li*5>a
  convert it into 
  <div id="page">
	<div class="logo"></div>
	<ul id="navigation">
		<li><a href=""></a></li>
		<li><a href=""></a></li>
		<li><a href=""></a></li>
		<li><a href=""></a></li>
		<li><a href=""></a></li>
	</ul>
</div>
It simply gives you boiler plate for the code you want to write.

Difference between a Library and Framework?
 - Library is providing predefined function or classes with the help of that you can create a application
 - Framework on the other hand is like the foundation upon which you are developing some applications
 - With library you can control the flow of your code, you can inject library anywhere call your function when required
 - With framework you cannot control, as framework will provide you some places where you can write your code or inject any library

What is CDN? Why do we use it?
 - CDN, is content delivery network servers that are geographically distributed to cache content closer to the user so that it will serve the content with minimum latency.
 - CDN are used to deliver content with minimum latency and also provide the same content to multiple users
 - CDN are formed long time back to cache the content and serve it to the requested IP
 - On the first request if Content is not cached then CDN will fetch that content first and then cache the response for other users while serving the newly fetch content to the user
 - Better performance, ensure availability of content and content security

Why is React known as React?
 - React is a library which is being used to change appData or view when user perform any event on the webpage, so to change the view or "react" with those user events. User events like click, scroll, form submit etc

What is crossorigin in script tag?
 - Crossorigin in script tag sets the mode for the HTTP CORS request, to handle cross origin requests
 - In webpages mostly we often make request to load resources from other servers so in order to get access to that server we need CORS attribute otherwise server will block our request
 - CORS = "anonymous"|"credential"
 - With anonymous all the request will be served
 - with credential we need to pass credentials, like cookie, token etc

What is diference between React and ReactDOM
 - React library is responsible to creating a view on the otherhand ReactDOM will handle DOM manipulations like changing the UI or view on the basis of user events
 - With React we are creating elements and ReactDOM will render those elements on the browser

What is difference between react.development.js and react.production.js files via CDN?

 - react.development.js is being mostly used for the development phase as it is not minified version so we are getting can caught errors and see those errors described in the console, whereas in react.production.js it is a minified version so the error displayed is also minified and it becomes difficult during development to debug as well.
 - So react.production.js files will be mostly used only on production so the build size is small and minified version will be there on the prod so that user will get better performance experience

What is async and defer?
 - Async and defer are two boolean attributes in the script tag
 - There are two phases to load the webpage one is html parsing and other is script fetching and executing
 - In normal scenario browser parse html and as soon as script tag is come in picture browser stop parsing and will fetch and execute the script tag and then continues with the parsing
 - When async attribute is true, browser start html parsing and in background script is fetching once the script is fetched then browser stop parsing and execute the script and then continues with the parsing
 - When defer attribute is true, browser start html parsing and in background script is fetching and once the html parsing is done then only script execution will happen.
 - Async attribute does not guarantee order of execution however defer attribute is maintaining the order of execution
 




