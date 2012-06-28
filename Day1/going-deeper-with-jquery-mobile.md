# Going Deeper with jQuery Mobile

## Andy Matthews

### Abstract
Building a jQuery Mobile application is easy, but making it stand out from the pack takes work. This session will take an in-depth look at the inner workings of jQuery Mobile and show you how to get started with creating custom theming, custom icons, and even custom plugins.

## Notes
* [Slides are available online](http://www.andymatthews.net/read/2012/06/28/Slides-and-demos-from-jQuery-Con-2012)
* Files available for [download](http://goog.le/4CnpJ)
* [jqmgallery.com](http://jqmgallery.com) - user submissions of jQuery Mobile websites.
* Custom Icons
	* JQM ships with 22 icons
	* Andy made his own icons: [https://github.com/commadelimited/jQuery-Mobile-Icon-Pack](https://github.com/commadelimited/jQuery-Mobile-Icon-Pack)
	* Creating Icons Tips
		* start with 36x36
		* border to show available space 18x18
		* Export to PNG-24
		* Things to remember
			* Simpler is better
			* Work with vector shapes
			* subpixel rendering sucks
* Custom Themes
	* visual building blocks of JQM
		* Border-radius
		* linear-gradient
		* box-shadows
		* text-shadows
	* UI Framework
		* namespacing
			* ui-widget-theme
		* Bite-sized pieces
		* stacked styles
	* ThemeRoller demo
		* [http://jquerymobile.com/themeroller/](http://jquerymobile.com/themeroller/)
		* Import theme will only import the unminified version so keep the full css file around to be able to import and upgrade it. 
* Custom Plugins
	* Why write your own plugin?
		* Impress your friends
		* Learn something
		* You have a need
	* Getting Started
		* Start with an empty page
		* Copy existing plugin, make changes
		* Use Grunt - build tool for javascript
		
	