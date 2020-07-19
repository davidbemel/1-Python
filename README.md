# Python basics
## Math Operators
From Highest to Lowest precedence:
```
** 	Exponent 	2 ** 3 = 8
% 	Modulus/Remaider 	22 % 8 = 6
// 	Integer division 	22 // 8 = 2
/ 	Division 	22 / 8 = 2.75
* 	Multiplication 	3 * 3 = 9
- 	Subtraction 	5 - 2 = 3
+ 	Addition 	2 + 2 = 4
```
## Data Types

Data Type 	Examples
Integers 	-2, -1, 0, 1, 2, 3, 4, 5
Floating-point numbers 	-1.25, -1.0, --0.5, 0.0, 0.5, 1.0, 1.25
Strings 	'a', 'aa', 'aaa', 'Hello!', '11 cats'

# String Concatenation and Replication

String concatenation:
´´´
print('Alice' 'Bob')
```
< Note: Avoid + operator for string concatenation. Prefer string formatting.

# Comments

```
# This is a
# multiline comment
a = 1  # initialization

Function docstring:
```
def foo():
    """
    This is a function docstring
    You can also use:
    ''' Function Docstring '''
    """
 ```
## The print() Function

>>> print('Hello world!')
Hello world!

```
a = 1
print('Hello world!', a)
Hello world! 1
```
## The input() Function

Example Code:
```
print('What is your name?')   # ask for their name
myName = input()
print('It is good to meet you, {}'.format(myName))
```

## Functions len(),The str(), int(), and float() Functions
```
len('hello')
a = [1, 2, 3]
if a:
print("the list is not empty!")
str(29)
print('I am {} years old.'.format(str(29)))
int(7.7)
int(7.7) + 1
```
## Comparison Operators
Operator 	Meaning
== 	Equal to
!= 	Not equal to
< 	Less than
> 	Greater Than
<= 	Less than or Equal to
>= 	Greater than or Equal to

These operators evaluate to True or False depending on the values you give them.

Examples:
```
print(42 == 42)

## Boolean evaluation
Never use == or != operator to evaluate boolean operation. Use the is or is not operators, or use implicit boolean evaluation.
NO (even if they are valid Python)

# if Statements
