# Cordova-sqlite-evcore-free-dependencies (evcore-ext build)

AUTHOR: Christopher J. Brody

LICENSE: GPL v3 (http://www.gnu.org/licenses/gpl.txt) or commercial license options

Contains source and library (shared object) code built from:
- [litehelpers / Android-sqlite-evcore-native-driver-free](https://github.com/litehelpers/Android-sqlite-evcore-native-driver-free) - GPL v3 or commercial license options
- [SQLite (sqlite.org)](https://sqlite.org/) - public domain

Also included in Android JAR build:
- [brodybits / sqlite3-regexp-cached](https://github.com/brodybits/sqlite3-regexp-cached) (based on <http://git.altlinux.org/people/at/packages/?p=sqlite3-pcre.git> by Alexey Tourbin, public domain)
- [brodybits / sqlite3-base64](https://github.com/brodybits/sqlite3-base64) (Unlicense, public domain)
- [brodybits / libb64-encode](https://github.com/brodybits/libb64-encode) (based on <http://libb64.sourceforge.net/> by Chris Venter, public domain)

This project provides the following dependencies needed to build Cordova SQLite evcore plugin versions:
- `sqlite3.h`, `sqlite3.c` - SQLite `3.15.2` amalgamation needed to build iOS and Windows versions
- `evcore-native-driver.jar` - Android-sqlite-evcore-native-driver-free NDK JAR built with SQLite `3.15.2` amalgamation, with the following option flags:
   - `-DSQLITE_TEMP_STORE=2`
   - `-DSQLITE_THREADSAFE=2`
   - `-DSQLITE_ENABLE_FTS3`
   - `-DSQLITE_ENABLE_FTS3_PARENTHESIS`
   - `-DSQLITE_ENABLE_FTS4`
   - `-DSQLITE_ENABLE_RTREE`
   - `-DSQLITE_ENABLE_FTS5`
   - `-DSQLITE_ENABLE_JSON1`
   - `-DSQLITE_DEFAULT_PAGE_SIZE=4096`
   - `-DSQLITE_DEFAULT_CACHE_SIZE=-2000`
