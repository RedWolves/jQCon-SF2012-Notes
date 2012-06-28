# Beyond the DOM: Sane Structure for JS Apps

## Rebecca Murphy

### Abstract

In the bad old days of JavaScript, our days were spent fighting through a thicket of DOM differences. These days, we've pretty much conquered those challenges thanks to tools such as jQuery, but our new challenge is figuring out how to adapt as more and more of our application logic moves from the server to the client. We have great tools like Backbone, Ember, Knockout, and more, but in order to use them effectively, we need to do more than learn their APIs -- we need to learn to think about our code beyond the DOM-centric ways of the past. In this talk, I'll look at useful patterns for thinking about client-side application development that will help you avoid creating a tangled mess of code.

## Notes
* [Slides available online](https://speakerdeck.com/u/rmurphey/p/jquery-conference-sf-2012-beyond-the-dom-sane-structure-for-js-apps)
* Logic of applications are moving more and more to the client side. 
* A simple search application can produce a lot of spaghetti jQuery code that looks ugly. 
* As your application gets more and more complex you need to rethink how you architect your application
* Client side MVC
	* Examples
		* AngularJS
		* BackboneJS
		* CanJS
		* Ember
		* Knockout
	* When is it time to start thinking about using a MVC library?
		* if you're asking it now is the time. 
	* How do you choose which one to use?
		* There isn't a solid answer to this question
		* try them 
			* go to TODO MVC for examples of each
* RequireJS
	* We might have our code in more then one file
	* we want as few files as possible
	* RequireJS allows you to express which views are required on which pages. 
	* RequireJS has one script tag and points to a configuration file. 
* Demo
	* [Live demo](http://srchr-demo.nodejitsu.com)
	* Walked through code which is available on [Github](https://github.com/rmurphey/srchr-demo)
	