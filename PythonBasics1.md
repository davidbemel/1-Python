# Python basics WEBPAGE EXAMPLES
## Math Operators
### From Highest to Lowest precedence:
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

## String Concatenation and Replication
String concatenation:
```
print('Alice' 'Bob')
```
Note: Avoid + operator for string concatenation. Prefer string formatting.

## Comments
```
# This is a
# multiline comment
a = 1  # initialization
```
## Function Coment docstring:
```
def foo():
    """
    This is a function docstring
    You can also use:
    ''' Function Docstring '''
    """
 ```
## The print() Function
```
a = 1
print('Hello world!', a)
Hello world! 1
```
## The input() Function
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
```
Operator 	Meaning
== 	Equal to
!= 	Not equal to
< 	Less than
> 	Greater Than
<= 	Less than or Equal to
>= 	Greater than or Equal to
```
## Boolean evaluation
Never use == or != operator to evaluate boolean operation. Use the is or is not operators, or use implicit boolean evaluation.
NO (even if they are valid Python)
use in example: True is True // True is not False // a is not False

# Loops and If

## if Statements
```
if name == 'Alice':
    print('Hi, Alice.')
```
## if and else
```
name = 'Bob'
if name == 'Alice':
    print('Hi, Alice.')
else:
    print('Hello, stranger.')
```
## elif
```
name = 'Bob'
age = 5
if name == 'Alice':
    print('Hi, Alice.')
elif age < 12:
    print('You are not Alice, kiddo.')
```
## while Loop Statements
```
spam = 0
while spam < 5:
    print('Hello, world.')
    spam = spam + 1
```
## Break Statements
If the execution reaches a break statement, it immediately exits the while loop’s clause:
```
while True:
    print('Please type your name.')
    name = input()
    if name == 'your name':
        break
print('Thank you!')
```
## Continue Statements
When the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop.
```
while True:
    print('Who are you?')
    name = input()
    if name != 'Joe':
        continue
    print('Hello, Joe. What is the password? (It is a fish.)')
    password = input()
    if password == 'swordfish':
        break
print('Access granted.')
```
## for Loops and the range() Function
```
print('My name is')
for i in range(5):
    print('Jimmy Five Times ({})'.format(str(i)))
```
You can even use a negative number for the step argument to make the for loop count down instead of up.
```
for i in range(5, -1, -1):
print(i)
```
## For else statement
This allows to specify a statement to execute in case of the full loop has been executed. Only useful when a break condition can occur in the loop:
```
for i in [1, 2, 3, 4, 5]:
  if i == 3:
    break
 else:
  print("only executed when no item of the list is equal to 3")
```
