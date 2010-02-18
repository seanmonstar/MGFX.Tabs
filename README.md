MGFX.Tabs
===========

![Screenshot](http://mcarthurgfx.com/images/blog/mgfxtabs.jpg)

A simple to use Tabs plugin using MooTools. Uses your normal semantic mark-up, and only requires a single line to get your tabs going.

How to use
----------

Write some semantic HTML that describes your buttons and panes:

	#HTML
	<ul id="tabs">
		<li><a class="tab" href="#" id="one">One</a></li>
		<li><a class="tab" href="#" id="two">Two</a></li>
		<li><a class="tab" href="#" id="three">Three</a></li>
	</ul>
	<div id="home">
		<div class="feature">
			<img src="img/mgfxtabs1.jpg" alt="" />
		</div>
		<div class="feature"">
			<img src="img/mgfxtabs2.jpg" alt="" />
		</div>
		<div class="feature">
			<img src="img/mgfxtabs3.jpg" alt="" />
		</div>
	</div>

Invoke the constructor. The first argument is the tab buttons, the second argument is the tab panes.  A third optional argument is a set of options to override the defaults.

	#JS
	var tabs = new MGFX.Tabs('#tabs li a', '#tabs div');
	
Demo can be seen [here](http://seanmonstar.github.com/MGFX.Tabs/).

Uses [Fx.Elements](http://mootools.net/more#Fx.Elements) from MooTools More.

Options
-------

### Version 1.2.0
* **slideInterval**: (*int*) Time in milliseconds to remain on each slide. Default: 5 seconds.
* **transitionDuration**: (*int*) Time in milliseconds for the transition effect to take. Default: 1 second.
* **startIndex**: (*int*) A zero-based number for which Tab should be displayed first. Default: 0 (first Tab).
* **autoplay**: (*boolean*) Whether the tabs should automatically rotate. Default: false.
* **hover**: (*boolean*) Whether the mouse hovering over a tab should stop the autoplay. Default: true.
* **hash**: (*boolean*) Whether the Tabs should examine the hash of the URL to determine the startindex. Example: "example.com/portfolio#card". Default: true.

License
-------

MIT License. Copyright 2008-2010 [Sean McArthur](http://mcarthurgfx.com).