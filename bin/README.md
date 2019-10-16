# Building the Windows DLL

Download and unpack the [SQLite source
amalgamation](https://sqlite.org/download.html).  The [how to compile
SQLite](https://sqlite.org/howtocompile.html) page states to use the
following MSVC command:

```
cl sqlite3.c -link -dll -out:sqlite3.dll
```

While this produces a DLL, said DLL doesn't actually export any symbol and
is thus useless for FFI. [This blog
post](https://protyposis.net/blog/compiling-sqlite-as-dll-with-msvc/) by
Mario Guggenberger provides the magic incantation:

```
cl sqlite3.c -DSQLITE_API=__declspec(dllexport) -link -dll -out:sqlite3.dll
```

