Eloquent Javascript Ch3 Summary
===============================

by Alina To
___________

### September 4, 2015

Chapter 3 discussed functions, scopes, closure, side effect, recursion, and code efficiency. It is important to remember that some functions produce a value (or a return value), while some other functions only produce a side effect to the greater block of code. The scope in which a block of code is nested in will create limitations to what that function will affect and how it will affect it.

In terms of closure, which I dealt with in an F2 problem, the book discusses what to do when local variables are no longer active because the function it is defined within is no longer active. Being able to reference a specific instance of local variables in an enclosing function is called closure. I recall closure being discussed in F2 when I was working with a problem with functions in which one of the functions did not have a “return” at the end of the function, which then it didn’t have closure. “A function that closes over some local variables is called a closure.” This can help from having to worry about the local variables and can give you something to work with in other functions.

The book describes a function as “freezing the code in its body and wrapping it into a package (the function value). So when you read “return function( … ) { … }”, think of it as returning a handle to a piece of computation, frozen for later use.” This goes back to what I’ve been understanding of the “Return Value”. Return can help close a function and its local variable, returns a value, which can be applied to other blocks of code.

In terms of efficiency of the code, the book explains that it is not important to worry until the program runs too slow. If it is too slow, figure out which parts take the most time and begin cleaning up those parts to create more efficiency, whether it might be spaces, variable names, or even the overall approach to the code.

Another piece this chapter touches on really begins to make clear of statements, expressions, and return values to me: “The “Function” keyword, when used as an expression, can create a function value. When used as a statement, it can be used to declare a variable and give it a function as its value.” The value in discussion is the return value of that function. The return value could be a variable or a function.
