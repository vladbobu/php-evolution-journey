
# PHP 5 Examples

This directory contains examples showcasing significant features introduced in PHP 5. Each feature is explained along with example code.

## Key Features and Examples

### 1. Improved Object-Oriented Programming (OOP)
PHP 5 introduced a complete overhaul of object-oriented capabilities.
```php
class Person {
    private $name;
    public function __construct($name) {
        $this->name = $name;
    }
    public function getName() {
        return $this->name;
    }
}
```

### 2. PDO (PHP Data Objects)
A consistent interface for accessing databases.
```php
$pdo = new PDO('mysql:host=localhost;dbname=test', 'user', 'password');
```

### 3. Improved MySQL Support
MySQLi extension was introduced for enhanced MySQL integration.
```php
$mysqli = new mysqli("localhost", "user", "password", "database");
```

### 4. Iterators
For easier handling of various data types using a standardized interface.
```php
class MyIterator implements Iterator {
    // Iterator methods implementation
}
```

### 5. Exception Handling
Introduced traditional try-catch exception handling.
```php
try {
    // Code that may throw an exception
} catch (Exception $e) {
    echo $e->getMessage();
}
```

### 6. XML Support
Enhanced XML integration, including SimpleXML.
```php
$xml = simplexml_load_string($xmlString);
echo $xml->asXML();
```

### 7. SOAP Support
Native support for SOAP to build web services.
```php
$client = new SoapClient("some.wsdl");
```

### 8. Namespaces (Introduced in PHP 5.3)
Allowed for better organization of code.
```php
namespace MyProject;
class MyClass {}
```

### 9. Late Static Binding (Introduced in PHP 5.3)
Enhanced the way static methods and properties are handled in inheritance.
```php
class ParentClass {
    public static function who() {
        echo __CLASS__;
    }
    public static function test() {
        static::who(); // Here comes Late Static Binding
    }
}
```

### 10. Closures (Introduced in PHP 5.3)
Support for anonymous functions.
```php
$greet = function($name) {
    printf("Hello %s
", $name);
};
$greet('World');
```

## Explore and Learn
These examples are designed to help understand the advancements and capabilities introduced in PHP 5.
