# HandlerSocket plugin for MySQL Improved Extension #

The handlersocketi extension allows you to access the functionality
provided by HandlerSocket plugin for MySQL.

More information about the HandlerSocket plugin for MySQL can be found at
[» http://github.com/ahiguti/HandlerSocket-Plugin-for-MySQL](http://github.com/ahiguti/HandlerSocket-Plugin-for-MySQL)

## PHP 8.2 Compatibility ##

This fork adds **PHP 8.2 compatibility** to the original HandlerSocketi extension.

### Changes Made ###
- Removed deprecated TSRMLS macros (removed in PHP 8.0)
- Fixed function signatures for PHP 8's new object model
- Updated exception handling for modern PHP
- Fixed clone function signatures
- Added conditional compilation for cross-version compatibility

### Building ###
```sh
git clone https://github.com/magma1447/php-ext-handlersocketi.git -b php-8.2
cd php-ext-handlersocketi
phpize
./configure
make
make install
```

### Docker Build ###
The repository includes the required `libhsclient-dev` dependency in `assets/` for reliable offline builds.

### Tested With ###
- PHP 8.2.29
- HandlerSocket protocol
- Real production workloads

**Original repository:** https://github.com/tony2001/php-ext-handlersocketi (badoo-7.0 branch)

