# Pharo-UDBC
Pharo Universal Database Connectivity


```Smalltalk
Metacello new 
	repository: 'github://astares/Pharo-UDBC/src';
	baseline: 'UDBC';
	load
```

# Only load SQLite3

```Smalltalk
Metacello new 
	repository: 'github://astares/Pharo-UDBC/src';
	baseline: 'UDBC';
	load: 'SQLite'
```

# Roadmap for SQLite3

- Implement support for
  [SQLcipher](https://github.com/sqlcipher/sqlcipher). This was available
  in NBSQLite, the SQLite binding using Pharo 4's NativeBoost FFI.

- Implement driver for [Voyage](https://github.com/pharo-nosql/voyage). 


