jQuery Fundamentals Summary
===========================

Chapter 3 - Traversing & Manipulating
_____________________________________

### September 20, 2015

There are so many fun things you can do with jQuery! This chapter discusses traversing and manipulating the DOM with jQuery.

jQuery lets us move through HTML elements. We make an initial selection, we move through DOM relative to that selection, and we change our initial selection as we move. Sometimes we replace that selection entirely with a new selection. Because we move through the DOM, it is important to have a very solid HTML to start before we traverse.

Some methods for traversing:
* .first() .last()
* .siblings()
* .next() .prev()
* .parent()
* .children()  // immediate children of the selection
* list.find(’li’) // get ALL list items in the list, * including nested ones
* listItem.parents(’.module’) // all ancestors of list * item with class of ‘module’
* listItem.closest(’.module’) // find closest ancestor * of list item with class of ‘module’

For adding:
* var X = list.add(’#mylist li’);

To get back to initial selection:
* .end() // use it sparingly!

To add original selection to current selection:
* .addBack()

Manipulation methods allow you to alter the DOM. These methods return jQuery objects on which they were called, and you can chain these methods with other jQuery methods.

For example, we can add and remove class:

* addClass(’hidden’), removeClass(’hidden’)
* toggleClass(’hidden’) === add if not present, remove if present

Change CSS style:
* .css() to change style!
  * Changes the element directly

Change form values:
* .val() === alter elements like select and input
* $(’input[type=“text”]’).val(’new value’);
* $(’select’).val(’2′);
* $(’input[type=“checkbox”]’).prop(’checked’, ‘checked’);

Changing other attributes:
* .attr()
  * Example: Set a new title attribute for a link:
  * $(’a’).attr(’title’, ‘Click me!’);
* When setting an attribute, you can pass a function as a second argument. Like setter methods, this function receives 2 arguments: index of the element, and original value of the attribute.
* $(’a’).attr(’href’, function(index, value) { return value + ‘?special=true’; });

Here are methods for placing elements in the document:
* .appendTo()
* .append()
* .insertAfter() // insert after the last list item
* .after() // insert after the last list item

Complete copy of a selection to be used elsewhere:
* .clone() // copy element

Removing elements using jQuery:
* .remove()
* .detach()
* .replaceWith()




