# SQLite

Types:
* NULL
* INTEGER: 1 to 8 bytes
* REAL: 8 bytes IEEE floating point number
* TEXT: uses DB encoding (UTF-8, UTF-16BE or UTF-16LE)
* BLOB: stored exactly as it was input

## Create

```shell
# create a DB
$ sqlite3 MyDb.db

# list existing databases
sqlite> .databases

# quit sqlite interpreter
sqlite> .quit

# dump db
$sqlite3 MyDb .dump > MyDb_dump.sql

# restore db from dump
$sqlite3 MyDb_dump.sql < MyDb.db
```
