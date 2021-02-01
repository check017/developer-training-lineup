# Data Structures

A computer system exists primarily to mainpulate data. A computer system does not have an infinite amount of memory resources,
nor does possess instantaneous transport of data. Because of these facts, it is necessary to handle data being used in a
computer system in the most efficient way possible. By organizing our data and intelligently accessing that organization,
we can maximize the performance of the system. One of the tools utilized
to achieve this is the data structure. If we were to have a series of related values (like a number)
that have some relationship to each other (like test scores or ID numbers) it makes sense that we would group them
together in one place.
This is one use of a data structure. It is not inconceivable that a computer could store related data anywhere it wanted.
It is perfectly capable of retrieving that data even though it may be scattered all over the place. However, that takes time
and multiple calculations. These are not necessary if the data is grouped in a data structure. When so grouped the
computational and memory resources are protected from being over extended, and the system is capable of doing
more than it could when not so organized. An understanding of Data Structures is essential to good software development.

## Terms

Before we get started, let's define some terms.

* `Data Structure`

    - A particular way of organizing data so that it can be used effectively.

* `Structured Data Type`

    - A data type that is comprised of several
    data items each one being a collection of other data items all using a single identifier.
    Oh, you want that in *English*?
    Ok, a structured type is a something that
    is made up of a bunch of other, smaller somethings
    arranged in a particular way.
    An Array is an example of a Structured Data Type.

The two definitions given above seem very similar. That's because they largely are the same thing. However,
some make a distinction between the two.
Data Structures can include a wide variety of different methods of organizing data. A Structured Data Type refers to a more
specific entity used to organize data. It's kind of like distinguishing between a cat and a Orange Tabby cat.
One is a more specific description of a general type of animal.
Anything that puts pieces of data together in such a way that
relationships can be inferred or defined is a data structure.
Exactly *how* it organizes the data would be the structured data type.

## Arrays

Arrays are data structures that hold values in a specific order.
Each value is assigned an integer in sequential order starting at 0.
Here is an example: `let array = [3,5,2,8];` . Each of these values is assigned an identifier starting with 0.
Think of them as boxes. The boxes have names. Inside the boxes is the value.
So, the box named 0 would contain the value 3, the box named 1 would contain the value 5, and so on.
The name of the box that stores a value is called an `index`. If you want to get the value out of the box,
you have to use its name (index). It looks like this: `console.log(array[0]);` . This will print the number 3.
The entire array has a name as well. In the case, it is called 'array'.
When you name your array, try to be a little more specific in the naming. This name is just for demonstration purposes.
In Javascript you can put anything you want in an array. You can even put other arrays into an array.
You can have different data types in the same array.
Arrays are used when you want to store a group of values together under one name, in order, with a numerical index.
