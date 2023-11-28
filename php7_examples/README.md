
# PHP 7 Examples

This directory contains examples showcasing the top features introduced in PHP 7. Each feature is explained along with example code.

## Features and Examples

### 1. Scalar Type Declarations
Allows the function to enforce the type of values it receives.
```php
function addNumbers(int $a, int $b) {
    return $a + $b;
}
```

### 2. Return Type Declarations
Enables specifying return types for functions.
```php
function getSum(int $a, int $b): int {
    return $a + $b;
}
```

### 3. Null Coalescing Operator
Used for returning the first non-null value.
```php
$username = $_GET['user'] ?? 'nobody';
```

### 4. Spaceship Operator
A three-way comparison operator that returns -1, 0, or 1.
```php
echo 1 <=> 2; // returns -1
```

### 5. Constant Arrays
Support for defining arrays as constants.
```php
define('FRUITS', [
    'apple',
    'banana',
    'orange',
]);
```

### 6. Anonymous Classes
Support for single-use, on-the-fly classes.
```php
$newClass = new class {
    public function sayHello() {
        echo 'Hello';
    }
};
```

### 7. Group Use Declarations
Allows grouping similar 'use' declarations into a single line.
```php
use MyProject\{ClassA, ClassB, ClassC as C};
```

### 8. Generator Return Expressions
Enhancements to generators to return expressions.
```php
$gen = (function() {
    yield 1;
    yield 2;
    return 3;
})();
```

### 9. Throwable Interface
A new base interface for error handling.
```php
try {
    throw new Exception("Error Processing Request", 1);
} catch (Throwable $e) {
    echo $e->getMessage();
}
```

### 10. CSPRNG Functions
Functions for cryptographically secure random number generation.
```php
$bytes = random_bytes(10);
$int = random_int(100, 999);
```

## Explore and Learn
These examples are designed to help understand the advancements and capabilities introduced in PHP 7.
