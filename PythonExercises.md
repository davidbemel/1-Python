# This is a resume for Basic Python tutorial with mosh
```
a = 10
b = 5
print(a*b-2**b>20 and not (a % b)!=0)
print(type(b))
name = input('What is your name?' )
print(name + ' solo un persona te hace feliz y eres tu' )
peso = input("peso (kg): ")
print(type(peso))
print(peso) 
print(peso // 3)
# Strings Basics
course = 'thanks to support me'
print(course[0])
print(course[0:3])
print(course[:6])
print(course[-2])
print(course[:-3])
print(course[:])
print(course[-1:])
print (course[1:-1])
```
## Formated Strings
```
first = 'David'
last = 'Julian'
message = first + ' [' + last + '] is a code'
print(message)
msg = f'{first} [{last}] is a coder'
print(msg)
print (len(msg))
print(msg.upper())
print(msg.lower())
print(msg.find("i"))
print(msg.find('e'))
print(msg.find('av'))
print(msg.replace('av', 'q4'))
print(msg)
print('vid' in msg)
print(msg.title())
```
## Operation with Maths
```
print(10/3)
print(10%3)
print(20//3)
print(10**3)
x = 10
x += 2
print(x)
```
## Precedence operations
```
x = 10 + 3 * 2 ** 2
print(x)
z = (2 + 34) * 10 - 3
print(z)
```
## Math functions
```
import math
z = 2.4
print(abs(-2.4))
print(math.ceil(12.5))
print(math.floor(420.5))
print(math.tan(1))
```
## IF
```
is_hot = False
is_cold = True
if is_hot:
    print('really hot')
    print('drink water')
elif is_cold:
    print("wear warm clothes")
else:
    print('enjoy cold')
    print('Wear warm clothes')
print('Enjoy your day')
```
## While
```
i = 1
while i <= 5:
    print('x' * i)
    i = i + 1
print("Done")
```
## Program game to check answers
```
secret_number = 9
guess_count = 0
guess_limit = 3
while guess_count < guess_limit:
    guess = int(input("Guess:"))
    guess_count += 1
    if guess == secret_number:
        print('You won¡ gue_von')
        break
    else:
        print('you lost, try again just 3 chances')
```
## For
```
for item in 'Python':
    print(item)

for item in ['Python','Madona','Cesar']:
    print(item)

for item in range(3,10):
    print(item)

for item in range(3,10,2):
    print(item)

for item in range(3,10,2):
    print(item)

print('I am {} years old.'.format(str(28)))
print(int(6.7) + 1)
```
## For item sum prices
```
prices = [10, 20, 30]
total = 0
for price in prices:
    total += price
print(f"Total: {total}")
```
## Example coordinates for nested loops
```
for x in range(4):
    for y in range(3):
        print(f"({x},{y})")
```
## Example for iterate
```
numbers = [5,2,5,2,2]
for x_count in numbers:
    output = ''
    for item in range(x_count):
        output += "d"
    print(output)
```
## Example of nested names
```
names = ['Hernan','pedro','Rosa']
print (names[2])
print (names[-1])
print (names[:])
print (names[0:2])
names[0] = 'jon'
```
## Find the largest number of a list
```
numbers = [3,6,2,8,4,10]
max = numbers[0]
for number in numbers:
    if number > max:
        max = number
print(max)
```
## Rectangular numbers in MATRIX
```
matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
]
print(matrix[0][1])
print(matrix[0][2])
matrix[2][2] = 20
print(matrix[2][2])
for row in matrix:
    for item in row:
        print(item)
```
## Append or insert numbers in a list
```
numbers = [2,4,5,6,8]
numbers.append(20)
numbers.insert(1,10)
print(numbers)
numbers.insert(1,10)
print(numbers)
numbers.remove(5) #Finds the value on item and remove it
print(numbers)
numbers.clear() #Erase the object, remove all items
print(numbers)
```
## Methods for List
```
numbers = [5,2,4,5,6,8]
print(numbers)
numbers.pop() #Erase the last object in a list
print(numbers)
print(numbers.count(5)) # cuenta los elementos
print(numbers.index(5)) # trae el indice del elemento
print(6 in numbers) # Boolean result of evaluates the list
```
## Add info and copy a list
```
print(numbers.count(0))
numbers2 = numbers.copy()
print(numbers2)
numbers2.append(10)
print(numbers2)
```
## Remove the duplicates on a list
```
numbers = [5,2,4,5,6,8]
uniques = []
for number in numbers:
    if number not in uniques:
        uniques.append(number)
print(uniques)
```
## Sort a list
```
numbers = [5,2,4,5,6,8]
numbers.sort()
numbers.reverse()
print(numbers)
```
## Fixed items Alias "Tuple", inmutable items
```
numbers = (1,2,3) # you can not append or index insert // only count and index
print(numbers[0])
coordinates = (1,2,3)
x = coordinates[0]
y = coordinates[1]
z = coordinates[2]
print(x,y,z)
xa, ya, za = coordinates # diferent method to get values of a tuple
print( xa, ya, za )
```
## Dictionaries use as key.value pairs
```
customer = {
    "name":"David Bernal",
    "age": 36,
    "is_verified": True
}
print(customer["name"])
print(customer.get("name")) # this feature does not Return error if does not match
print(customer.get("birthdate","October 4 1984")) # ror if does not match
print(customer) # .get does not change the original data
customer["birthdate"] ="October 4 1984"
print(customer)
```
## Retrive information for a phone and add the name of the numbers
```
phone  = input("Phone: ")
digits_mapping = {
    "1":"One ",
    "2":"Two ",
    "3":"Three ",
    "4":"Four ",
    "5":"Five ",
    "6":"Six ",
    "7":"Seven ",
    "8":"Eight ",
    "9":"Nine ",
    "0":"Zero "
    }
output = ""
for ch in phone:
    output += digits_mapping.get(ch, "!")
print(output)
```
## Emoji Converter "important to evaluates words"
```
message = input(">")
words = message.split(' ') #uses the space to separate the string
emojis = {
    ":)":"HAAAAAAPY",
    ":(":"SAAAD",
}
output = ""
for word in words:
    output += emojis.get(word, word) + " "
print(output)
```
# Functions--------------------
```
def greet_user(name): # lowercase no spaces two lines at the end //name as a parameter
    print(f'Hi {name}') # receive an argument
    print('Welcome aboard')


print("Start")
greet_user("Lady") #Send to parameters in functions
greet_user("Mary")
print("Finish")
```
## Keyword arguments with no positional value
```
def greet_user(first_name, last_name):
    print(f'Hi {first_name} {last_name}') # receive an argument
    print('Welcome aboard')


print("Start")
greet_user("David", "Julian") #Send to parameters in functions
greet_user(last_name="Bernal", first_name="David") #keywords after positional parameters
print("Finish")
```
# Functions with return values
```
def square(number):
        result = (number * number)
        return result


print(square(4))# same result as before // all functions return none
```
## Reusable function
```
def emoji_converter(msg):
    words = msg.split(' ') #uses the space to separate the string
    emojis = {
    ":)":"HAAAAAAPY",
    ":(":"SAAAD",
    }
    output = ""
    for word in words:
        output += emojis.get(word, word) + " "
    return output


msg = input(">")
print(emoji_converter(msg))
```
## Exceptions -- handle errors
```
try:
    age = int(input('Age: '))
    income = 20000
    risk = income / age
    print(age)
except ValueError: # catch if is not number
    print('Invalid value')
except ZeroDivisionError: # catch if is divide by 0
    print('Value can not be 0')
```
# Classes in Py ----------------
```
class Point: #convention Pascal for Clases not _ or lower
    def move(self):
        print("move")
    def draw(self):
        print('draw')


point1 = Point()
point1.x = 10
point1.y = 20
print(point1.x)
point1.draw()
```
# Constructors --They Run just after the object is created--
```
class Point:
    def __init__(self, x, y):
        self.y = y
        self.x = x

point = Point(10, 20)
print(point.x)
print(point.y)
```
## Define a Person
```
class Person:
    def __init__(self, name):
        self.name = name

    def talk(self):
        print(f'talk to {self.name}')

john = Person("Jhon Smith")
print(john.talk())

Bob = Person("Bobs Esponja")
print(Bob.talk())
```
# Inheritance
class Mammal:
        def bark(self):
            print("Bark")


class Dog (Mammal):
    pass # just to pass in object creation


class Cat (Mammal):
    def be_annoying(self):
        print("annoying")

#dog1 = Dog()
cat1 = Cat()
cat1.bark()
cat1.be_annoying()
dog1 = Dog()
dog1.bark()
cat1 = Cat()
cat1.bark()
```
