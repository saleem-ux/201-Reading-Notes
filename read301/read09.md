## Things I want to know more about

## What is functional programming?
Functional programming is a programming model, "a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data" (quote from article)

## What is a pure function and how do we know if something is a pure function?
Something is a pure function if, when given the same arguments, always returns the same result. It also does not cause any "observable side effects." AKA - if all the variables and values used in the function are given as parameters, it is a pure function

## What are the benefits of a pure function?
The benefits of a pure function is that if the global variables ever used are changed, the value accurately scales with the edit

## What is immutability?
This means that it's state cannot be changed after creation

## What is Referential transparency?
pure functions + immutable data = referential transparency NodeJS:

Split code up into logical modules Can call modules whenever needed Bare minimum added in each module To run a specific file through node in the console you can type node file_name.extension or node file_name To bring one file into another using node is by typing require './file_name.extension' at the top of the file where needed To bring in one file, you must say module.exports = function_name or module.exports = class_name at the bottom of the file the data is sent out from

## What is a module?
one part (or file) with a specific functionality to achieve a part of a larger goal (many files / functions / classes)

## What does the word ‘require’ do?
imports data from another file

## How do we bring another module into the file the we are working in?
require './file_name.extension'

## What do we have to do to make a module available?
module.exports = function_name