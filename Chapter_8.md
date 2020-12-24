# Chapter 8
## What is Lambda calculus?

Lambda calculus is basicly the reduction of lambda terms using a set or operations in order to express computation based on function abstraction. Lambda terms are composed of three parts, variable, abstraction, and application. 

`λx.(λx.y x) (x y)`

In this example of a lambda term, x and y are both variables that reperesent a parameter or value. When they are paired with a lambda like λx., they become an abstraction and the variable becomes bound in the expression. An abstraction is just a function definition. An application is when two lambda terms are applied together like (x y) at the end.

Reduction operations come in two forms, α-conversion and β-reduction. α-conversion is for renaming variables in the expression in order to avoid naming conflicts. 

`(λx.M[x]) → (λy.M[y])`

β-reduction is the variables being replaced with the argument expression in the body of the abstract. This is done to progress the reduction towards termination and the finding of the normal form.

`((λx.M) E) → (M[x := E])`
