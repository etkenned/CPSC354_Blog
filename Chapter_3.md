# Chapter 3
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
