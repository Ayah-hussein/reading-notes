# LOOPS:
there are two components to a decision:
- an expression is evaluated, which returns a value.
- a conditional statement says what to do in a given situation

if condition:
if the condition returns true executethe statments between the first set of curly brackets, otherwise execute the statment between the secod set of curly brackets.
example: 
if (average > 50) 
     {document.write('you passed');
} else
 {document.write('you fail')}

boolean operators:
 *  ==   is equal to
 *  !=   not equal to
 *  ===  strict equal
 *  !==  not strict equal
 *   >   greater than*  <   less than
  *  >=  greater than or equal to
 *   <=  less than or equal to


if else statment:Here you can see that anif ... e1se statement allows you to provide two sets of code:
1. one set if the condition evaluates to true
2. another set if the condition is false

### example:
var pass = 50;
var score = 75;
var msg;
if (score >= pass) {
msg = 'Congratulations, you passed!';
} else {
msg = 'Have another go!';
var el = document .getElementByld('answer');
el .textContent = msg;

## switch:
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and thecode that should run if the variable matches that value.

### example:
switch (level) {
case 'O ne ':
title= 'Level 1 ' ;
break;
case 'Two':
tit 1 e = ' Level 2 ' ;
break;
case ' Three' :
title = 'Level 3' ;
break ;
default :
title= 'Test';
break;}

## DATA TYPE PURPOSE
string >>>> Text
number >>>> Number
Boolean >>>> true or false
nul1 >>>>Empty value

 **Logical**  operators are processed left to right.
They short-circuit (stop) as soon as they have a result - but they return the value that stopped the processing (not necessarily true or fa1se).

**Logical operators** will not always return true or false, because:
• They return the value that stopped processing.
• That va lue might have beentreated as truthy or fa lsy although it was not a Boolean.



