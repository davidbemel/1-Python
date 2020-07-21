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
```
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
