# The transformation priority premise

When doing test-driven development, the aim is to start with a very simple function returning nothing and with the simplest possible failing test for that function. You will then add tests one-by-one until you have generalised the function enough that it will pass any conceivable test. 

As you get each new test case to pass, you are likely to begin to see repetition in your code that will need to be refactored to make the function more general.

Bob Martin's premise is that your refactoring will take the form of a series of simple transformations and that you should aim to apply these transformations in a specific order.

+ `({}–>nil)` no code at all->code that employs nil
+ `(nil->constant)` re
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

Maybe the most notable thing to note from this list is that variable assignment and multiple branching should be treated as last resorts. One other thing to note is that a conditional `if` can be seen as a degenerate case of a loop; a single condition is quite likely to generalise to a loop.

Another thing to note is that it is very important to start with the most simple tests first. If you find yourself unable to follow this general priority order, then go back and check that you are applying the most simple tests first. 

## References

+ [Bob Martin's original blog post](https://blog.8thlight.com/uncle-bob/2013/05/27/TheTransformationPriorityPremise.html)
+ [Bob's update to the original priority list](https://blog.8thlight.com/uncle-bob/2013/05/27/FibTPP.html)
+ [Wikipedia article on the transformation priority premise](https://en.wikipedia.org/wiki/Transformation_Priority_Premise)
+ [A comic-strip explanation of using the premise for sorting](https://blog.8thlight.com/uncle-bob/2013/05/27/TransformationPriorityAndSorting.html)
+ [Corey Haines' roman numerals run-through in Ruby](https://youtu.be/vX-Yym7166Y)
+ [Pedro Santos on the premise applied to the roman numerals kata in Java](http://codurance.com/2015/05/18/applying-transformation-priority-premise-to-roman-numerals-kata/)
+ [Bob using the premise to find prime factors in Java at NDC 2011](https://youtu.be/B93QezwTQpI?t=19m22s) (video)
+ [Joseph Yao on applying the premise to the Numbers in Words kata in Java](http://www.infoq.com/presentations/tpp-tdd) (video)
+ [Micah Martin on the applying the premise in Clojure](http://blog.8thlight.com/micah-martin/2012/11/17/transformation-priority-premise-applied.html)
+ Micah on the absolute priority premise, [Part One](https://vimeo.com/57851350) and [Part Two](https://vimeo.com/59265614) (videos)
