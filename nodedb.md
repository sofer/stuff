# Using databases with Node.js

There are a lot of databases to choose from and there are a lot of choices about how to connect to them. Whichever database you use, you will need some sort of library to get data to and from.

### A client library
A client library (or driver or adapter) provides a connexion to a database and access to commands specific to that database. 

Good examples of client libraries are the [Redis client for Node.js](https://github.com/NodeRedis/node_redis) or the [MongoDB Node.JS Driver](https://github.com/mongodb/node-mongodb-native).

### Object-relational mappers
An object-relational mapper is a single library that allows an application to access a database, often without having to worry too much about which database is actually being used, without having to care about database-specific commands, and without using SQL. 
Good examples of ORMs are [bookshelf.js](https://github.com/tgriesser/bookshelf), [Sequalize](https://github.com/sequelize/sequelize), [Waterline](https://github.com/sequelize/sequelize )and [Mongoose](https://github.com/Automattic/mongoose). Some ORMs, like Waterline work with many different databases and some, like Mongoose, work with just one.

The Ruby on Rails framework famously uses the Active Record ORM. ORMs are widely used, but not everyone likes them. The idea of using a single database-agnostic library that maps nicely to your data models is compelling, but can apparently cause problems with more complex or highly-trafficed applications.

## References
+ [Object-relational mapping](https://en.wikipedia.org/wiki/Object-relational_mapping) in Wikipedia
+ [Object-relational impedance mismatch](https://en.wikipedia.org/wiki/Object-relational_impedance_mismatch) in Wikipedia
+ [Object Relational Mapping Costs Time And Money](http://c2.com/cgi/wiki?ObjectRelationalMappingCostsTimeAndMoney)
+ [Object-Relational Mapping is the Vietnam of Computer Science](http://blog.codinghorror.com/object-relational-mapping-is-the-vietnam-of-computer-science/)
+ [OrmHate](http://martinfowler.com/bliki/OrmHate.html)
