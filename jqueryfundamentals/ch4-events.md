jQuery Fundamentals Summary
===========================

Chapter 4 - Events and Event Delegation
_______________________________________

### September 20, 2015

Events! Here's the fun part! We want the user to be able to click on a certain part of the page, or move the mouse over an element, and create events. We first need an event listener.

These shorthand methods for event binding corresponds to a native DOM event:

* .click()
* .blur()
* .change()
* .keydown()
* .keypress()
* .keyup()
* .mouseover()
* .mouseout()
* .mouseenter()
* .mouseleave()
* .scroll()
* .focus()
* .blur()
* .resize()

The .on() method is how all of the above works under the hood. Technically, we can write them out as this:
* $('li').on('click', function(){ .... });
* The "click" has been binded to 'li', our selection

There is a way to unbind an event!
* .off()
* $('li').off('click');

Namespaced event:
* If we want to unbind from a specific 'li', not ALL of the 'li'
  * $('li').on('click.logging', function() {
    console.log('a list item was clicked');
  });

  $('li').on('click.analytics', function() {
    registerClick();
    doSomethingElse();
  });
  $('li').off('click.logging');

* This code leaves the "analytics" untouched, but unbinds the logging related click.

Passing named functions as event handlers:
* This is useful if you want to use the same handler for different events or events on different elements.

* var handleClick = function() {
  console.log( 'something was clicked' );
};

  $( 'li' ).on( 'click', handleClick );
  $( 'h1' ).on( 'click', handleClick );

The event object:
* Whenever the event object is triggered, the event handler function receives 1 argument, an event object that is normalized across browsers.
* It's a good way to have better cross-browser compatibility and solve cross-browser issues

Prevent default action:
* There are ways to prevent the default "reload entire page from clicking something" with jQuery
* We do so by including .preventDefault() in our jQuery function

Event bubbling:
* When an event is triggered and it triggers other selectors all the way up the DOM
* Big no no!
* It's important to think about not only scope in JavaScript, but scope in selections in jQuery.
* Example:
  * When clicking on <a>, you're clicking on the <span> that's inside the <a>. The event still bubbles up to the <a> and the bound click handler is fired.

Event delegation:
* Because of bubbling, we can bind handlers to high-level elements, then detect which low-level element initiated the event.
* We can bind to high-level element, then specify the low-level within it.




