# New Perspectives on Performance

## Menno van Slooten

### Abstract
Performance. A word programmers use so often it's almost a buzzword. But in our world of web apps written in HTML, CSS and JavaScript it can mean many different, sometimes contradictory things.

In this presentation I will talk about the most common targets of web app performance, the techniques used to optimize them and how they influence each other. Additionally, I will discuss several performance targets that are mostly overlooked even though they arguably matter most.

## Notes
* Pillars of Performance
	* Visibility
	* Interactivity
	* Responsiveness
* Before you start optimizing…
	* Establish a baseline
		* Measurable
		* Repeatable
		* Stable
	* Always focus first on low-hanging fruit
	* Visibility
		* "High Performance Web Sites"" by Steve Souder
		* Install Firebug and YSlow
			* Do whatever YSlow tells you
		* Crowd source your measurements with Google Analytics
		* 8-bit PNG's with alpha: [http://8bitalpha.com](http://8bitalpha.com)
	* Interactivity
		* "Even Faster Web Sites" by Steve Souders
		* profile your $.ready();
		* delay initialization
			* Use $.one();
	* Responsivness
		* "High Performance JavaScript" by Nicholas Zakas
		* Throttle/debounce events
			* [http://benalman.com/projects/jquery-throttle-debounce-plugin/](http://benalman.com/projects/jquery-throttle-debounce-plugin/)
		* It's better to have something take 2 seconds and show progress then have something take 1 second and not show any progress.
* New Perspectives
	* Performance optimizations are expensive
	* Performance optimizations can increase costs
	