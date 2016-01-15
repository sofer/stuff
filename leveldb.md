# LevelDB

LevelDB is a key-value store, written by Jeff Dean and  Sanjay Ghemawat at Google. What makes it interesting to Node developers is the LevelUp npm pacakage, which allows LevelDB to be included within a Node application.

A number of contributors have created npm modules that allow LevelDB to be used as the basis for a graph, a relational or a document store. In addition, LevelUp can be used not just with LevelDB, but with other databases, such as RocksDB. 

This approach allows us to create a database for an application that meets our needs, while not forcing us to re-write all the database abstraction layer that an external database usually gives us. It means that we can use a single and very fast data store for a number of different use cases. It also allows us to swap out the data store, if we need to.

From a learning perspective, we can concentrate on thinking about (and implementing) different data abstractions, rather than spending time on understanding and installing a specific database, such as MongoDB or PostgreSQL. By making the database less of a black box, we are likely to get a better understanding of what we want a database to do for us and how.

One key feature that is hard to implement in LevelDB, but is available in forks such as HyperLevelDB and RocksDB, is live backup. Both HyperLevelDB and RocksDB are available as npm modules.

## Tutorial


## References

+ LevelDB and Node: [What is LevelDB Anyway?](http://dailyjs.com/2013/04/18/leveldb-and-node-1/) and [Getting Up and Running](http://dailyjs.com/2013/05/02/leveldb-and-node-2/) by Rod Vagg
+ [LevelDB website](http://leveldb.org/)
+ [LevelUp repo on GitHub](https://github.com/Level/levelup)
+ [List of community-written modules](https://github.com/Level/levelup/wiki/Modules) on the LevelUP wiki
+ [Level Me Up Scotty!](https://github.com/workshopper/levelmeup) (nodeschool tutorial)
+ [Intro to LevelDB by Kyle Young](https://youtu.be/sR7p_JbEip0) (video tutorial)
+ [Level](https://github.com/Level/levelup/wiki/Modules)
+ [Rod Vagg: A Real Database Rethink: "Introducing LevelDB and Node.JS" NodeconfEU2013](https://youtu.be/C-SbXvXi7Og) (video)
+ [Dominic Tarr: A Modular Database?](https://youtu.be/4_22ie--Rzs) (video)
+ [Julian Gruber: Level Me up Scotty!](https://youtu.be/41oDDTRWjIQ) (video)
+ [Matteo Collina - How to cook a Graph database in a Night](https://vimeo.com/110115775) (video)
+ [Max Ogden at LXJS 2012: JavaScript Databases!?](https://youtu.be/FDDpEBRGdew) (video)
+ [Rod Vagg  at LXJS 2013: JavaScript Databases 2](https://youtu.be/-vD33vPKcAM) (video)

### Also:

**Rocks** (Facebook)  
+ [RocksDB](http://rocksdb.org/)
+ [level-rocksdb](https://github.com/Level/level-rocksdb)
+ [RocksDB: A High Performance Embedded Key-Value Store for Flash Storage - Data@Scale](https://youtu.be/V_C-T5S-w8g) (video)
+ [a Node.js-style RocksDB wrapper](https://github.com/Level/level-rocksdb)

**Riak**  
[Basho clone of LevelDB](https://github.com/basho/leveldb)
[Optimizing LevelDB for Performance and Scale - RICON East 2013](https://youtu.be/vo88IdglU_8)

**HyperLevelDB**  
+ [HyperLevelDB](https://github.com/rescrv/HyperLevelDB)
+ [level-hyper](https://github.com/Level/level-hyper)

**SSDB**  
+ [SSDB](https://github.com/ideawu/ssdb) (*"an alternative to Redis"*)

### On backing up:
+ [How to backup RocksDB?](https://github.com/facebook/rocksdb/wiki/How-to-backup-RocksDB%3F)
+ [HyperDex Question](https://github.com/Level/level-hyper/issues/1)


