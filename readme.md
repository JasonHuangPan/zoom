## About Zoom

A small jQuery plugin for zooming images on mouseover or mousedown. See the [project page](http://jacklmoore.com/zoom/) for documentation and a demonstration.  Released under the [MIT license](http://www.opensource.org/licenses/mit-license.php).
 
## Changelog:

### v1.7.7 - 2013/7/14
* Restricted grab to just the left-mouse-button on mousedown

### v1.7.6 - 2013/6/24
* Fixed misnamed onZoomOut callback

### v1.7.5 - 2013/6/19
* Fixed a bug with absolutely or fixed position target elements
* Set the value of `this` to be zoom-image element for the onZoomIn and onZoomOut callbacks

### v1.7.4 - 2013/6/18
* Namespaced events to assist unbinding events.
* Added destroy event to unbind zoom events & remove created img element. Example:
	$('.example').trigger('zoom.destroy');
* Added onZoomIn and onZoomOut callbacks

### v1.7.3 - 2013/6/10
* Fixing mistake made in previous commit

### v1.7.2 - 2013/6/6
* Replaced new Image() with document.createElement('img') to avoid a potential bug in Chrome 27.

### v1.7.1 - 2013/3/12
* Replaced jQuery shorthand methods with on() in anticipation of jQuery 2.0

### v1.7.0 - 2013/1/31
* Added 'toggle' behavior to zoom in/out on click.  Example: $('#example').zoom({ on:'toggle' });
* Removed the icon property in favor of just using CSS.

### v1.6.0 - 2013/1/22
* Created $.zoom which contains the positioning logic, so that users can write custom controls or event handling.

### v1.5.0 - 2012/11/19
* Added 'target' property for specifying the element that displays the zoomed image.

### v1.4.0 - 2012/9/29
* Changed API & added option to activate on click.

### v1.3.0 - 2011/12/21
* Added 'callback' property that will execute a callback function once the image has loaded.
* Fixed a bug relating to the 'grab' property

### v1.2.0 - 2011/11/15
* Fixed a positioning bug

### v1.1.0 - 2011/11/15
* Added 'grab' property

### v1.0.0 - 2011/11/11
* First release