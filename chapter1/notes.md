# Section 1.2

The workflow of type-driven development:
type, define, refine.

## Exercise answers

1. map: map (* 2) [1,2,3] => [2,4,6]

2. duplicate: duplicate [1,2,3] => [1,2,3,1,2,3]

3. pop: pop [1,2,3] => [1,2]

4. get: get 1 [1,2,3] => 2

# Section 1.3

When we say a programming language is *functional*, it means:

* Programs are composed of functions.

* Program execution consists of the evaluation of functions.

* Functions are a first-class language construct.

In a *pure* functional language, the following are also true:

* Functions don’t have side effects such as modifying global variables,
  throwing exceptions, or performing console input or output.

* As a result, for any specific inputs, a function will always give the same result.

In pure functional programming in general, and Idris in particular,
you can solve this problem by writing functions and *describe* side effects,
rather than functions that *execute* them, and defer the details of execution
to the compiler and runtime system.

A *total* function is guaranteed to produce a result,
meaning that it will return a value in a finite time for every possible
well-defined input, and it's guaranteed not to throw any exceptions.

A *partial* functions, on the other hand, might not return a result 
for some inputs.

A total function is guaranteed to produce a *finite prefix* of a potentially
infinite result.

# Section 1.4

The prompt of Idris REPL is the *file* name, instead of the *module* name
in Haskell ghci.
