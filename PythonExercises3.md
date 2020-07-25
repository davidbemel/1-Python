# Modules  ------
## First form to  import
```
import modules
print(modules.kg_to_lb(90))
```
## Second form to import modules
```
import modules
from modules import kg_to_lb
from modules import find_max

kg_to_lb(1)
print(modules.kg_to_lb(92))
numbers = [2,4,6,8,9,712,4,7,321,5,87,321,89,5]
maximum = find_max(numbers)
print(maximum)
```
## Modules used by python
```
def lbs_to_kg(weight):
    return weight * 0.45


def kg_to_lb(weight):
    return weight / 0.45


def find_max(numbers):
    maximum = numbers[0]
    for number in numbers:
        if number > maximum:
            maximum = number
    return maximum
```
# Packages ----- Needs to create a directory with __init__ and file.py
## First option import package
```
import ecommerce.shipping
ecommerce.shipping.calc_shipping()
```
## Second option import function
```
from ecommerce.shipping import calc_shipping
calc_shipping()
```
## Third option import module
```
from ecommerce import shipping
shipping.calc_shipping()
```
# Example of modules form python // search python 3 module index
## Use of Random module from Py
```
import random

for i in range(3):
    print(random.random())
    print(random.randint(10,30))
```
## Program for select a leader
```
import random

members = ['Jhon','Pascual','Rosa','Rigo']
leader = random.choice(members)
print(leader)
```
## Program to Roll A Dice
```
import random


class Dice:
    def roll(self):
        first = random.randint(1, 6)
        second = random.randint(1, 6)
        return first, second  # not add () Automatically generates a tuple


dice = Dice()
print(dice.roll())
```
# Files and directories // Use of Path Class in the Pathlib
## Either you can use Absolute path or Relative
```
from pathlib import Path
path = Path("ecommerce")
print(path.exists())
print(Path())
path = Path("emails")
```
### create folder
```
print(path.mkdir())
```
### delete folder
```
(path.rmdir())
```
## Moves in folder glob method
```
from pathlib import Path

path = Path()
print(path.glob('*'))  # generates an object files and directories
print(path.glob('*.*'))  # Generates just files
print(path.glob('*.py'))  # python files
print(path.glob('*.xls))  # excel files
```
## Need to Print the object in folder glob method for review

from pathlib import Path

path = Path()
for file in path.glob('*.py'):
    print(file)
```
