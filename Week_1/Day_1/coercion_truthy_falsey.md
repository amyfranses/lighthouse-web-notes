# Coercion

**Type Coercion** 
- Refers to the process of automatic or **implicit conversion of values from one data type to another**. 
  
  -   Including conversion from Number to String, 
  -   String to Number, 
  -   Boolean to Number etc. 
  
  **when different types of operators are applied to the values.**

  Two ways to compare values in JS 
  
  - ==
  eg 23 == "23" is true because == will attempt to force the two values to be of the same type, if possible
  - === compares **values** and **type of value**
  eg 23 === "23" is false because one is a string and the other a number

  - Comparing two values in JavaScript will return either true or false.  
     
     - when using ==, that the correct response will be the opposite of what you might expect

     eg 0 == false

     ## falsey values

     - **False** - False is False. Makes sense, right?
     - **0** - 0 is the only falsey Number
     - **""** - an empty string is falsey
     - **null** - a null, or empty value, is falsey.
     - **undefined** - an object that has not been defined is considered falsey.
     - **NaN** - Not a Number. You'll learn more about NaN as we go on.