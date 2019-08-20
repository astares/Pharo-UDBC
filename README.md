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
