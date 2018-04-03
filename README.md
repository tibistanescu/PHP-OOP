# PHP-OOP

## Classes and Objects
>A class is a **blueprint** or **template** used to build a specific type of object. 
#### Properties
>The characteristics of a class or object are called **properties** (also attributes or fields).
#### Methods
>Behaviours of a class or object are called **methods** (also actions).
#### Members
>The methods and properties of a class are called the members of the class.
#### Creating classes and objects

```php
// class declaration
class Car
{
    public $maker;
    public $color = 'black';

    public function getMaker() {
        return $this->maker;
    }

    public function getColor() {
        return $this->color;
    }
}

// class instantiation
$bmw = new Car();
$opel = new Car();

// accessing properties
$bmw->maker;
// calling methods
$bmw->getMaker();
```
## Visibility
- Public: Class members declared public can be accessed everywhere.
- Protected: Members declared protected can be accessed only within the class itself and by inheriting and parent classes. 
- Public: Members declared as private may only be accessed by the class that defines the member.

Properties must have visibility declared, methods that don't have visibility declared are public by default.

## Class Constants
``
