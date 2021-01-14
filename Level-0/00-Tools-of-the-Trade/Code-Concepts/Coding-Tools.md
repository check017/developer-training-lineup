# Code Tools

In the previous section we discussed the physical tools you will need to begin work on web developement projects.
Now, let's cover some programming concepts that you will need to be familiar with while working on a project.
These programming concepts are not specific to any single programming language.
They are ideas that are present in *any* language you work with.
The only thing that changes from one language to another is the actual syntax you need to implement the concept.
By understanding *concepts* rather than syntax, you will be well on your way to being able to implement your code
in any language you choose.

## A Note on Popularity

It is very likely that you have seen news stories, articles,
or even YouTube videos telling you which programming language is the most "popular".  What does that mean, exactly?
Some of these sources have stated that by "popular" they mean the language most likely to get you a job.
I'm afraid this is somewhat deceptive. A developer with a good grasp of programming concepts, and a knowledge of where and
when to apply them to a given programming problem, can learn the specific syntax of a language in the course of a weekend.
He already knows all the hard stuff, he's just learning a slightly different way to implement the concepts he already knows.
There are, of course, exceptions to this, but not many.
And don't forget, the applications already written
had to be written in a language that may have been the "most popular" only
a short while ago. That, of course, means that these applications are still using that "not so popular" language.
The code base of these applications
is not abandoned just because it was written in a language currently not in vogue. Rather than chase after trends,
it is better to gain an understanding of programming *concepts* instead of the current language fad.
These fads will be with us for the foreseeable future.
If you stick with concept, not language, you will be on solid ground regardless of trends or what is currently fashionable.

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
Use a Switch Statement for everything else.

### Ternary Operator

If you need to check only two different conditions, it is handy to use a Ternary Operator.
This keeps your code concise and thus easier to read.
If you have only two conditions to check, use the Ternary Operator.

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
But just to keep it simple, the above concept is what a For Loop does.

### The While Loop

There are situations wherein we do not know how many times we need the code to execute.
So, instead of giving a finite number we supply a condition.
A while loop says, "keep doing this until the condition of something is___".
What is the condition? It could be the value of a variable. It could be when an expression evaluates to true or false.
Note that condition should eventually change until it evaluates to condition you set. In other words,
if you stated that the loop should continue until var a = 10 then you have to account for how var a is going to eventually
get to 10. Otherwise, your loop will continue forever.

### Do While Loop

This loop is pretty similar to the While loop with one exception. The Do While loop will execute at least one loop.
It may not do a second or third loop, but it will do at least one. The condition is checked at the end of the loop,
not before (like in While or For loops). This means the code *must* run at least once. These are not seen very often.
They are used sometimes for displaying menus.
The loop displays the menu until a selection is made.
Selecting an item from the menu renders the test condition `false`,
and the loop is exited.

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
