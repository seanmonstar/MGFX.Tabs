Class: MGFX.Rotater {#MGFX.Rotater}
=====================

The base Rotater class, can be used by itself for simple slideshows.

### Implements:

Events, Options

MGFX.Rotater Method: constructor {#MGFX.Rotater:constructor}
-----------------------------------------------

### Syntax:

	var tabs = new MGFX.Rotater($$('.panel'), options);

### Arguments:

1. slides - (*selector, collection*)
2. options - (*object*, optional)

### Options:

* **slideInterval**: (*int*) Time in milliseconds to remain on each slide. Default: 5 seconds.
* **transitionDuration**: (*int*) Time in milliseconds for the transition effect to take. Default: 1 second.
* **startIndex**: (*int*) A zero-based number for which Tab should be displayed first. Default: 0 (first Tab).
* **autoplay**: (*boolean*) Whether the tabs should automatically rotate. Default: false.
* **hover**: (*boolean*) Whether the mouse hovering over a tab should stop the autoplay. Default: true.
* **hash**: (*boolean*) Whether the Tabs should examine the hash of the URL to determine the startindex. Example: "example.com/portfolio#card". Default: true.


MGFX.Rotater Method: showSlide {#MGFX.Rotater:showSlide}
-------------------------------------

Changes the currently shown tab to the one at the specified index.

### Syntax:
		
		tabs.showSlide(1);


### Arguments:

1. slideIndex - (int)

### Returns:

* (*object*) This MGFX.Rotater instance.

### Events:

* onShowSlide

MGFX.Rotater Method: autoplay {#MGFX.Rotater:autoplay}
---------------------------------------------

Start the rotation of slides based on **slideInterval**.

### Syntax:
		
		tabs.autoplay();

### Returns:

* (*object*) This MGFX.Rotater instance.

### Events:

* onAutoPlay



MGFX.Rotater Method: stop {#MGFX.Rotater:stop}
-----------------------------------------

This stops the rotating started by [autoplay](#MGFX.Rotater:autoplay).

### Syntax:

		tabs.stop();

### Returns:

* (*object*) This MGFX.Rotater instance.

### Events:

* onStop



MGFX.Rotater Method: rotate {#MGFX.Rotater:rotate}
-----------------------------------------------------------

This changes the current showing slide to the next in the list.

### Syntax:

		tabs.rotate();

### Returns:

* (*object*) This MGFX.Rotater instance.

### Events:

* onRotate

Class: MGFX.Tabs {#MGFX.Tabs}
=====================

Extends base [Rotater](#MGFX.Rotater) class to use a set of controller buttons that function like Tabs.

### Extends:

MGFX.Rotater