# Звіт до роботи
## Тема: _Основи Python_
### Мета роботи: _Познайомитися з основами Python, виконати завдання та завантаження їх у репозиторій_
---
### Виконання роботи
- Результати виконання завдання *№1*;
1. Виконала приклади коду на Python
2. Створила новий файл `first_app.ipynb` та виконала в ньому базові приклади:
   і. Познайомилась з основними типами даних. Попрактивувалась з простими змінними, списками list, наборами set та словниками dict:
```python
a = "змінна з текстом"
b = 1
c = ["a", 1, 1.25, "Слово"]
d = {"a": "Слово", "b": 1}
e = ("a", )
f = {"ss", }

# Виведення значень змінних
print("Змінна 'a':", a)
print("Змінна 'b':", b)
print("Змінна 'c':", c)
print("Змінна 'd':", d)
print("Змінна 'e':", e)
print("Змінна 'f':", f) 
```
  іі. Вивела вбудовані константи:
```python
print("Перша константа True:", True)
print("Друга константа None:", None) 
```
  ііі. Вивела результати роботи вбудованих функцій:
```python
number = -42.5
print(f"Абсолютне значення числа {number}: {abs(number)}")

letters = ["a", "b", "c"]
print(f"Довжина списку letters: {len(letters)}")

numbers = [5, 10, 3]
print(f"Максимальне значення серед чисел {numbers}: {max(numbers)}") 
```
  іv. Познайомилась з циклами. Написала 3 коди які демонструють роботу циклів:
```python
# №1 Цикл for для списку
letters = ["a", "b", "c"]
for letter in letters:
    print(f"Буква: {letter}")

# №2 Цикл while для чисел
counter = 0
while counter < 5:
    print(f"Поточне значення лічильника: {counter}")
    counter += 1

# №3 Цикл for для кортежу
tuple_example = ("яблуко", "мандарин", "банан")
for fruit in tuple_example:
    print(f"Фрукт: {fruit}") 
```
  v. Познайомилась з розгалуженнями. Написала 3 коди які демонструють роботу розгалужень:
```python
# №1
number = 10
if number > 0:
    print("Число додатнє")
else:
    print("Число не додатнє")

# №2
grade = 85
if grade >= 90:
    print("Відмінно")
elif grade >= 70:
    print("Добре")
elif grade >= 50:
    print("Задовільно")
else:
    print("Не задовільно")

# №3
is_even = True
parity = "Парне" if is_even else "Непарне"
print(f"Число є {parity}") 
```
  vі. Конструкція try->except->finally. Написала свій варіант коду з помилкою:
```python
A = 0
try:
    result = 10 / A  
except ZeroDivisionError as e:
    print(f"Помилка: {e}")
finally:
    print("Код в блоку finally виконується навіть при помилці.") 
```
  vіі. Контекст-менеджер with. Написала свій код з контекст-менеджером:
```python
file_path = "example.txt"

try:
    with open(file_path, "r") as file:
        for line in file:
            print(line.strip())
except FileNotFoundError as e:
    print(f"Помилка: {e}") 
```
  vііі. Познайомилась з Python lambdas. Написала свій приклад коду:
```python
this_is_lambda = lambda first, last: f'Цей код написала: {first} {last}'
print("Це просто функція:", this_is_lambda)
print("Це її виклик:", this_is_lambda ('Іванна', 'Шумлянська'))

# №2 Лямбда-функція для обчислення суми двох чисел
add = lambda x, y: x + y

result = add(3, 5)
print(f"Результат додавання: {result}")

numbers = [1, 2, 3, 4, 5]
squared_numbers = list(map(lambda x: x**2, numbers))
print(f"Квадрати чисел: {squared_numbers}") 
```
3. Запитала у ChatGPT як би він розписав про основи Python.

Основи Python включають в себе роботу зі змінними, умовними операторами, циклами та функціями. Тут наведено кілька основних концепцій та приклади коду:

1. Змінні та типи даних:

```python
# Змінні
x = 5
y = "Hello, World!"

# Типи даних
integer_variable = 10
float_variable = 3.14
string_variable = "Python"
boolean_variable = True
```
2. Умовні оператори:
```python
# Умовний оператор if-else
age = 18
if age >= 18:
    print("Ви повнолітні")
else:
    print("Ви не повнолітні")

# Тернарний оператор
result = "Повнолітня" if age >= 18 else "Не повнолітня"
print(result)
```
3. Цикли:
```python
# Цикл for
for i in range(5):
    print(i)

# Цикл while
counter = 0
while counter < 5:
    print(counter)
    counter += 1
```
4. Функції:
```python
# Функція без параметрів
def greet():
    print("Привіт!")

greet()

# Функція з параметрами
def add_numbers(a, b):
    return a + b

result = add_numbers(3, 7)
print(result)
```
5. Списки та словники:
```python
# Список
numbers = [1, 2, 3, 4, 5]
print(numbers[2])  

# Словник
person = {"name": "Іванна", "age": 18, "city": "Львів"}
print(person["name"])  
```
Це лише кілька базових концепцій. Python має ще багато інших можливостей, таких як робота з класами, обробка винятків, модулі, та багато іншого. Ці приклади допоможуть вам розпочати, але для більш глибокого розуміння рекомендується вивчити офіційну документацію Python.

### Висновок: 
> у висновку потрібно відповісти на запитання:
- :question: Що зроблено в роботі;
- У роботі ми ознайомлювалися з основами Python, виконувала іх приклади та завантажувала їх у репозиторій
- :question: Чи досягнуто мети роботи;
- Мету роботи було досягнуто.
- :question: Чи вдалось відповісти на всі питання задані в ході роботи;
- Так.
- :question: Чи вдалося виконати всі завдання;
- Так.
- :question: Чи виникли складності у виконанні завдання;
- Складносте у виконанні завдання не виникало.
- :question: Чи подобається такий формат здачі роботи (Feedback);
- Так.
