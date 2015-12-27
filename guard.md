# Guard clause

If there are any special conditions that a function has to deal with, such as checking the value of the input arguments, then put them at the top of the function. 

For example, do this:

    var merge = function (x, y) {
      if (x === undefined) return y;
      if (y === undefined) return x;
      // merge x and y here
    }

Instead of this:

    var merge = function (x, y) {
      if (x !== undefined) {
        if (y !== undefined) {
          // merge x and y here
        } else {
          return x;
      } else {  
        return y;
      }
    }

## References

+ [Entry in the Portland Pattern Repository](http://c2.com/cgi/wiki?GuardClause)
+ [Wikipedia entry for Guard](https://en.wikipedia.org/wiki/Guard_(computer_science))
