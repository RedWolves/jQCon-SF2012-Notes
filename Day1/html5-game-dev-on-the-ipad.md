# HTML5 Game Dev on the iPad

## Daniel Cohen

### Abstract

Our team has learned great lessons while developing Fashion Tale, a hidden object game entirely in HTML5. The process taught us several tricks, pitfalls, and successful workarounds. This talk covers using hardware accelerated graphics, responding effectively to touch events and gestures, and creating actionable feeds and message centers using jQuery.data().

## Notes

* Developer of Fashion Tale
	* Built with jQuery/HTML5
* The Mechanics
	* Simplicity is fine. Concentrate on short
	* Update levels without resubmission
	* Plan to share
	* Plan for Ads
	* Plan for stats
* Structure
	* iFrames for views
	* Minimal HTML skeleton
	* Ajax calls for game-state, messaging feeds, and purchasing options
	* In house wrapper (similar to PhoneGap)
* Beyond the front-end
	* A wrapper (for offline)
	* DB Connection
* DOM Elements vs Canvas
	* iPad dev = one CSS prefix
	* DOM Elements > canvas draws
	* repeated calls are super fast
	* CSS re-sizes to every resolution
* The CSS
	* Curve paths using 2 elements
	* Avoid opacity & Box shadow
	* Use -webkit transforms first
	* Pseudo Elements don't add leaves
* The Events
	* webkitAnimationEnd & webTransitionEnd are your friends
	* click vs onTouchStart
	* original event for touches / gestures
	* onorientationchange and media queries
* The JS
	* $.fn() is a perfect generator for feed pages
	* $.data() is great to save info from JSON
	* Put it in an iFrame, use it, and toss it
* Migration / Expansion
	* Other webkit tablets - Easy
	* Other webkit phones - Medium Easy
	* The desktop world - more difficult
