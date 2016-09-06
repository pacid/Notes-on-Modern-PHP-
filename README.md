# Notes-on-Modern-PHP-
Notes on Modern PHP 


Initially Personal Home Page Tool (a bunch of CGI scripts for Rasmus Lerdorf's website).

Andi Gutmans and Zeev Suraski joined Lerdorf and wanted to change the set of CGI tools into a programming language with basic OOP features. Named it PHP3 and published it at the end of 1998.

Writing a specification of PHP was announced by Sara Golemon in 2014. (http://bit.ly/php-langspec)

The official interpreter was introduced with pHP4, called Zend Engine and it's written in C by Lerdorf, Gutmans and Suraski.

Recently a new interpreter was created called HipHop Virtual Machine by Facebook. (HHVM)

Hack is a new programming language with:
- typed variables
- new data structures
- additional interfaces
- backward compatible

Namespaces in PHP since PHP 5.3.0

Namespace decalration:
-take one line
-be the first thing after the <?php mark
-first part is the name of the provider, then secondary namespaces
-separated with \
-they are not the the reflection of folder structure(but they can be). They are **virtual concept**.
-starts with keyword 'namespace', then a space and a name followed by a semicolon

```php
namespace Pawel;
```


```php
namespace Pawel\libs;
```

-all the classes, interfaces, functions and constants declared under namespace are connected to each other
-not all functions, classes etc have to be declared in one file
-importing namaspace - use Symfony\Component\HttpFoundation\Response;
-importing namaspace using alias  - use Symfony\Component\HttpFoundation\Response as Resp;
-php 5.6 added the ability to import functions or contants

```php
<?php
use func Somenamespace\nameOfFunction;

nameOfFunction();
```

```php
<?php
use constant Somenamespace\nameOfCONSTANT;

echo nameOfCONSTANT();
```

-possibility of not putting 'use' before every namespace declaration
```php
<?php
use  Somenamespace\nameOfSubNamespace1;
     Somenamespace\nameOfSubNamespace2;
     Somenamespace\nameOfSubNamespace3;

```

-possibility of adding several namespaces in one file (though, not receommended for clarity sake)

 


