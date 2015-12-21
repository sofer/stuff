# The transformation priority premise

Bob Martin's premise is that when doing the red-green-refactor approach to test-driven development, you will find yourself applying a series of simple transformations to your code to get each successive test to pass, and that you are less likely to get stuck or to have to do significant refactoring if you stick to the following priority order for your transformations, starting with those at the top and moving down the list one step at a time as you introduce each new test:

+ `({}–>nil)` no code at all->code that employs nil
+ `(nil->constant)`
+ `(constant->constant+)` a simple constant to a more complex constant
+ `(constant->scalar)` replacing a constant with a variable or an argument
+ `(statement->statements)` adding more unconditional statements.
+ `(unconditional->if)` splitting the execution path
+ `(scalar->array)`
+ `(array->container)`
+ `(statement->tail-recursion)`
+ `(if->while)`
+ `(statement->recursion)`
+ `(expression->function)` replacing an expression with a function or algorithm
+ `(variable->assignment)` replacing the value of a variable.
+ `(case)` adding a `case` (or `else`) to an existing `switch` or `if`

If you find yourself unable to follow this general priority order, then go back and look at your most recent test and see if you can replace it with a different test that will allow you to pass with a higher-priority transformation.

## References

+ [Bob Martin's original blog post](https://blog.8thlight.com/uncle-bob/2013/05/27/TheTransformationPriorityPremise.html)
+ [Bob's update to the original priority list](https://blog.8thlight.com/uncle-bob/2013/05/27/FibTPP.html)
+ [Wikipedia article on the transformation priority premise](https://en.wikipedia.org/wiki/Transformation_Priority_Premise)
+ [Corey Haines' roman numerals run-through in Ruby](https://youtu.be/vX-Yym7166Y)
+ [Micah Martin on the applying the premise in Clojure](http://blog.8thlight.com/micah-martin/2012/11/17/transformation-priority-premise-applied.html)
+ [A comic-strip explanation of using the premise for sorting](https://blog.8thlight.com/uncle-bob/2013/05/27/TransformationPriorityAndSorting.html)
+ [Pedro Santos on the premise applied to the roman numerals kata in Java](http://codurance.com/2015/05/18/applying-transformation-priority-premise-to-roman-numerals-kata/)
+ [Bob using the premise to find prime factors in Java at NDC 2011](https://youtu.be/B93QezwTQpI) (video)
+ [Bob again on prime factors at NDC 2014](https://vimeo.com/97516288) (video)
+ [Joseph Yao on applying the premise to the Numbers in Words kata in Java](http://www.infoq.com/presentations/tpp-tdd) (video)
+ Micah Martin on the absolute priority premise, [Part One](https://vimeo.com/57851350) and [Part Two](https://vimeo.com/59265614) (videos)
