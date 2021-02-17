# Programming Paradigms

A paradigm is a fancy word for "a way of doing something". It might seem obvious that the way to give instructions to a
computer is to do so one instruction at a time. The computer executes one instruction then moves down to the next instruction
and executes that one, and so on. This is certainly one way of doing it. However, it is not the only way of doing it.
There are many different "ways" to give the computer instructions. We will focus on the three most common paradigms.

## Procedural Programming

Procedural programming is a way of giving instructions that follow a list of steps. Each step is executed before moving onto
the next instruction in the list. It looks like this:

```javascript
1. Get the peanut butter
2. Get the jelly
3. Get the bread
4. Open the peanut butter jar.
5. Get a knife.
6. Apply peanut butter to bread
7. Apply jelly to bread
8. Combine both pieces of bread
```

There are likely a million different ways of making a peanut butter sandwich. Which instruction you give, and in what order you
give it in, is totally up to you. Nevertheless, the computer must execute the instructions one at a time in the order they
are written. This is procedural programming.

## Functional Programming

Rather than give one instruction at a time in order to get something done, you can group your code into small chunks.
Each chunk of code does *one* thing. You can think of these chunks as "micro-programs". They are separate from each other,
but work together to accomplish a task. The chunks are called `functions`. Functions are separate pieces of code that can be
used and reused as needed anywhere in your program. In procedural programming it is required that you write out each line of
code to be executed. If you have to perform the same action in multiple places in your program, you are required to write
 the lines to do this each time you need it to be done.
 This means you might have to write the exact same lines of code in different places. That makes for a very long program! By
 using functions, you can simply call (activate) the function you need whenever and wherever you need it. Not only does this
 make you code shorter, it also makes it easier to read. Here is an example:

 ```javascript
 const addIt(num1, num2){
     return num1 + num2;
 };

 addIt(3, 4);
 //expected output is 7
 ```

In the above example we have a function called `addIt`. `num1` and `num2` are called `parameters`. You can think of them as
place holders. The `parameters` are saying, "This function needs two numbers to do its thing." There can be all sorts of
different parameters for a function. Strings, arrays, and booleans can all be function parameters. These are the pieces of
data that are to be given to the function when the function called.

Notice that the code inside the function is surrounded by a set of curly braces, `{}`. This feature separates the function
from any other code in the program and making it a separate "chunk" of code. It can be called anywhere in your program multiple
times, if needed. You can have several separate functions in your program. Each one will do one thing when called.
This is basic idea of functional programming.

## Object Oriented Programming

Object Oriented Programming combines data with functions all wrapped in one container called an `object`. The idea is to more
closely simulate an actual object in real life. Any common object you see around you has two different qualities.
the first are its `properties`(things that describe the object,
such as its color or shape). The second is its function(things that it can do, such as roll or fly).
These two qualities are combined together to make an `object`. The `object` has data (properties) and functions
(called `methods`). There is quite a bit to know about `objects` and how they work. For now, all that is intended is to make
the student aware of their existence. You will see plenty more about objects in the near future.
Here is an example of a simple `object`:

```javascript
const myObject = {
    name : 'Tim',
    age : 23,
    getAge : function(){
        return this.age;
    }
}
```

Don't worry if that looks a bit confusing. We will cover this more extensively later. The above is just for the purpose of
showing the basic idea of `objects`.

## Uses of Programming Paradigms

Different languages utilize one or more of the above programming paradigms. Javascript is capable of using all of them.
Other languages are specific to only one paradigm. Java is an example of a programming language that uses Object Oriented
Programming almost exclusively. Ruby and PHP are both weighted toward Object Oriented Programming as well.
By contrast, the C language is largely a procedural language. It is important to understand that a paradigm is not an aspect of
a language, it is only a way to get things done.
