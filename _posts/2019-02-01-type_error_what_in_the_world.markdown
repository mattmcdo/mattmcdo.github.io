---
layout: post
title:      "Type Error?! What in the World?"
date:       2019-02-02 02:13:13 +0000
permalink:  type_error_what_in_the_world
---

In my effort to re learn coding and restart the Flatiron Curriculum, I recently refreshed myself on the value of an error message and how to dissect what it meant.

When I went through the beginning sections of this program initially, I found myself really guessing at what was wrong with my code instead of stopping and trying to really dissect what the error was telling me. I panicked! So many lines of random words that I had *no* clue how to interpret! 

Boy was I wrong, Ruby was really just trying to point me in the right direction!

First and foremost, i was reminded of how to read errors messages. There are essentially 3 parts:

The who (or what, in my opinion) -- what type of error

The where -- what line of code

The why -- why is the code breaking/have an issue?

By breaking apart the error in those 3 pieces, it starts to make much more sense.

Additionally, I reaquainted of 4 main types of errors:

1. Name Error
2. Type Error
3. Syntax Error
4. Zero Division Error

Let's break them down.

1.) Name Error 

This error occurs when Ruby comes across a word that may not have been defined.

For example, if I were to have in my code 

puts apple

Ruby would come up with a Name Error because I have not defined what apple is; the word apple isn't a Ruby Keyword so it assumes it is a variable (which needs to be defined with an = sign) or method.

2.) Type Error

The type error is the next error I came across. This error comes along if you are trying to combine or work with two different types of data (EX: Strings and Integers) that don't play together. Example, adding an integer and a string together, 1 + "1", will spit out a type error.

Also another example I've seen: [1, 2, 3].first("two") -- gives you a type error (TypeError: no implicit conversion of String into Integer). 

When I played around with the WHY in IRB, it is because ".first" is really counting/picking out out the first two INTEGERS/indexes in the array.

[1,2,3].first(2) --> gives me [1,2] as a return value


3.) Syntax Error

This error is pretty self explanatory, this comes about the result of incorrect syntax, or nonsensical code.

3_ + 5 
*
Gives me a Syntax error, it has no idea why I added "" in my equation. That's a pretty contrived example but gets my point across. This is bad code.

4.) Zero Division Error

Here's the most simple one.. you can't divide by zero! Simple math 101 right there!

5013589 / 0 gives you a Zero Division Error. Pretty self explanatory!

That's all for now. Until next time!

Matt
