
# Chapter 02: Dart Programming Language 
## 1. What's the object in Dart?
Answer: Everything you can place in a variable is an object, and every object is an instance of a class. Even numbers, functions, and null are objects. 

## 2. How the types are inferred in Dart?
Answer: Although Dart is strongly typed, type annotations are optional because Dart can infer types. For instance, 42 is inferred to be of type int. When you want to explicitly say that no type is expected, use the special type dynamic.

## 3. What are the generic types?
Answer: Dart supports generic types, like List\<int> (a list of integers) or List\<dynamic> (a list of objects of any type).

## 4. What kinds of functions are in Dart?
Answer: Dart supports top-level functions (such as main()), as well as functions tied to a class or object (static and instance methods, respectively). You can also create functions within functions (nested or local functions).

## 5. What kinds of variables are in Dart?
Answer: Dart supports top-level variables, as well as variables tied to a class or object (static and instance variables). Instance variables are sometimes known as fields or properties.

## 6. Does Dart have the keywords public, protected, and private?
Answer: Unlike Java, Dart doesn’t have the keywords public, protected, and private. If an identifier starts with an underscore (_), it’s private to its library. 

## 7. What are the expressions and statements?
Answer: Dart has both expressions (which have runtime values) and statements (which don’t). For example, the conditional expression condition ? expr1 : expr2 has a value of expr1 or expr2. Compare that to an if-else statement, which has no value. 

## 8. What are the warnings and errors showed in Dart tools?
Answer: Dart tools can report two kinds of problems: warnings and errors. Warnings are just indications that your code might not work, but they don’t prevent your program from executing. Errors can be either compile-time or run-time. A compile-time error prevents the code from executing at all; a run-time error results in an exception being raised while the code executes. 
