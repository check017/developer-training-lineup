# Code Tools

In the previous section we discussed the physical tools you will need to begin work on web developement projects.
Now, let's cover some programming concepts that you will need to be familiar with while working on a project.
These programming concepts are not specific to any single programming language.
They are ideas that are present in *any* language you work with.
The only thing that changes from one language to another is the actual syntax you need to implement the concept.
By understanding *concepts* rather than syntax, you will be well on your way to being able to implement your code
in any language you choose.

## Conceptual Understanding

It is very likely that you have seen news stories, articles,
or even YouTube videos telling you which programming language is the most "popular".  What does that mean, exactly?
Some of these sources have stated that by "popular" they mean the language most likely to get you a job. While this is very
desirable, there is an even better way to ensure longevity in this industry. It is the understanding of concepts, not syntax,
but concepts. An understanding of fundamental concepts goes further than any knowledge of syntax ever will.
There are not too many of these concepts. Whenever you are presented with a coding idea, make a point to look for the
underlying *concept* behind that piece of code. These ideas do not change much from one language to another.
The only real difference is emphasis. Some languages tend to emphasize one concept over another. However, the concept itself
didn't really change. Computers do not think. They have no capacity for even the most basic level rational thought.
Your household pet has more capacity for thinking than a computer will ever have.
That statement might offend some of the A.I. boys, but it is demonstratively true.
The computer only does what you tell it to
do, nothing more. You are the mind that gives the instructions.
The computer can't handle executing instructions the way a
human can. It does not understand inference. It cannot not assume anything.
It has no common knowledge. Because of this,
we have to be very clever in giving the computer
instructions that do not require any of these things.
By having a thorough understanding of concepts, our job is made much easier.

## Making Decisions

One of the simplest but most powerful tools you will use is the IF/ELSE statement.
With this statemment you can give the power of decision to the computer!. The idea is this:
"If this is the case, do this. If not, do something else." We can take this one step further by adding *else if*.
With this addition, there can be multiple cases you can check, and have a different set of instructions for each condition.
However, there are better ways to handle multiple conditions that need to be checked.
It is allowed to use a single IF statement without a ELSE statement. This is used to test
conditions to see if they are a certain value, but you don't necessarily want to do anything if they're not.

### Switch Statement

If you find yourself needing to check
multiple conditions (more than three), you might not want to write out a long chain of
IF/ELSE IF/ELSE statements.
Instead you can use a Switch Statement. This is used when multiple conditions are required to be checked.
In a Switch statement one value is tested against several different conditions (cases). If the value and the case match,
the code for that case is executed.
This might be used if you wished to check something other than just "*this* otherwise *that*."
Switch Statements are much more versatile, concise, and easier to read than an IF/ELSE statement.
The general rule of thumb is to use a IF/ELSE for evaluating one or two different conditions.
Use a Switch Statement for everything else. It looks like this:

```javascript
switch(expression) {
    case x: //Do something
    break;
    case y: //Do something
    break;
    case z: //Do something
    break;
    default: //If none of the above, do this
}
```

The expression can be anything you need to check. It could be a number or a string or a boolean. The expression is seen by
the computer as a *something*. If this something matches one of the cases in the list,
the computer executes the instructions written there.

### Ternary Operator

If you need to check only two different conditions, it is handy to use a Ternary Operator.
This keeps your code concise and thus easier to read.
If you have only two conditions to check, use the Ternary Operator. It looks like this:

```javascript
var age = 25;

var canDrive = age > 16 ? "yes" : "no";
```

The ternary operator has three parts (ternary means "composed of three parts").
First we have the expression in question `age > 16` . Then we have the yes/no decision.
The first part evaluates to "true" and the second part evaluates to "false".
This never changes, it is always expression, true, then false. This can get a little more sophisticated than just yes/no.
You can also put instructions in there. If the expression is true, do this. If it is false, do something else.
It would look like this:

```javascript
var age = 25;

var canDrive = age > 16 ? console.log('You can drive') : console.log('You cannot drive');
```

As you can see in the code block above, we are now executing a command (console.log)
based on whether the expression is true or false.

## The Loop

The idea is simple in itself. All it is is a way to tell the
computer to repeat a set of instructions over and over again.
The execution stops when you tell it to stop. There are a few ways to tell it to stop.
How you stop the loop gives the loop its own designation. Let's go over the types of loops very briefly here.

### The For Loop

This loop repeats a set of instructions a finite number of times. You specify how many. You can use a number,
such as 10 or 100, or you can use a length,
such as the length of an array.
Either way, you are saying, "Execute this set of instructions this many times."
The number of times the code will be executed is finite
(even if you don't know the number of times yourself, i.e. an array length)
This can be (and often is) combined with other concepts to execute a given task.
But just to keep it simple, the above concept is what a For Loop does. It looks like this:

```javascript
for(i = 0; i < 20; i++) {

console.log("Hello World!")
};
```

Let's break this down. "i" is our iterator. Iterate means to do something over and over again. An iterator is the thing that
does something over and over again. You will very often see the letter "i" used for this purpose. "i" stands for "iterator".
You can call the iterator anything you want, and some developers object to using "i" as it is not descriptive enough.
However, the use of "i" as the iterator is very, very common.

As you can see above, "i" is assigned the value 0. Then we see another expression, `i < 20;`. This means that the loop should
continue until the value of "i" is less than 20, but equal or greater than 20. The last statement is `i++`.
This means that after every run through the instructions of the loop the value of "i" should be increased by one.
In this case, the value "i" can only go to 19. If it were to equal 20, then it would not be less than 20.
Hence, "i" only goes up to 19. In the above example, the phrase "Hello World!" will be printed to the screen 19 times.

### The While Loop

There are situations wherein we do not know how many times we need the code to execute.
So, instead of giving a finite number we supply a condition.
A while loop says, "keep doing this until the condition of something is___".
What is the condition? It could be the value of a variable. It could be when an expression evaluates to true or false.
Note that the condition should eventually change until it evaluates to the condition you set. In other words,
if you stated that the loop should continue until `var a = 10;` then you have to account for how `var a` is going to eventually
get to 10. Otherwise, your loop will continue forever. It looks like this:

```javascript
let count = 20;
while(count > 0){
    console.log("Hello World");
    count--;
}
```

This is a little different than the For loop. We need to set a variable outside the code block to act as our condition.
Then the code executes. Included in the code block is the instruction to decrease the value of `count` with each pass.
When the value of `count` reaches 1, the loop is exited.

### Do While Loop

This loop is pretty similar to the While loop with one exception. The Do While loop will execute at least one loop.
It may not do a second or third loop, but it will do at least one. The condition is checked at the end of the loop,
not before (like in While or For loops). This means the code *must* run at least once. These are not seen very often.
They are used sometimes for displaying menus.
The loop displays the menu until a selection is made.
Selecting an item from the menu renders the test condition `false`,
and the loop is exited. It looks like this:

```javascript
let count = '';
let i = 0;
do {
    i = i + 1;
    count = count + i;
} while(i < 10);
console.log(count)
```

This loop would be used if you want the loop to execute at least one time.
Why would you want to do that? Well, lets say you ask for some input from the user.
If the data the user inputs does not match the `while` part of the loop, it will execute again.
It will continue to do this until the correct input is given.

### Common Uses of For Loops

For Loops are the most common type of loop you will encounter in your code. They are used to search for data, to sort data,
and to check for the presence of data.
For example, a test score is stored in an array of test scores.
You need one specific score. How would you find this?
Well, that score is special.
It has a specific quality that makes it unique.
That could be an index number, or a name, or a specific value.
This is the thing you are looking for. A For Loop is just the
thing to search through the array to locate the piece of data you need. How would that look, exactly?
Let's break it down into plain old English. Using our example above, let's say you need to find a specific test score.
We can find it by using its specific value. Or we can find it in a range of values.
If we were looking for, say, scores above 60 we could have our loop compare each index to see if it was less then 60.
If the index value was less than 60 then we ignore it.
If the index value is 60 or greater we could print that out or increment a variable.
One will give each score above 60, the other will tell us how many scores are above 60.
The important thing to take away from all of this is to ask yourself, "What am I trying to do here?"
If you can answer that, you can figure out the code to do it.
In the above example, we would use a For Loop. Inside of that For Loop we would have an IF/Else statement.
This is how you would search and select.
