# Chapter 9
## What is an ARS?
An ARS or Abstract Reduction System, is a set of objects that have a binary relation. You would use these binary relations as a set of rules to rewrite/reduce the objects into their normal forms. These binary realtionships are usualy denoted with → such as,

`a → b`

`b → c`

`cc → ''`

What these rules state is that for any set that contains 'a', then all 'a's will reduce to 'b's. All 'b's will be reduce to 'c's, and all 'cc's will be reduced to the empty word. An empty word is just an object with no value. The order that the compiler acts apon these rules does not matter and can happen in any way. This set of rules terminating, meaning that the compiler will eventually reach a point where it cannot apply any more rules to the set of objects and the normal form will be found. The termination of these rules can be proven using invariants and a measure function. Invariants are functions that are unaffeted by the rules and help to prove what is impossible. There for you would use invariants to prove the existane of a unique normal form for the set to reduce to. With no normal form the set would never terminate and be stuck in an infinite loop. A measure function uses the invariants youve created to demonstrate that ARS does terminate. An example of a set being reduced by these rules would be as follows,

`acabcbb`

`bcabcbb`

`ccabcbb`

`ccbbcbb`

`cccbcbb`

`cccccbb`

`ccccccb`

`ccccccc`

`ccccc`

`ccc`

`c`

With 'c' being the normal form. We can know that 'c' is a unique normal form using the invariant,

`(#a + #b + #c) % 2`

This invariant would be able to determine the unique normal form for any of the sets, either the total number of a's, b's, and c's is even and the normal form is the empty word, or the total is odd and the normal form is 'c'. 

[Return to Index](https://github.com/etkenned/CPSC354_Blog/blob/main/README.md)
