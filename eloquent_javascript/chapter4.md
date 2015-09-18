Eloquent Javascript Ch4 Summary
===============================

by Alina To
___________

### September 17, 2015

Chapter 4 covered data structures in JS, including objects and arrays. Objects allow us to group values together and build more complex structures. This chapter uses an example of a “weresquirrel” to examine how objects and data structures are important in working with Javascript. The “weresquirrel” keeps track of when he turns into a squirrel, and explores these individual journal entries (or data sets) to look for patterns.

This chapter looks at dot notation vs bracket notation. “When using a dot, the part after the dot must be a valid variable name, and it directly names the property. When using square brackets, the expression between the brackets is evaluated to get the property name. Whereas value.x fetches the property of value named “x”, value[x] tries to evaluate the expression x and uses the result as the property name.” Another difference between the two is that bracket notation can access key:value pairs where the key is a string, with multiple words. Dot notation may not access those key:value pairs.

This chapter also looks at this problem of “weresquirrel” and discusses correlation, a measure of dependence between variables, and uses a table to examine the data from the “weresquirrel” journal. A loop is applied to go over properties of the object (journal entries) and maps the events, which calculates a correlation number based on how often certain events occurred when the “weresquirrel” transformed.

Methods:

* length
* toUpperCase
* toLowerCase
* join (glue between array elements)

Operators:

* delete
* in

Array methods:

* push
* pop
* unshift
* shift
* indexOf
* lastIndexOf
* slice
* concat

Global variables are present as a property of an object. In browsers, global scope objects are stored in the window variable. In order to access them, you must call on window to access. Objects in general can also serve as maps, associating values with names. The in operator can be used to find out whether an object contains a property with a given name. The same keyword can also be used in a for loop to loop over an object's properties. (i.e. (for (var name in object))  )
