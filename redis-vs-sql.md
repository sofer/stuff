# Redis vs SQL

Redis is a key-value store. 6 data types, 160 commands. Simple, fast, lightweight.

Redis makes you think. It's a *database copnstruction kit*.

No referentional integrity, no foreign keys.

Lots of duplication, no normalisation

Redis is ACID, because it is single-threaded: atomic. consistent, isolated.

It has transactions (but without rollbacks)

Indexes have to be built, using sets and zsets, they are not maintained automatically.

Redis is great for counting.

Widely used as a cache.
Good for ephemeral storage, e.g. a shopping cart

    CREATE TABLE redis (
      k VARCHAR(512MB) NOT NULL,
      v VARCHAR(512MB),
      PRIMARY KEY (k)
    )

Strings, integers, floats, bits, hash, sets, zsets

# References
[Redis Use Patterns: An Introduction to the SQL Practitioner](https://youtu.be/8Unaug_vmFI)
[Why and When You Should Use Redis](https://youtu.be/CoQcNgfPYPc)

