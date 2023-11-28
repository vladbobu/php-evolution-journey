
# PHP 8 Examples

This directory contains examples showcasing the key features introduced in PHP 8. Each feature is explained along with example code.

## Features and Examples

### 1. Union Types
Allows more than one type for function parameters and return types.
```php
function foo(int|string $input): void {
    // function implementation
}
```

### 2. Named Arguments
Enables specifying argument names when calling functions.
```php
function foo(int $a, int $b, ?string $c): void {
    // function implementation
}
foo(b: 1, a: 2, c: null);
```

### 3. Match Expression
A new `match` expression, a more powerful switch statement.
```php
$result = match($input) {
    'apple' => 'This is an apple',
    'orange' => 'This is an orange',
};
echo $result;
```

### 4. Attributes
Attributes (annotations) add metadata to classes.
```php
#[Attribute]
class MyAttribute {
    // attribute implementation
}
```

### 5. Constructor Property Promotion
Simplifies declaring and assigning properties in constructors.
```php
class Point {
    public function __construct(
        public float $x = 0.0,
        public float $y = 0.0,
    ) {}
}
```

### 6. Nullsafe Operator
Safe calling of methods on nullable objects.
```php
$result = $obj?->method();
```

### 7. Weak Maps
Holds references to objects weakly.
```php
$map = new WeakMap();
$object = new stdClass;
$map[$object] = 'Data';
```

### 8. Just-In-Time (JIT) Compilation
Improves performance by compiling parts of the code at runtime.

### 9. Mixed Type
Indicates a function accepts/returns multiple types.
```php
function foo(mixed $input): mixed {
    // function implementation
}
```

### 10. New String Functions
New functions for common string operations.
```php
$str = "    PHP is fun!    ";
echo str_starts_with($str, ' PHP'); // false
echo str_ends_with($str, 'fun!    '); // true
echo str_contains($str, 'is'); // true
```

## Explore and Learn
These examples are designed to help understand the advancements and capabilities introduced in PHP 8.
