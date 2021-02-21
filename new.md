import {
  CodeSurfer,
  CodeSurferColumns,
  Step,
} from "code-surfer";
import { Image, Notes, Head } from "mdx-deck";
import { github, vsDark } from "@code-surfer/themes";
import customTheme from "./custom-theme"

export const theme = vsDark;

## Школа преподавателя 👋

---

Всем привет меня зовут Марат, работаю преподавателем, учусь на 4 курсе. Пытаюсь занять себя чем угодно.
На курсе будем проходить темы по Python.

---

## Правила
- 
- 
- если чето знаете, можете добавить
-

<CodeSurfer>

```python
План на 5 дней. 


---

1 день 
- Знакомство
- Базовый Python
- Вопросы/Ответы


---

2 день
- Повторение
- Pyxel API 
- Вопросы/Ответы

---

3 день
- Повторение
- Werkzeug API
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

```python
print("Hello World!\n")

print(2+3*3)
print(3**3)
print(9/3)
print(9//3)
print(9%3)

```

---

```python
name = "Marat"
age = 21
print("My name is",name)
```

---

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

---

## Типы данных

```python
int()
str()
float()
bool()
object()
```

---

## Условные операторы

```python
num = int(input("Enter first num:"))
if num > 0:
  print("Num is bigger than 0")
```

```python
num = int(input("Enter first num:"))
if num > 0:
  print("Num is bigger than 0")
elif num < 0:
  print("Num is lower than 0")
else: 
  print("It's 0")
```

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


---

## Логические операторы

```python
and 
or 
not 
```

```python 
True and True # => True
True and False # = False
False and True # => False 
False and False # => False
```

```python
True or True # => True 
True or False # => True 
False or True # => True 
False or False # => False 
```

```python
not True # => False 
not False # => True 
```

---

Циклы 
```python
while True:
  stuff()
  if fail_condition:
    break
```

```python 
i = 0 
while i < 10:
  i+=1
```

```python 
for i in range(0,10):
  print(i)
```

```python
for i in [1,2,3,4,5]:
  print(i)
```

```python
for id,item in enumerate([1,2,3,4,5]):
  print(id,item)
```

---

## Структура данных

```python
dict() # => словари
tuple() # => кортежи
list() # => массив
set() # => множества
```

---

Функции

```python
def pr(string,num):
  print(string,num)
  pass 
```

```python
def summ(a,b):
  res = a+big
  return res
```

```python
def test(*args):
  print(args)
``` 

```python 
def ktest(**kwargs):
  print(kwargs)
``` 

```python 
pr("Number is",56)
a = summ(23,56)
pr("Number is", a)
```

---

## Модули 

```python 
import random as r 
from random import randint
```

---

## Классы и объекты

```python
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

---
<CodeSurfer>

```python
type(str(123213))
```

</CodeSurfer>

---