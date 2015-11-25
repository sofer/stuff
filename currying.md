# Currying

#### Why?
At the heart of all programming is the idea of [decomposition], where a complex problem is broken down into a series of simple steps. [Method chaining]&mdash;where a series of functions operate on a single object that gets transformed step-by-step as it passes through the function chain&mdash;is a common way of achieving this. The jQuery library uses this technique. *Currying* is a similarly-powerful way of decomposing a problem through chaining, which comes from purely functional languages, where&mdash;unlike in JavaScript&mdash;objects are not used to maintain state.

#### What?
A *curried* function is a function with two or more arguments that has been transformed into a function to which each of the original arguments can be individualy applied successively in a chain to get the same result.

    f(a, b, c) -> f'(a)(b)(c)

For this to work, the new function `f'` must take a single argument and return a new function that also takes a single argument. 

Crucially, the returned function will need to have access to the argument applied to the original function, in order to make use of it in the returned function.

*Currying* is a special case of the *partial application* of a function, where some of the arguments of the original function have been applied and a new function has been returned that can take the remaining arguments and compute the original function with all of the required arguments.

### How?

In ES6:

    function curry(f, ...args) {
      [ to do]
    }

In ES5:

    function curry(f) {
      [ to do]
    }

### See also
[Decomposition] | [Closures] | [Chaining]

## References
+ [John Resig on Partial Application in JavaScript](http://ejohn.org/blog/partial-functions-in-javascript/) *
+ [currying in JavaScript](https://medium.com/@kbrainwave/currying-in-javascript-ce6da2d324fe#.tbfzd4xib)
+ [A Beginner’s Guide to Currying in Functional JavaScript](http://www.sitepoint.com/currying-in-functional-javascript/)
+ [Currying on Wikipedia](https://en.wikipedia.org/wiki/Currying)
+ [Partial Function Application is not Currying](http://www.uncarved.com/articles/not_currying)
+ [What's the difference between Currying and Partial Application?](http://raganwald.com/2013/03/07/currying-and-partial-application.html)
+ [ECMAScript 6 and Currying](http://macr.ae/article/es6-and-currying.html)








