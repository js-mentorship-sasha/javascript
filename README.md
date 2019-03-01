# javascript

**The modern mode**, "use strict"
To keep old version of code working "use strict" in the top.

                                             Variables
  Variable is name of data storage. There is 2 type of variables, "let" and "const".
  let - variable that can be changet
  const - this variable cannot be changet.
   
                                           Variable naming
1. First litter must be not a number(digit).
2. Not reserved name(reserved by programming language).
3. The name must contain only letters, digits, or the symbols $ and _.
4. The name should give a description of this variable
        
                                             Data types
                                             
A variable in JS can contain any data.
There is a 7 different data types name:
1."number" - for number
2."boolean" - true/false
3."string" - for strings
4."symbol" - unique identifiers
5. "object" - complex data structure(
6."undefined" - variable without any date or data with undefined value
7."null" - unknown value

when we type let someVariable = null, we clear value of this variable. So null is value with nothing.


There is also 2 form of typeof without any difference "typeof x and typeof(x)"

                                   Type Conversions
                                   
We can convert value type. Also JS have functions that automatically convert.

                                    Operators


An operand – is what operators are applied to. For instance, in the multiplication of 5 * 2 there are two operands: the left operand is 5 and the right operand is 2. Sometimes, people call these “arguments” instead of “operands”.

An operator is unary if it has a single operand. For example, the unary negation - reverses the sign of a number.
An operator is binary if it has two operands. 

    Remainder %
 The result of a % b is the remainder of the integer division of a by b.

   Exponentiation **
 For a natural number b, the result of a ** b is a multiplied by itself b times.

  Increment/decrement
 Increment ++ increases a variable by 1
 a++ = a+1;

 Decrement -- decreases a variable by 1
 a-- = a-1;

!!! Increment/decrement can only be applied to variables. Trying to use it on a value like 5++ will give an error. !!!

   Bitwise operators
    AND - ( & )
    OR - ( | )
    XOR  - ( ^ )
    NOT = ( ~ )
    LEFT SHIFT - ( << )
    RIGHT SHIFT - ( >> )
    ZERO-FILL RIGHT SHIFT - ( >>> )

   Comma 
   (rare to use)
 The comma operator allows us to evaluate several expressions, dividing them with a comma ,. Each of them is evaluated but only the result of the last one is returned.

