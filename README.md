# sqlite in C

In order to practice C and learn about database internals, I followed this awesome tutorial: (https://cstack.github.io/db_tutorial/)[https://cstack.github.io/db_tutorial/].

The database has a fixed schema of the following format:

| Id     | Username | Email     |
| ------ | -------- | --------- |
| uint32 | char[32] | char[255] |

## How to compile

```bash
cc db.c -o db
```

## Start REPL

The program requires a file to persist data. Supply a name to create one if it does not exist.

```bash
./db mydb.db
```

## Insert

Insert a row into the database.

```bash
insert 1 user1 person1@example.com
```

## Select

Print all rows in the database

```bash
select
```

## Print database in BTree format

```bash
.btree
```

## Exit REPL

Flush changes to database file and close REPL.

```bash
.exit
```
