[![Coverage Status](https://coveralls.io/repos/github/qtn3/IS219Calculation-OOP/badge.svg?branch=master)](https://coveralls.io/github/qtn3/IS219Calculation-OOP?branch=master)
[![Build Status](https://travis-ci.org/qtn3/IS219Calculation-OOP.svg?branch=master)](https://travis-ci.org/qtn3/IS219Calculation-OOP)

Principles of Object Oriented Programming
1. Abstraction
function Square (a, b) {
    return Math.pow(a, b);
}
module.exports = Square;

static Create(a, b, op){
        return new Calculation(a, b, op);
    }

2. Encapsulation:
The process of wrapping property and function within a single unit is known as encapsulation. 
For example, we can see the Calculation class in the Calculation file. In the Calculation class, we have constructor
which we can change the variables 

3. Inheritance
The concept in which some property and methods of an Object is being used by another Object.
Javascript is difference than the most of OOP languages where classes inherit classes, but JavaScript
Object inherits Object, so that certain features (property and methods) of one object can be reused 
by other Objects.

4. Polymorphism

SOLID Principles
1. S- Single Responsibility Principle
For example in the Calculation.js file, we have Create(a, b, op) method which is repsonsible for creating of the operation

static Create(a, b, op){
        return new Calculation(a, b, op);
    }

2. O- Open-Closed Principle
For example, the Quotient operation should handle exception such as dividing by zero (mormally, it will thrown an error).

function Quotient (a,b) {
    var quotient = a / b;
    if(quotient !== quotient){
        throw new Error(a + " / " + b);
    }
    return quotient;
}
module.exports = Quotient;

3. L- Liskov Substitution Principle

4. I- Interface Segregation Principle

5. D- Dependency Inversion Principle

