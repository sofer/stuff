# Somewhere to store data

A real software application needs somewhere to store its data.

**Choosing the right place to store your data is one of the most important choices you can make. It is very easy to make a choice that makes your life harder than it needs to be.**

The entire text of the Oxford English Dictionary takes around 540MB of storage space. That would comfortably fit in the Amazon EC2 free tier (1GB as of 2015). For many, many uses, it is entirely reasonable to keep all of an an application's data in memory, periodically saving updates to disk, but otherwise updating and querying the data directly from memory. 

...

**Most applications have simple application structures, simple transactional needs and not a lot of data by modern standards, so, unless you have complex query requirements or a lot of data to store, use a persistent data store that resides in memory and has an interface that is easy to use and that you are comfortable with.**

##References

+ [OED Dictionary Facts](http://public.oed.com/history-of-the-oed/dictionary-facts/)
