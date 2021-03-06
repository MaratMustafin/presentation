import {
  CodeSurfer,
  CodeSurferColumns,
  Step,
} from "code-surfer";
import { Image, Notes, Head, Box } from "mdx-deck";
import { github, vsDark } from "@code-surfer/themes";

export const theme = vsDark;

## Школа преподавателя 👋

---

Всем привет меня зовут Марат, работаю преподавателем, учусь на 4 курсе. Пытаюсь занять себя чем угодно.
На курсе будем проходить темы по Python.

---

## Правила
- заходим вовремя на урок, не опаздываем
- запоминать, выполнять материал
- подсказывайте, поправляйте, автор сам много незнает

---

# План на 5 дней.

---

1 день 
- Знакомство
- Базовый Python
- Вопросы/Ответы


---

2 день
- Повторение
- Pyxel
- Вопросы/Ответы

---

3 день
- Повторение
- Flask
- Вопросы/Ответы

---

4 день
- Повторение
- Презентация
- Вопросы/Ответы

---

5 день
- Пробный урок
- Вопросы/Ответы

---

## Базовый python

---

<CodeSurferColumns>

<Step>

```python title="print" subtitle="математические операции"
print("Hello World!\n")

print(2+3*3)
print(3**3)
print(9/3)
print(9//3)
print(9%3)
```

</Step>

<Step subtitle="создание переменных">

```python
name = "Marat"
age = 21
print("My name is",name)
```

</Step>


</CodeSurferColumns>

---

<CodeSurferColumns>

<Step title="в чём разница">

```python
num = input("Enter first num:")
num2 = input("Enter second num:")
res = num + num2
print(res)
```

```python
num = int(input("Enter first num:"))
num2 = int(input("Enter second num:"))
res = num + num2
print(res)
```

</Step>

<Step title="в чём разница">

```python 3:4 subtitle="выведет строку"
num = input("Enter first num:")
num2 = input("Enter second num:")
res = num + num2
print(res)
```

```python 3:4 subtitle="выведет число"
num = int(input("Enter first num:"))
num2 = int(input("Enter second num:"))
res = num + num2
print(res)
```

</Step>


</CodeSurferColumns>

---

<CodeSurfer>


```python 1 title="типы данных" subtitle="число"
int()
str()
float()
bool()
```

```python 2 title="типы данных" subtitle="строка"
int()
str()
float()
bool()
```

```python 3 title="типы данных" subtitle="число с точкой"
int()
str()
float()
bool()
```

```python 4 title="типы данных" subtitle="логический тип"
int()
str()
float()
bool()
```

</CodeSurfer>

---

<CodeSurferColumns>

<Step title="условие" subtitle="одиночное условие">

```python
num = int(input("Enter first num:"))
if num > 0:
  print("Num is bigger than 0")
```


</Step>

<Step title="условие" subtitle="многа условия">

```python
num = int(input("Enter first num:"))
if num > 0:
  print("Num is bigger than 0")
elif num < 0:
  print("Num is lower than 0")
else: 
  print("It's 0")
```

</Step>

<Step title="условия" subtitle="вложенные условия">

```python
num = int(input("Enter first num:"))
if num > 0:
  print("Num is bigger than 0")
elif num < 0:
  print("Num is lower than 0")
else: 
  zero = input("Secret word:")
  if zero == 'zero':
    two = input('Secret word:")
    if two == 'two':
      print('На сегодня интернета достаточно')
```


</Step>

</CodeSurferColumns>

---

<CodeSurfer>

```python title="логический оператор"
and 
or 
not 
```

```python title="логический оператор" subtitle="и"
True and True # => True
True and False # = False
False and True # => False 
False and False # => False
```

```python title="логический оператор" subtitle="или"
True or True # => True 
True or False # => True 
False or True # => True 
False or False # => False 
```

```python title="логический оператор" subtitle="не"
not True # => False 
not False # => True 
```

</CodeSurfer>

---

<CodeSurfer>

```python title="циклы"
while True:
  stuff()
  if fail_condition:
    break
```

```python title="циклы"
i = 0  
while i < 10:
  i+=1
```

```python title="циклы"
for i in range(0,10):
  print(i)
```

```python title="циклы"
for i in [1,2,3,4,5]:
  print(i)
```

```python title="циклы"
for id,item in enumerate([1,2,3,4,5]):
  print(id,item)
```

</CodeSurfer>

---

<CodeSurfer>

```python 1 title="структура данных"
dict() # => словари
tuple() # => кортежи
list() # => массив
set() # => множества
```

```python 2:5 title="структура данных"
dict() # => словари
records = {
  'Suzan' : 'shemale',
  'Tom' : 'male'
}
tuple() # => кортежи
list() # => массив
set() # => множества
```

```python 2 title="структура данных"
dict() # => словари
tuple() # => кортежи
list() # => массив
set() # => множества
```

```python 3 title="структура данных"
dict() # => словари
tuple() # => кортежи
prettyNumber = (7,11,22,33,44,55,66,77,88,99)
list() # => массив
set() # => множества
```

```python 3 title="структура данных"
dict() # => словари
tuple() # => кортежи
list() # => массив
set() # => множества
```


```python 4 title="структура данных"
dict() # => словари
tuple() # => кортежи
list() # => массив
direction = [False,True,False,False]
set() # => множества
```

```python 4 title="структура данных"
dict() # => словари
tuple() # => кортежи
list() # => массив
set() # => множества
```

```python 5 title="структура данных"
dict() # => словари
tuple() # => кортежи
list() # => массив
set() # => множества
pinCode = {'1111','1111','1111','2222'}
```


</CodeSurfer>

---

<CodeSurferColumns>


<Step title="функции">

```python
def pr(string,num):
    print(string,num)
    pass 
```

</Step>

<Step title="функции">

```python
def summ(a,b):
    res = a+big
    return res
```

</Step>

<Step title="функции">

```python
def test(*args):
    print(args)
```

</Step>

<Step title="функции">

```python 
def ktest(**kwargs):
    print(kwargs)
``` 

</Step>

<Step title="вызов функций">

```python 
pr("Number is",56)
a = summ(23,56)
pr("Number is", a)
```

</Step>

</CodeSurferColumns>

---

<CodeSurfer>

```python title="модули"
import random as r 
from random import randint
```

</CodeSurfer>

---

<CodeSurferColumns>

<Step title="классы и объекты">

```python showNumbers
class Car:
    name = "None"
    weight = 1000
    speed = 200.00

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight
        print(self.name, " has weight", self.weight)

    def set(self, name, weight, speed):
        self.name = name
        self.weight = weight
        self.speed = speed

class Truck(Car):  # Унаследовали класс Car
    wheels = 8

    def __init__(self):
        pass  # Конструктор без параметров, который ничего не возвращает
              # Без пустого конструктора нужно передать параметры name, weight

man = Truck()  # Создали объект man
man.wheels = 12
man.set("Man", 4500, 140.5)
print(man.weight)


audi = Car("Audi", 1450)
audi.set("Audi", 1450, 320.30)
print(audi.name)

shkoda = Car("Shkoda", 1300)
shkoda.set("Shkoda", 1300, 235.30)
print(shkoda.name)
```
</Step>

<Step title="классы и объекты">

```python 1:5 showNumbers subtitle="класс Car"
class Car:
    name = "None"
    weight = 1000
    speed = 200.00

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight
        print(self.name, " has weight", self.weight)

    def set(self, name, weight, speed):
        self.name = name
        self.weight = weight
        self.speed = speed

class Truck(Car):  # Унаследовали класс Car
    wheels = 8

    def __init__(self):
        pass  # Конструктор без параметров, который ничего не возвращает
              # Без пустого конструктора нужно передать параметры name, weight

man = Truck()  # Создали объект man
man.wheels = 12
man.set("Man", 4500, 140.5)
print(man.weight)


audi = Car("Audi", 1450)
audi.set("Audi", 1450, 320.30)
print(audi.name)

shkoda = Car("Shkoda", 1300)
shkoda.set("Shkoda", 1300, 235.30)
print(shkoda.name)
```
</Step>

<Step title="классы и объекты">

```python 6:10 showNumbers subtitle="конструктор"

class Car:
    name = "None"
    weight = 1000
    speed = 200.00

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight
        print(self.name, " has weight", self.weight)

    def set(self, name, weight, speed):
        self.name = name
        self.weight = weight
        self.speed = speed

class Truck(Car):  # Унаследовали класс Car
    wheels = 8

    def __init__(self):
        pass  # Конструктор без параметров, который ничего не возвращает
              # Без пустого конструктора нужно передать параметры name, weight

man = Truck()  # Создали объект man
man.wheels = 12
man.set("Man", 4500, 140.5)
print(man.weight)


audi = Car("Audi", 1450)
audi.set("Audi", 1450, 320.30)
print(audi.name)

shkoda = Car("Shkoda", 1300)
shkoda.set("Shkoda", 1300, 235.30)
print(shkoda.name)
```
</Step>

<Step title="классы и объекты">

```python 11:15 showNumbers subtitle="метод set()"

class Car:
    name = "None"
    weight = 1000
    speed = 200.00

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight
        print(self.name, " has weight", self.weight)

    def set(self, name, weight, speed):
        self.name = name
        self.weight = weight
        self.speed = speed

class Truck(Car):  # Унаследовали класс Car
    wheels = 8

    def __init__(self):
        pass  # Конструктор без параметров, который ничего не возвращает
              # Без пустого конструктора нужно передать параметры name, weight

man = Truck()  # Создали объект man
man.wheels = 12
man.set("Man", 4500, 140.5)
print(man.weight)


audi = Car("Audi", 1450)
audi.set("Audi", 1450, 320.30)
print(audi.name)

shkoda = Car("Shkoda", 1300)
shkoda.set("Shkoda", 1300, 235.30)
print(shkoda.name)
```
</Step>

<Step title="классы и объекты">

```python 16:22 showNumbers subtitle="класс Track"

class Car:
    name = "None"
    weight = 1000
    speed = 200.00

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight
        print(self.name, " has weight", self.weight)

    def set(self, name, weight, speed):
        self.name = name
        self.weight = weight
        self.speed = speed

class Truck(Car):  # Унаследовали класс Car
    wheels = 8

    def __init__(self):
        pass  # Конструктор без параметров, который ничего не возвращает
              # Без пустого конструктора нужно передать параметры name, weight

man = Truck()  # Создали объект man
man.wheels = 12
man.set("Man", 4500, 140.5)
print(man.weight)


audi = Car("Audi", 1450)
audi.set("Audi", 1450, 320.30)
print(audi.name)

shkoda = Car("Shkoda", 1300)
shkoda.set("Shkoda", 1300, 235.30)
print(shkoda.name)
```
</Step>

<Step title="классы и объекты">

```python 23:36 showNumbers

class Car:
    name = "None"
    weight = 1000
    speed = 200.00

    def __init__(self, name, weight):
        self.name = name
        self.weight = weight
        print(self.name, " has weight", self.weight)

    def set(self, name, weight, speed):
        self.name = name
        self.weight = weight
        self.speed = speed

class Truck(Car):  # Унаследовали класс Car
    wheels = 8

    def __init__(self):
        pass  # Конструктор без параметров, который ничего не возвращает
              # Без пустого конструктора нужно передать параметры name, weight

man = Truck()  # Создали объект man
man.wheels = 12
man.set("Man", 4500, 140.5)
print(man.weight)


audi = Car("Audi", 1450)
audi.set("Audi", 1450, 320.30)
print(audi.name)

shkoda = Car("Shkoda", 1300)
shkoda.set("Shkoda", 1300, 235.30)
print(shkoda.name)
```
</Step>

</CodeSurferColumns>

---

## Спасибо за урок

---

# 2 день.

---

2 день
- Повторение
- [Pyxel](https://github.com/kitao/pyxel)
- Вопросы/Ответы

---

# Что такое API?

---

- [API](https://habr.com/ru/post/464261/#api)
- [PythonAwesome](https://awesome-python.com/)
- [PIP](https://pip.pypa.io/en/stable/)
- [PyPi](https://pypi.org/)
- [SetupTools](https://pypi.org/project/setuptools/)

---

Сегодня будем разбирать игру змейка
- [исходный код](https://github.com/CaffeinatedTech/Python_Nibbles)
- [видео](https://www.youtube.com/watch?v=Qg16VhEo2Qs)

---

<CodeSurferColumns>

<Step title="nibbles" >

```python 1:10 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 1:10 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 13:18 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 21:24 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 27:37 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 42:47 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 49:50 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 52:61 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 63:65 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 68:76 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 78:83 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 84:99 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 101:110 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 113:122 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 126:135 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 137:139 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 141:145 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 147:150 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 152:155 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 158 showNumbers file="./nibbles1.py" subtitle="запускатор"
```

</Step>

<Step title="nibbles" >

```python 158:184 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 186:206 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 208:219 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 221:227 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 229:239 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 241:262 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 243:249 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 251:257 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 258:262 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 263:286 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 287:316 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 290:295 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 297:306 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 308:316 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 317:351 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 319:323 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 324:330 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 331:337 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 338:344 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>

<Step title="nibbles" >

```python 345:351 showNumbers file="./nibbles1.py" subtitle="это что"
```

</Step>


</CodeSurferColumns>


---

<CodeSurfer>

```python
from setuptools import setup,find_packages

setup(
    name='nibbles',
    version='1.0',
    description='Описание игры',
    author=' CaffeinatedTech ',
    author_email='',
    url='https://github.com/CaffeinatedTech/Python_Nibbles',
    py_modules=['main'],
    packages = find_packages(),
    install_requires=[
          'pyxel',
      ],
)
```

</CodeSurfer>

---


# Спасибо за урок