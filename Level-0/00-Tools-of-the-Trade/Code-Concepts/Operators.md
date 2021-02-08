# Operators

Operators are symbols used to compare values or perform mathematical operations. Most of these are pretty familiar.
However, there are a few that are unique to computer languages.
In this section we will briefly go over the most common operators found in almost every computer language.

## Addition

This operator is one you are likely very familiar with. It looks like this: `+`.
It is used to add values together like this: `3 + 4 = 7`.
However, that is not all it can do. When using the `+` operator on strings it will combine them together.
It looks like this: `var chainedString = 'This is a ' + 'string';`.
When we print the value of `chainedString` to the console, we get this: `This is a string`.

The addition operator can be used to combine just about anything.
If the operands are values, like an integer or a variable that evaluates to a number,
the addition operator will add them together. However, if one or more of the operands is not a value, like a string,
the addition operator will combine the operands together. Here is an example of this:

```javascript
let foo = 23;
let string = 'Tom is ' + foo + ' years old.';
console.log(string);
```

The code block above will return `Tom is 23 years old.`.
The action of chaining together different variables is called concatenation.
This is a fancy word that means "chaining things together".
When you need to do addition or link things together, you can use the addition operator.

## Increment Operator

Many times while you are writing your code you will find you need to increase the value of a variable by one.
This is so common, in fact, that there is a specific operator to do just this one thing. It is called the increment operator.
It looks like this: `++`. It is placed after the variable or value you wish to increment. It looks like this:

```javascript
let foo = 2;
foo++;
console.log(foo);
```

The output of this block of code will be 3.
You see this operator used in For loops to increase the value of the counter after every pass through the looped code.
The increment operator is also used whenever you need to count something. All it does is increase the value by 1.

## Decrement Operator

The decrement operator looks like this: `--`. As you may have guessed already,
the decrement operator does the exact opposite of the increment operator.
It will decrease the value by 1. It is used whenever you need to count down from a set value towards 0.

## Subtraction

This is the subtraction operator. You may know it as a minus sign.
It's the same thing. It is used to subtract a value from a value. It looks like this: `10 - 5 = 5`.
You can't subtract anything that is not a value. So, you can't subtract a string from a string.

## Multiplication

The multiplication operator looks like this `*`. You may have seen the same thing that looks like this `x`.
This symbol is not used by the computer for multiplication. Instead we use the `*` for multiplying numbers.
Computers don't really perform mulitiplication. They don't memorize multiplication tables like you did when you were a kid.
Multiplication is really just adding a number to itself a given number of times. The expression 8 * 4 is simply
saying 8 + 8 + 8 + 8. Your computer can add stuff way, way, way faster than you can. So, when you tell it multiply, it adds
the number to itself the number of times you say. It does this really, really fast. Whenever you need to multiply
numbers use the `*` operator.

## Division

The division operator looks like this `/`. It divides the operand on the left by the operand on the right.
It looks like this: `10 / 2 = 5`. All it does is divide values.

## Modulus

The modulus operator returns to remainder of a number divided by a number. It looks like this: `10 % 6 = 4`. You can use the
modulus operator to determine if a number is even or odd. It looks like this:

```javascript
let foo = 124 % 2;
console.log(foo);
```

If the console shows a 0 (in the above example, it will) then you know the number was evenly divided because there is no
remainder. You can also use it to determine if a number is divisible by another number. If 0 is returned by the modulus
operation, you know that the first
number is divisible by the second number. This can be useful when you need to determine the multiples of a given number. 