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

########################################### Comparisons
  Comparison type: '<, >, =, >=, <=, !=, ===, ==,'
  When we use 'if', condition was already boolean.
  for example:
  if (something) {
    ..
  }
  'something' - boolean.
## Boolean
true - yes(1) /correct
false - no(0) / wrong
We use comparing ofter for compare something to perform actions under a certain condition
Comparison operators return a boolean value.
Strings are compared letter-by-letter in the “dictionary” order.

## Interaction: alert, prompt, confirm
all this scripts paused script execution

alert

```
/// alert(message);
````

promt

Sshow a message and paused script until you press "OK"
 It returns the text or, if CANCEL or Esc is clicked, null.

```
/// result = prompt(title[, default]);
```
promt accepts two arguments, first will show message(before coma) and second will shows an input field.

confirm

```
/// result = confirm(question);
```
show message with two option "OK" and "CANCLE", just for boolean.


##   Conditional operators: if, '?'

# The “if” statement

The if statement evaluates a condition and, if the condition’s result is true, executes a block of code.

# Boolean conversion

The if (…) statement evaluates the expression in its parentheses and converts the result to a boolean.

# The “else” clause

The if statement may contain an optional “else” block. It executes when the condition is false.

## Several conditions: “else if”

We can do multiplicate time "else if" if its needed. Same as "else"


## Ternary operator ‘?’

same as "if, else" but with ternary operator its much simple and shorter.
 Example:
let result = condition ? value1 : value2;

 Example:

```
let age = prompt('age?', 18);

let message = (age < 3) ? 'Hi, baby!' :
  (age < 18) ? 'Hello!' :
  (age < 100) ? 'Greetings!' :
  'What an unusual age!';

alert( message );
```

with ternary operator "?" :

```
let age = prompt('age?', 18);

let message = (age < 3) ? 'Hi, baby!' :
  (age < 18) ? 'Hello!' :
  (age < 100) ? 'Greetings!' :
  'What an unusual age!';

alert( message );
```



######### Logical operators

 There are three logical operators in JavaScript: 
 1.   || (OR) -  used for test if any conditions is true.
 2.   && (AND)
 3.   ! (NOT)


# || (OR)
Getting the first truthy value from a list of variables or expressions.

# && (AND)
&& (AND) finds the first falsy value
The AND && operator does the following:
   Evaluates operands from left to right.
   For each operand, converts it to a boolean. If the result isfalse, stops and returns the original value of that operand.
   If all operands have been evaluated (i.e. all were truthy),returns the last operand.

# Precedence of AND && is higher than OR ||
So the code a && b || c && d is essentially the same as if the && expressions were in parentheses: (a && b) || (c && d).


`` Just like OR, the AND && operator can sometimes replace if.

```
let x = 1;

(x > 0) && alert( 'Greater than zero!' );
```
The action in the right part of && would execute only if the evaluation reaches it. That is, only if (x > 0) is true.

transform to standart:
```
let x = 1;

if (x > 0) {
  alert( 'Greater than zero!' );
}
```


### ! (NOT)

```
result = !value;
```
The operator accepts a single argument and does the following:

    Converts the operand to boolean type: true/false.
    Returns the inverse value.

A double NOT !! is sometimes used for converting a value to boolean type:
```
alert( !!"non-empty string" ); // true
alert( !!null ); // false
```
That is, the first NOT converts the value to boolean and returns the inverse, and the second NOT inverses it again. In the end, we have a plain value-to-boolean conversion.

The precedence of NOT ! is the highest of all logical operators, so it always executes first, before && or ||.
