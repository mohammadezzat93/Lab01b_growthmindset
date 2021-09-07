# Functional Programming Concepts

## What is functional programming?
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

## What is a pure function and how do we know if something is a pure function?
- ** pure function is a computational analogue of a mathematical function.**
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects
- It returns the same result if given the same arguments

## What are the benefits of a pure function?
- The code’s definitely easier to test.
- We don’t need to mock anything. So we can unit test pure functions with different contexts:  
-Given a parameter A → expect the function to return value B  
-Given a parameter C → expect the function to return value D

## What is immutability?
- Unchanging over time or unable to be changed.
- When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

## What is Referential transparency?
- Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

- **pure functions + immutable data = referential transparency**  
- With this concept, a cool thing we can do is to memoize the function. 

# Node JS Tutorial for Beginners 6 - Modules and require()

## What is a module?
- JS modules (also known as “ES modules” or “ECMAScript modules”) are a major new feature, or rather a collection of new features  All of these module systems have one thing in common: they allow you to import and export stuff.
- Modules are a way to split an application into separate files instead of having all of your application in one file. 

## What does the word ‘require’ do?
- require() is not part of the standard JavaScript API. But in Node.js, it's a built-in function with a special purpose: to load modules.

## How do we bring another module into the file the we are working in?
- By using the class and then invoking it through the import

## What do we have to do to make a module available?
- Top level await is a feature available within modules. This means the await keyword can be used. It allows modules to act as big asynchronous functions meaning code can be evaluated before use in parent modules, but without blocking sibling modules from loading.