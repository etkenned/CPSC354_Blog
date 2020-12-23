# Chapter 2
## How do I get started?
Before I could actualy get started writing any code for Haskell, I first had to set up the enviroment. To do this you need to have your terminal ready and go to the Haskell home page [here](https://www.haskell.org/platform/#osx), and follow along with their instructions depending on your operating system. 

In my case I tried to installed Haskell for Mac OS, but had some prerequisite downloads I needed first. They were [homebrew](https://brew.sh/) and wget so that I could actually install the other components of Haskell. 

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Once brew is installed, install wget.

`$ brew install wget`

The second install I needed was [stack](https://docs.haskellstack.org/en/stable/README/), which is needed to install packages, build, and test the programs you write. Stack will also automaticly install ghc. 

`wget -qO- https://get.haskellstack.org/ | sh`

Lastly I installed [cabal](https://www.haskell.org/cabal/), which builds and packages the libraries. I did so by downloading the pre build binaries from [here](https://www.haskell.org/cabal/download.html), and using them to execute this in the command line.

`cabal-install`


If everything was installed correctly then you should be able to input the command

`stack exec ghci`

and start up the Haskell console.
