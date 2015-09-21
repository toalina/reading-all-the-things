jQuery Fundamentals Summary
===========================

Chapter 5 - Effects!
_______________________________________

### September 20, 2015

Finally! More fun stuff like effects and animations!

This chapter warns that in modern browsers, it is still more efficient to achieve animations using CSS rather than JavaScript. If only focusing on mobile devices or browsers, CSS is still the front-runner.
* Setting jQuery.fx.off to true on low-resource devices can cause animation methods to immediately set elements to desired outcome rather than animating/progressing to that outcome.

Built in Effects:
* These jQuery methods can be called on any jQuery objects:
  * .show()
  * .hide()
  * .fadeIn()
  * .fadeOut()
  * .slideDown()
  * .slideUp()
  * .slideToggle() // Show or hide selected elements with a vertical sliding motion

jQuery.fx.speeds:
* This can be used to reset an existing predevined speed. For example:
  * jQuery.fx.speeds.fast = 50;
  * jQuery.fx.speeds.turtle = 3000;

Providing a callback function to animation methods can dictate what will happen when the effect is complete. Inside the callback, 'this' refers to the raw DOM element that the effect was applied to.
* For example, we can make an element fadeOut at a specific speed, then a callback function to .remove() that element.

Custom effects with .animate():
* .animate() takes up to 3 arguments:
  * an object defining the properties to be animated
  * the duration of the animation (milliseconds)
  * a callback function that will be called when animation is complete

$('.blahblah').animate({
  left: '+=50',
  opacity: 0.25,
  fontSize: '12px'
},
300,
function() {
  // CALLBACK FUNCTION!
});

How to manage animations:
* .stop() // stop currently running animation
* .delay() // pause before execution of the next animation method, takes a number (milliseconds) for how long to pause
