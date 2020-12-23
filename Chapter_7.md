# Chapter 7
## How do I code in Haskell?

To begin writing code in Haskell you need to first open the GHCI compiler by inputing the command,

`ghci`

into your terminal. Once that is up and running you can begin passing code into it as it will function like the Try it! feature [here](https://www.haskell.org/). While Haskell is a staticly typed language, for most numbers the compiler should be able to figure out what type they should be so you do not need to label them yourself. If you were to input a simple math function like,

`1 + 2`

`3:: Num a => a`

into the compiler then it would output the answer '3'. This works for all the basic functions of PEMDAS: (), ^, *, /, +, -.

For characters and strings, Haskell handels them in a similar way where as long as they are surrounded in qutation marks then the compiler will interpret them as a char,

`"a"`

`"a":: [Char]`

or a string,

`"abc"`

`"abc":: [Char]`

Haskell will also interpret ASCII code into chars,

`'\97'`

`"a":: [Char]`

Booleans are also interpreted pretty well by the compiler along with boolean functions like,

`True || False`

`True:: Bool`

and

`True && False`

`False:: Bool`

Lists can be created in Haskell and are traditionaly homogeneous so they must contain only one data type of variable. You can create lists by just surrounding the contents with square brackets.

`[1,2,3,4]`

Each list is made up of a head and a tail and you can access them both seporatly by using the head() and tail() functions.

`head([1,2,3,4])`

`1:: Num a => a`

`tail([1,2,3,4])`

`[2,3,4]:: Num a => [a]`

