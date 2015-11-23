# Currying

[in progress]

A curried function is one to which one or more left-most arguments have been applied and a new function has been returned that can take the remaining unapplied arguments and compute the original function with all the required arguments.

A partially-applied function is a more general case of a curried function where the partially-applied arguments do not have to be at the beginning of the argument list, but can be at arbitrary points in the list.

Partial function application ia a technique that requires a language (like JavaScript) that has closures. The returned (i.e. partially-applied) function encloses over the context where it was called, a context which includes the original already-applied arguments, to which the function can refer whenever it is subsequently called.

Partial application is a great technique for abstracting out behaviour, so that it can be applied in different contexts without having to repeat the same code.

Contexts where partial application might be useful include: creating several different event listeners in the DOM that behave in similar, but not identical, ways...

### See also
[Closures] |


## References
[John Resig on Partial Application in JavaScript](http://ejohn.org/blog/partial-functions-in-javascript/) *

[How do JavaScript closures work?](http://stackoverflow.com/questions/111102/how-do-javascript-closures-work) *




"Partially applying a function is a, particularly, interesting technique in which you can pre-fill-in arguments to a function before it is ever executed...Filling in the first couple arguments of a function (and returning a new function) is typically called currying. " http://ejohn.org/blog/partial-functions-in-javascript/


*"a way of constructing functions that allows partial application of a function’s arguments. What this means is that you can pass all of the arguments a function is expecting and get the result, or pass a subset of those arguments and get a function back that’s waiting for the rest of the arguments...Currying is elemental in languages such as Haskell and Scala, which are built around functional concepts."* 

"coming up with a consistent naming convention for your curried functions will help make your code more readable. Each derived variation of a function should have a name that makes it clear how it behaves, and what arguments it’s expecting."

"Adding currying to your coding practice will encourage the use of partially applied functions throughout your code, avoiding a lot of potential repetition"

http://www.sitepoint.com/currying-in-functional-javascript/







