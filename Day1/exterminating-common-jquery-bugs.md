# Exterminating Common jQuery Bugs
## Elijah Manor

### Abstract
jQuery is so easy to use and thankfully abstracts many of the cross-browser concerns we used to labor over years ago. As with any library, however, there are a common set of bugs that tend to crop up as you start and continue to use it more and more. This session aims to help equip developers with the appropriate knowledge and tools to exterminate a subset of these common issues.

For each topic that is covered we will start with an example piece of code that contains a jQuery bug, then expose what the bug is, explain why it is happening, proceed to explore various techniques to exterminate the bug, and in some cases provide extra insight surrounding the problem.

These solutions range from simple to advanced concepts. By exterminating bugs in multiple ways it will help expose some of the newer and more advanced features of jQuery that aren't as widely known.

Some of the bugs that we will address involve dealing with synchronous and asynchronous code, uncovering some possibly confusing aspects of the $.each() method, uncovering why some animations have a mind of their own, explaining the difference between bind(), live(), delegate(), and live(), explaining why and how you might have killed event delegation, explaining the difference between commonly confused jQuery methods, problems when reusing a method as an event handler, and more.

## Notes
* Bugs meaning bugs in our application code
	* common bugs on StackOverflow or the jQuery Forum
* Chicken or the Egg problem
	* With an ajax call developers commonly think that the callbacks are called synchronously.  In fact it happens asynchronously. 
		* so if you write an action that happens in the success callback and then have some styling functions that happen in the complete callback those two functions happen at the same time and you won't get the desire result.
* Give me truth problem
	* Testing the truthiness of a jQuery object is always going to be true cause.  i.e. using the .not() method
	* the .not method is commonly confused to return if the elements exists or not which it isn't.  The correct method is the .is method
* Animations gone wild problem
	* Animations run in a queue and the next animation will wait till the first is complete before running the next. 
	* sometimes you want it to stop.  Developers commonly don't use the .stop() method to stop and start a new queue of animations
	* example of this problem can be seen in a dropdown menu and you go back and forth across the menus fast and then stop the animations are all queued up. 
	* Some ways of accomplishing delaying menu's opening
		* hoverIntent plugin
		* Ben Alman's $.doTimeout jQuery plugin which is a wrapper around window.setTimeout() 
* Defective Data problem
	* The $.data() method reads from the DOM only once. So setting the data attribute with $.attr() method after the page load the data will not be read again. 
	* Don't use $.attr() to update date attributes use the $.data() method.
	* Extras
		* $.data() automatically does type conversion for you
* Erratic events problem
	* Using return false; has unintended effects when you have multiple events on the page. Event delegation will not happen with return false;
	* use e.preventDefault(); or e.stopPropagation(); instead 
* Switching to the .on() method problem
	* you can't just switch $.live() to $.on() because the $.on() syntax is slightly different that equates to the $.live() functionality.