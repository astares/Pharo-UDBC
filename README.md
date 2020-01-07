# Pharo-UDBC
Pharo Universal Database Connectivity


```Smalltalk
Metacello new 
	repository: 'github://astares/Pharo-UDBC/src';
	baseline: 'UDBC';
	load
```

# For SQlite3

Old:
```Smalltalk
Metacello new 
	repository: 'github://astares/Pharo-UDBC/src';
	baseline: 'UDBC';
	load: 'SQLite'
```

New: please now use [https://github.com/pharo-rdbms/Pharo-SQLite3](https://github.com/pharo-rdbms/Pharo-SQLite3) for SQlite3 only

# Roadmap for SQLite3

- Implement support for
  [SQLcipher](https://github.com/sqlcipher/sqlcipher). This was available
  in NBSQLite, the SQLite binding using Pharo 4's NativeBoost FFI.

- Implement driver for [Voyage](https://github.com/pharo-nosql/voyage). 


