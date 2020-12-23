# Chapter 5 
## What is recursion?
Recursion is when a function contains a reference to itself and so can call itself. Doing so without planning could create an infinite loop of a function calling itself over and over. To prevent this the value of the recursive function call must be less then the recursive function that called it. An example being the fibonachi sequence to the n number. 

`fib 0 = 0`

`fib 1 = 1`

`fib n = fib (n-1) + fib (n-2)`

What this haskell code does is that it checks if the value of n is 0, in that case the output is 0. If the value of n is 1, then the output is 1. For all other cases of n, the output is the output of fib(n-1) added to the output of fib(n-2). A good way to visualise this is with a branching tree where n = 4.

                       fib(4)
                      /     \
               fib(3)    +    fib(2)
              /     \         /     \
        fib(2)  +  fib(1)   fib(1) + fib(0)
        /    \      
    fib(1) + fib(0)
    
Then once no more recursive calls can be made, the values of the fib(1)'s and fib(0)'s are added up and returned as the output for the fib(4).
