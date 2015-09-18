Eloquent Javascript Ch5 Summary
===============================

by Alina To
___________

### September 17, 2015

Chapter 5 delves into higher-order functions, discussing programs that contain more systems within a single file. A large program create more room for errors and making bugs hard to find. Abstractions can hide details and give us the ability to talk about problems at a higher level. For example, walking through each step in more concise and succinct ways with words that are more relatable to each other can create clean and effective code. Focus on higher-level concepts.

Functions can be written within one another, but each function should also be kept to performing a single task, in order to keep the code clean. Functions can be written to provide control flow in the system, like keeping control of which scope a function lives in as well as the variables involved. The book states, “An important difference is that variables declared inside inner functions do not end up in the environment of the outside function, and that is usually a good thing.” I think this is a good habit to form, in order to keep variables organized, unless there is a return from a function to be used elsewhere in the code.

JSON looks like Javascript, but it is non functional and contains data. A JSON can have methods applied, such as JSON.stringify and JSON.parse, which then can convert data from and to this format. Stringify takes a JS value and returns a JSON-encoded string. Parse takes a string and converts it to the value it encodes.

Map is a method used to transform an array by apply a function to all of its elements and building a new array from the returned values. Arrays provide a lot of useful higher-order methods, such as forEach, filter, map, and reduce (combine all of an array’s elements into a single value). Functions have an apply method (used to call something using an array specifying their arguments) and bind method, which creates a partially applied version of the function.

Between chapter 4 and 5, the idea of objects and single responsibility is well represented. I can see a lot of cross over concepts into CSS architecture, especially now that we have covered Sass in class. I think all of these concepts, on a much bigger scale, show the importance of keeping each thing you need (or small set of rules, or even one single rule) nice and tidy, very modular. And can be easily moved around, not completely dependent on another piece in the workflow.
