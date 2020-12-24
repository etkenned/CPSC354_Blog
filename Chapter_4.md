# Chapter 4
## What is BNFC?
BNFC stands for Backus-Naur Form Converter, and it is a high-level front end to traditional implementation formats. Haskell uses BNFC to generate a compiler front-end from a Labelled BNF grammar. Basicly it compiles a compiler. In my experience before you install BNFC you need to make sure you have alex and happy installed. If you do not then you can download them if you have successfuly installed cabal by inputing these commands into your terminal.

`curl --proto '=https' --tlsv1.2 -sSf https://get-ghcup.haskell.org | sh`

`cabal install alex` 

`cabal install happy`

You can download and install BNFC from their site [here](http://bnfc.digitalgrammars.com/), or 

`$ cabal install BNFC`

or you can install like I did for Mac OS using homebrew.

`brew install bnfc`


## How do I use BNFC?
To get started with BNFC you need to download a context free grammar, I recomend Calc.cf to test if everything works.

`bnfc -m -haskell Calc.cf`

`make`

The 'make' command is what creates the parser TestCalc. To test if everything went well, try the following command.

`echo "2 + 4 * 6" | ./TestCalc`

The output should look something like this

`Parse Successful!`

`[Abstract Syntax]`

`EAdd (EInt 2) (EMul (EInt 4) (EInt 6))`

`[Linearized tree]`

`2 + 4 * 6`


[Return to Index](https://github.com/etkenned/CPSC354_Blog/blob/main/README.md)

[Next](https://github.com/etkenned/CPSC354_Blog/blob/main/Chapter_5.md)
