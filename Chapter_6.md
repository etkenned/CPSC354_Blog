# Chapter 6
## How do I write functions in Haskell?
Now that you know the basic data types, you can start making your own functions. To declare a function you need a name, argument list, and output. 

`sub :: Integer -> Integer -> Integer`

In this example 'sub' is the name, followed by the argument list of two integers and then the output of an integer.
The definition of the function would be written directly below the declaration like this,

`sub x y = x - y`

where the x is representing the first integer argument, and the y is representing the second. The equal sign change the value of x or y but instead acts to set the output of the function to x - y.
To call the function you simply write the name of the function followed by the arguments of the correct data type in the main method.

`sub 5 3`

A common mistake I ran into with calling functions was with including parentheses incorrectly. With how Haskell interprets everything incased in parentheses as one argument, trying to call sub(5 3) would cause an error as sub is missing its second argument. 

All together the function would look like this.

`sub :: Integer -> Integer -> Integer`

`sub x y = x - y`


`print(sub 5 3)`

`2`

In order for us to see the result of our function we need to use the print() function to display the outcome '2' in the compiler.

[Return to Index](https://github.com/etkenned/CPSC354_Blog/blob/main/README.md)

[Next](https://github.com/etkenned/CPSC354_Blog/blob/main/Chapter_7.md)
