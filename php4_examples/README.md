
# PHP 4 Examples

This directory contains examples showcasing significant features introduced in PHP 4. Each feature is explained along with example code.

## Key Features and Examples

### 1. Introduction of Zend Engine
PHP 4 was powered by the Zend Engine, providing improved performance and a foundation for future PHP development.
```php
// Example: Basic PHP script demonstrating improved performance
echo "Hello, World!";
```

### 2. Improved Object-Oriented Programming
PHP 4 made strides in object-oriented programming, although it was less comprehensive than in PHP 5.
```php
class Person {
    var $name;
    function setName($newName) { 
        $this->name = $newName; 
    }
    function getName() {
        return $this->name;
    }
}
```

### 3. Sessions
PHP 4 introduced native support for sessions, making user tracking and data persistence easier.
```php
session_start();
$_SESSION['user'] = 'John Doe';
```

### 4. Output Buffering
Output control functions were introduced, allowing for buffering of output.
```php
ob_start();
echo "Hello, World!";
$output = ob_get_clean();
```

### 5. More Predefined Super Globals
Introduction of several superglobals like `$_SESSION`, `$_COOKIE`, etc.
```php
echo $_COOKIE['user'];
```

### 6. Improved Support for a Variety of Databases
PHP 4 enhanced its database connectivity, supporting a wide range of databases.
```php
mysql_connect('localhost', 'username', 'password');
mysql_select_db('database');
```

### 7. Enhanced Security Features
PHP 4 introduced several security enhancements, including improved session handling.
```php
// Example: Secure session handling mechanisms
session_start();
// Security code goes here
```

## Explore and Learn
These examples are designed to help understand the advancements and capabilities introduced in PHP 4.
