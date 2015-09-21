jQuery Fundamentals Summary
===========================

Chapter 2 - jQuery Basics
_____________________________

### September 20, 2015

This chapter starts digging a little further into jQuery, and goes over the jQuery basics. jQuery is a library used to manipulate the HTML page after it’s been rendered in the browser. It creates interactivity with the user/viewer of the page, creates animations for selected elements, and provides tools for communicating with a server without reloading the page ($ajax).

The ‘$’ is reserved for calling a jQuery function. To begin writing a jQuery function, we can use the $ to start:

* $(document).ready()
  * Shorthand for this is: $function( ) { ... do stuff }

Selectors used in jQuery can be elements with ID, class names, or just the elements themselves. All CSS selectors apply here. The selections must be elements that are already in the page when the selection is made. They cannot be created after.

To create jQuery objects, there are many ways:

* $(document.body.children[0]); // create jQ object from DOM element
* $([window, document]); // create jQ obj from list of DOM elements
* var firstBodyChild = document.body.children[0]; $(’li’, firstBodyChild); // make selection in context of DOM elements
* var paragraph = $(’p’); $(’a’, paragraph); // make selection within previous selection

It is precautionary to set up a function to check if a selection can be used or not. In regards to truthiness, we know 1 is truthy and 0 is falsey. Therefore, we can set up an if statement:

* if ($(’#nonexistent’).length) { ... this will only run if this matches }

Other ways to work with jQuery selections:

* Getting single element from selection
  * var listItems = $(’li’); var secondListItem = listItems.eq(1)
  * // We can get to a particular element by index number

* Creating new elements
  * $(’<p>Hello!</p>’) creates new <p> element with content
  * Can also create by passing an object with info
  $(’<p>’, { html: ‘Hello!’, ‘class’: ‘greet’});

* Testing selection
  * .is() method -- returns true/false
  * $(’li’).eq(0).is(’.special’); // false
  * .... eq(1).... // true

This chapter discusses setter methods, which I am not completely clear on. I think it is for setting (or changing) content in the HTML? The example first uses .html() to change the text, then uses another jQuery function to return the previous text (before the change:

* $(’li’).html(function (index, oldHTML) { return oldHTML + “!!!” });

And of course, we talk about the use of ‘this’ in jQuery! It is a very special keyword, used similarly in JavaScript, to refer to the selection in question within the context of the function.
