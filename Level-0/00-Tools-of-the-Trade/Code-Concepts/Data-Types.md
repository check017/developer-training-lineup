# Primitive Data Types

The computer does not distinguish between letters, numbers, and sentences. To the computer these all just symbols.
Nothing that you type into the computer means anything at all to it.
After all, the only language the computer
speaks is binary (1's and 0's). We as developers have to tell the computer what these symbols mean. In order to do this
efficiently, programmers have divided the symbols on
your keyboard into *types*.  A data type tells the
computer what kind of
data it is dealing with. If you were to write out a grocery list by placing a number before each item, you don't mean that
your grocery list will be using those numbers for some sort of calculation. You just need a list of separate items.
The computer does not know the difference. While the number used for itemizing a list and calculating a value is the
same symbol, the way it is intended to be used determines its type. Let's go over the basic types here:

## Integers

A whole number that is not a fraction is called an integer. Any number that does not have a decimal point after it is
considered an integer. The computer understands that this is
intended to represent a value of something (how much or how little). The numbers 3 or 5 or 239842 are integers.

## Float

A Float is a number that contains a fraction. 3.141592 is a Float. It is called a "float" because the decimal point is allowed
to "float" (move around) as needed to represent a fractional number. The computer is required to handle floats differently
from integers as they require more memory storage. Floats represent fractional values to the computer.
Javascript does not distinguish between integer and float data types. Either type can be assigned as a value without noting
which is which. This is not true in some other languages (Like Java or C++).

## BigInt

BigInt is a number data type.
It allows for calculating very large numbers that
exceed the memory capacity for an Integer or
Float type. You will see it used in public encyption keys where very large numbers are required.

## Boolean

The Boolean type is used for determining whether something is true or false. A Boolean value will always evaluate to either
true or false. This is used in a variety of different ways, but mostly you will see it when comparing two values or expressions
to determine if they are equal.
It is helpful to think in terms of true or false when writng If/Else statements or for certain callback functions.
There is quite a bit more to this, but we will cover those details in later sections.

## Char

A Char data type represents a single character. Javascript does not have this as a data type.
All characters are represented in Javascript as string data types.
In other languages Char represents a single character or
its ASCII number code. If the char is in quotes, it is interpreted as the character itself.
If the character is not in quotes, it is represented by its ASCII code integer.
For example, if we were to say `char letter = x` the value stored in memory would be 120, not the character 'x'.
This is because the ASCII code for 'x' is 120. Conversely, if we were to say `char letter = 'x' the value stored in memory
still be 120, but would be interpreted as the letter 'x'. While this is not an issue in Javascript,
several other languages do use the Char data type.

## String

A String is any set of characters written between quotation marks. A string can be a single character, or it can be a whole
sentence. In Javascript a string can be assigned to a variable without any further distinction. All that is required is the
use of regular assignment syntax like this `var myString = 'This is a string'`. The String type is very common in code.
Strings can be chained together through a technique called concatenation. This is a fancy word for "chained together".
This is done by using the '+' operator.
Here is an example of this: `console.log('This is a ' + ' sentence chained together')`.
This will output to the monitor `This is a sentence chained together`.
Note that there is a space added at the end of the first segment.
This is needed to maintain proper spacing when the two segments are connected.
It is mentioned here because forgetting the space is a common error.

## Undefined

Undefined means that a variable has been declared, but has not been defined.
In other words, the computer knows soemthing is there,is OK with it, but it does not know what its value is.
Undefined is not necessarily an error. Developers can use Undefined to determine if a value is present or not.
Sometimes you will find your code snippet is correct in its syntax, but flawed in its logic. When this is the case,
you will often see undefined printed to the monitor, but no error message is thrown. It means your syntax is great,
but your logic might need some tweaking.

## Null

Null means that there is no value there on purpose. It's just a big, fat nothing. It does not mean 0 or undefined.
0 is an integer. It is a *something*.
Undefined is also a *something*. Null is a *nothing*, the total absence of data. Null can be used to determine whether a
*something* is extant. If it is not, it is said to be Null.
Bear in mind that in the case of undefined there is at least a declared variable. This counts as a *something*, and is
therefore not Null. 0 is a value. Even though it evaluates to nothing, it still has a value, i.e. no value.
It is not Null as there is a value that equates to nothing.
Null would be absolutely nothing there at all, no variable, no value of any kind.
