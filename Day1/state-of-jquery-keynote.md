# State of jQuery

## Dave Methvin, Timmy Willis, Scott Gonzalez, Todd Parker

### Abstract

Learn about the progress on jQuery Core, jQuery UI and jQuery Mobile

## jQuery Core

* David is now the President and core lead
* jQuery Foundation
	*	organizes support for the jQuery Project and community
* jQuery 1.8
	* Only major release this year
 	* Adding CSS vendor prefixes
 	* Dumped uneeded code (Safari 2 for example)
 	* Deprecate "trip hazards"
 		* e.g. $.browser
 	* sets the stage for the future
 * Modularity
 	* New grunt build system
 	* For advanced users
 		* user must understand the dependencies
 		* no automation
	 * Size examples
	 	* Only require JSONP
	 		* 1.7.2 32KB
	 		* 1.8 w/only JSONP 24KB
	 * It's not easy
	 	* plugins released - block box of it's dependencies
	*closure compiler
		* experimental branch
* Future of jQuery
	* 1.9 
		* API cleanup
		* compatibility plugin
	* ERMAHGERD jQuery 2.0
		* Same API as 1.9
		* no feature additions
		* *No support for IE6, IE 7 not even IE8*
	* jQuery 1.9 is the solution for oldIE
	* Simplifying from removing code
		* Faster
		* Smaller
		* revisit design decisions
	* Not just Mobile - Modern browsers
		* mobile is not just iOS/Webkit
			* MSFT Surface
			* Responsive design?
		* 2.0 supports modern browsers
			* not just webkit
			* works everywhere
* Breaking the web?
	* supporting both versions
	* "Tears of joy" policy
		* include jQuery 1.9 for oldIE with conditional comments
* jQuery Core Future Growth
	* improve browser features to solve issues that exist everywhere
	* Use plugins for everything else
		* Touch events
			* Two non-standard implementations
			* can't include in core because of the non-standards
* Sizzle 
	* Faster in 1.8
		* Filter and matching
			* event trigger, simple, Complex, element-rooted ID are all faster vs 1.7.2
	* Bugs
		* Improved QSA/matchesSelector bug-detection
		* When using multiple combinators in the same selector some possible matches were being lost
		* Unicode Validations
	* Coming soon
		* more CSS3 selectors (after 1.8)
	* Contributing (http://github.com/jquery/sizzle)
		* Submit issues 
		* help fix bugs
		
## jQuery UI
* jQuery UI 1.9
	* Roadmap
		* Cleanup
			* API redesign
			* <10 bugs for all widgets
			* full accessibility for all widgets
		* New
			* Menu, Menubar
			* Tooltip
			* Spinner
			* Mask
			* Selectmenu
			* Datepicker rewrite
		* Overambitious goals
			* release now and gain some sanity
				* 1.9, 1.10, 1.11
		* 1.9 New Roadmap
			* API redesigns, bug fixes, accessibility
			* New widgets
				* Menu, spinner, tooltip
	* 1.9 BETA released this morning
		* 2098 commits
		* 201 tickets
	* 1.8
		* 27 mouths
		* 21 releases
		* one release over the last month
		* 2700 commits
	* 15% of the commits came from the community
	* API redesign
		* full back-compat for one major release
		* $.uiBackCompat = false;
			* forward compat testing
	* 1.10 roadmap
		* same pattern as 1.9
			* API redesign, bug fixes, accessibility
			* New widgets
				* menubar, selectmenu
			* Plan for better UI/Mobile integration
	* 1.11 roadmap
		* new widgets
			* mask, timepicker, effects
			* Globalize
	* 2.0 roadmap
		* Interaction rewrite
			* touch support
			* device/event agnostic base widget
		* More form controls
		
## jQuery Mobile
* 8 months since 1.0
* 1.1.1 in early July
* 1.2 in late July
* very popular internationally
* Compatibility and Accessibility matter
* Companies want to reach the broadest audience and why they are adapting jQuery mobile
* Ecosystem
	* Phonegap
	* codiqa
	* Dreamweaver 6
	* Microsoft MVC 4
	* WP7 Phone Theme
* Plugins
	* Rich set of plugins are available
		* [http://jquerymobile.com/resource](http://jquerymobile.com/resource)
* Team
	* 70 test devices
	* 1.0 team was 5 people
	* 6 new additions since 1.0
* contribute
	* Get involved in the issue tracker on github
	* Help us test
* Impact
	* Open issues 580  > 350
* What's Next
	* 1.1.1
		* RC1 released today
		* final release in 2 weeks
		* Features
			* Speedier (long) pages
			* Webview flicker resolved
			* Visual Consistency
	* 1.2
		* New Popup widget
			* can put any kind of widget inside of a pop-up
				* tooltips
				* popup menus
				* etc.
		* alpha next week
		* Goal: final release late July
	* Future releases
		* more releases
		* performance tuning
		* tablet optimizations
		* UI Harmonization (working with the jQuery UI project)
* Themeroller
	* Some changes in 1.1
		* version support
		* import feature for easy upgrading
* XML API Docs
	* just like core
* One more thing
	* Download builder
		* launched today
		* [http://jquerymobile.com/download-builder/](http://jquerymobile.com/download-builder/)	
		* will only work for 1.1.1+
		* It's Alpha	
* Donate devices
	* [http://jquerymobile.com/donate-devices/](http://jquerymobile.com/donate-devices/)