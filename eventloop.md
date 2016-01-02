# The JavaScript event loop

[unfinished]

*"Q: JavaSCript, what are you?"*
*"A: I am a aingle-threded non-blocking asynchronous concurrent language. I have a call stack, an event loop, a callback queue, some other APIs and stuff"*

V8: has a call stack and a heap, but there's no SetTimeout in V8.

JavaScript runtime: a heap and a stack

Single-threeded: has a single call stack

Can run a single piece of code at at a time

Data type: a classificantion of different kinds of data into well-defined types that define what values those different kinds of data can take and what behaviour they exhibit. There are generally recognised to be three classes of data type: primitive data types, such as , such as integer, boolean, character, floating-point number; composite types, such as arrays, sets or records; and abstract data types.

Abstract data type: a data type, such as a queue, stack, hash or tree, that can be implemented using one or more composite types.

A stack: an abstract data type that operates as a last-in, first-out list.

Call stack: a presentation of program state. When a function is called it is added to the top of the stack. When the function returns, it is removed from the the top of the stack and the program returns to the state it was in when the function was called. The JavaScript runtime, in common with most programming language runtimes, has a pre-defined call stack size and if too many functions are called without first returning, the runtime will return a stackoverflow error. (`RangeError: Maximum call stack size exceeded).

Blocking
Asynchronous callbacks
Web APIs
Render queue
Callback queue
Callbacks
Single threaded

Anyway, just [watch the talk](https://youtu.be/8aGhZQkoFbQ)

## References

+ [https://youtu.be/8aGhZQkoFbQ](https://youtu.be/8aGhZQkoFbQ)
