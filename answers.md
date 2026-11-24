# Итоговая проверочная работа по аттестации

**ФИО:** Мкртчян Юрик  
**Группа:** 3-ИСП9-54

---

# Часть I

## A. Тест

**1. Что вернёт `len([1, [2, 3], [], 4])`?**
- а) `3`
- б) `4`
- в) `5`
- г) Ошибку

## **Ответ: б) `4`**

**2. Что произойдёт при выполнении?**
```python
a = [1, 2, 3]
b = a[:]
b.append(4)
print(a)
```
- а) `[1, 2, 3, 4]`
- б) `[1, 2, 3]`
- в) `[4]`
- г) Ошибку

## **Ответ: б) `[1, 2, 3]`**

**3. Что вернёт `[1, 2, 3, 4, 5][2:-1]`?**
- а) `[3, 4]`
- б) `[3, 4, 5]`
- в) `[2, 3, 4]`
- г) `[2, 3, 4, 5]`

## **Ответ: а) `[3, 4]`**

**4. Что делает `lst.sort(reverse=True)`?**
- а) Возвращает новый список по убыванию
- б) Сортирует список **на месте** по убыванию, возвращает `None`
- в) Разворачивает список
- г) Удаляет дубликаты

## **Ответ: б) Сортирует список на месте по убыванию, возвращает `None`**

**5. Что вернёт `[1, 2, 3].index(2)`?**
- а) `2`
- б) `1`
- в) `0`
- г) `-1`

## **Ответ: б) `1`**

**6. Что произойдёт, если после `INSERT` не вызвать `conn.commit()` и закрыть соединение?**
- а) Данные сохранятся
- б) Данные не будут записаны на диск
- в) Python выбросит `ProgrammingError`
- г) Данные запишутся в другую таблицу

## **Ответ: б) Данные не будут записаны на диск**

**7. Какой запрос защищён от SQL-инъекции?**
- а) `cursor.execute(f"SELECT * FROM t WHERE id = {id}")`
- б) `cursor.execute("SELECT * FROM t WHERE id = ?", (id,))`
- в) `cursor.execute("SELECT * FROM t WHERE id = " + str(id))`
- г) `cursor.execute("SELECT * FROM t WHERE id = %d" % id)`

## **Ответ: б) `cursor.execute("SELECT * FROM t WHERE id = ?", (id,))`**

**8. Что делает `conn.rollback()`?**
- а) Закрывает соединение
- б) Отменяет текущую транзакцию
- в) Удаляет все таблицы
- г) Создаёт резервную копию

## **Ответ: б) Отменяет текущую транзакцию**

**9. Что вернёт `cursor.rowcount` после `DELETE FROM t WHERE id = 999`, если строки с id=999 нет?**
- а) `None`
- б) `0`
- в) `1`
- г) `-1`

## **Ответ: б) `0`**

**10. Зачем нужен `sqlite3.Row`?**
- а) Для сортировки строк
- б) Чтобы обращаться к полям результата по имени: `row['title']`
- в) Для создания новых строк в таблице
- г) Для защиты от SQL-инъекций

## **Ответ: б) Чтобы обращаться к полям результата по имени: `row['title']`**

**11. Что делает декоратор `@app.route('/')`?**
- а) Создаёт новую таблицу
- б) Связывает URL `/` с функцией-обработчиком
- в) Запускает сервер на порту 80
- г) Возвращает HTML-страницу

## **Ответ: б) Связывает URL `/` с функцией-обработчиком**

**12. Что произойдёт, если отправить POST на маршрут, объявленный без `methods=['POST']`?**
- а) Flask автоматически обработает POST
- б) Вернётся 404
- в) Вернётся 405 Method Not Allowed
- г) Данные потеряются

## **Ответ: в) Вернётся 405 Method Not Allowed**

**13. Где по умолчанию Flask ищет HTML-шаблоны?**
- а) В папке `html/`
- б) В папке `views/`
- в) В папке `templates/`
- г) В корне проекта

## **Ответ: в) В папке `templates/`**

**14. Зачем нужен `redirect(url_for('index'))` после успешного POST?**
- а) Для ускорения работы
- б) Для защиты от дублирования при F5 (PRG-паттерн)
- в) Для сохранения данных в базу
- г) Для валидации формы

## **Ответ: б) Для защиты от дублирования при F5 (PRG-паттерн)**

**15. Что вернёт `url_for('index')`, если функция называется `def index():` и маршрут `/`?**
- а) `'index'`
- б) `'/'`
- в) `'http://127.0.0.1:5000'`
- г) Объект функции

## **Ответ: б) `'/'`**

**16. Что делает `request.form.get('title', '')`?**
- а) Возвращает объект формы
- б) Возвращает значение поля `title` или пустую строку, если поля нет
- в) Выбрасывает `KeyError`, если поля нет
- г) Создаёт поле формы

## **Ответ: б) Возвращает значение поля `title` или пустую строку, если поля нет**

**17. Что произойдёт при выполнении?**
```python
def f(lst):
    lst.append(1)

a = []
f(a)
print(a)
```
- а) `[]`
- б) `[1]`
- в) `None`
- г) Ошибку

## **Ответ: б) `[1]`**

**18. Что выведет код?**
```python
x = [1, 2, 3]
y = x
y[0] = 100
print(x)
```
- а) `[1, 2, 3]`
- б) `[100, 2, 3]`
- в) `[100]`
- г) Ошибку

## **Ответ: б) `[100, 2, 3]`**

**19. Какая ошибка возникнет при выполнении?**
```python
lst = [1, 2, 3]
lst[5] = 10
```
- а) `KeyError`
- б) `ValueError`
- в) `IndexError`
- г) `TypeError`

## **Ответ: в) `IndexError`**

**20. Что выведет код?**
```python
result = []
for i in range(3):
    result.append(lambda: i)
print([f() for f in result])
```
- а) `[0, 1, 2]`
- б) `[2, 2, 2]`
- в) `[3, 3, 3]`
- г) Ошибку

## **Ответ: б) `[2, 2, 2]`**

## B. Что выведет код

### 21.

```python
a = [1, 2, 3, 4, 5]
b = a[1:4]
b[0] = 100
print(a)
print(b)
```

## **Ответ — вывод:**

```text
[1, 2, 3, 4, 5]
[100, 3, 4]
```

### 22.

```python
lst = [3, 1, 2]
x = lst.sort()
print(x)
print(lst)
```

## **Ответ — вывод:**

```text
None
[1, 2, 3]
```

### 23.

```python
a = [1, 2]
b = a
a = a + [3]
print(a)
print(b)
```

## **Ответ — вывод:**

```text
[1, 2, 3]
[1, 2]
```

### 24.

```python
a = [1, 2]
b = a
a += [3]
print(a)
print(b)
```

## **Ответ — вывод:**

```text
[1, 2, 3]
[1, 2, 3]
```

### 25.

```python
def modify(lst):
    lst = lst + [99]
    return lst

original = [1, 2, 3]
result = modify(original)
print(original)
print(result)
```

## **Ответ — вывод:**

```text
[1, 2, 3]
[1, 2, 3, 99]
```

### 26.

```python
data = {'a': 1, 'b': 2}
items = list(data.items())
items[0] = ('x', 100)
print(data)
print(items)
```

## **Ответ — вывод:**

```text
{'a': 1, 'b': 2}
[('x', 100), ('b', 2)]
```

### 27.

```python
matrix = [[1, 2], [3, 4]]
copy = matrix.copy()
copy[0][0] = 100
print(matrix)
print(copy)
```

## **Ответ — вывод:**

```text
[[100, 2], [3, 4]]
[[100, 2], [3, 4]]
```

### 28.

```python
lst = [1, 2, 3, 4, 5, 6]
even = [x for x in lst if x % 2 == 0]
squares = [x ** 2 for x in even]
print(even)
print(squares)
```

## **Ответ — вывод:**

```text
[2, 4, 6]
[4, 16, 36]
```

## C. Дописать код

### 29. Функция поиска минимума (4 балла)

**Код с пропусками:**

```python
def find_min(numbers):
    """Возвращает минимальное число в списке. Список не пустой."""
    if not numbers:
        return None
    minimum = ???              # (1) начальное значение
    for n in numbers:
        if n < ???:            # (2) условие сравнения
            minimum = ???      # (3) обновление минимума
    return ???                 # (4) что вернуть
```

## **Ответ:**

```python
def find_min(numbers):
    if not numbers:
        return None
    minimum = numbers[0]
    for n in numbers:
        if n < minimum:
            minimum = n
    return minimum
```

### 30. Функция удаления по значению (4 балла)

**Код с пропусками:**

```python
def remove_all(lst, value):
    """Удаляет ВСЕ вхождения value из lst. Изменяет lst на месте."""
    i = 0
    while i < ???:                                # (1) граница цикла
        if lst[i] == value:
            lst.???                                # (2) удалить элемент
            # (3) НЕ увеличиваем i — иначе пропустим следующий элемент
        else:
            i += ???                               # (4) сдвиг вперёд
```

## **Ответ:**

```python
def remove_all(lst, value):
    i = 0
    while i < len(lst):
        if lst[i] == value:
            lst.pop(i)
        else:
            i += 1
```

После удаления следующий элемент занимает индекс i, поэтому i увеличивается только в ветке else.

### 31. Функция работы с БД (4 балла)

**Код с пропусками:**

```python
import sqlite3

def get_done_tasks():
    """Возвращает список названий задач со статусом 'done'."""
    conn = sqlite3.connect('app.db')
    conn.row_factory = ???                                 # (1) доступ по имени
    try:
        cursor = conn.cursor()
        cursor.execute("SELECT title FROM tasks WHERE status = ???", ('done',))  # (2) плейсхолдер
        return cursor.???                                  # (3) получить все строки
    except sqlite3.Error as e:
        print(f"[DB ERROR] {e}")
        return ???
    finally:
        ???                                                # (4) закрыть соединение
```

## **Ответ:**

```python
import sqlite3

def get_done_tasks():
    conn = sqlite3.connect('app.db')
    conn.row_factory = sqlite3.Row
    try:
        cursor = conn.cursor()
        cursor.execute("SELECT title FROM tasks WHERE status = ?", ('done',))
        return [row['title'] for row in cursor.fetchall()]
    except sqlite3.Error as e:
        print(f"[DB ERROR] {e}")
        return []
    finally:
        conn.close()
```

### 32. Маршрут Flask (4 балла)

**Код с пропусками:**

```python
from flask import Flask, render_template, request, redirect, url_for
import sqlite3

app = Flask(__name__)

@app.route('/', methods=???)                              # (1) методы
def index():
    if request.method == 'POST':
        title = request.form.get('title', '').strip()
        if not title:
            return render_template('index.html', items=[], error='Пусто!')

        conn = sqlite3.connect('app.db')
        try:
            cursor = conn.cursor()
            cursor.execute("INSERT INTO tasks (title) VALUES (?)", (title,))
            conn.???                                      # (2) фиксация
        except sqlite3.Error as e:
            conn.???                                      # (3) откат
            return render_template('index.html', items=[], error=str(e))
        finally:
            conn.close()

        return ???                                        # (4) PRG-редирект

    return render_template('index.html', items=[])
```

## **Ответ:**

```python
from flask import Flask, render_template, request, redirect, url_for
import sqlite3

app = Flask(__name__)

@app.route('/', methods=['GET', 'POST'])
def index():
    if request.method == 'POST':
        title = request.form.get('title', '').strip()
        if not title:
            return render_template('index.html', items=[], error='Пусто!')

        conn = sqlite3.connect('app.db')
        try:
            cursor = conn.cursor()
            cursor.execute("INSERT INTO tasks (title) VALUES (?)", (title,))
            conn.commit()
        except sqlite3.Error as e:
            conn.rollback()
            return render_template('index.html', items=[], error=str(e))
        finally:
            conn.close()

        return redirect(url_for('index'))

    return render_template('index.html', items=[])
```

### 33. Обработка ошибок (4 балла)

**Код с пропусками:**

```python
import sqlite3

def safe_insert(title):
    """Вставляет задачу. При ошибке — откат и возврат False."""
    conn = sqlite3.connect('app.db')
    try:
        cursor = conn.cursor()
        cursor.execute("INSERT INTO tasks (title) VALUES (?)", (title,))
        conn.???                                      # (1) фиксация
        return ???
    except sqlite3.??? as e:                          # (2) какой класс ошибки
        conn.???                                      # (3) откат
        print(f"[DB ERROR] {e}")
        return ???
    finally:
        conn.close()
```

## **Ответ:**

```python
import sqlite3

def safe_insert(title):
    conn = sqlite3.connect('app.db')
    try:
        cursor = conn.cursor()
        cursor.execute("INSERT INTO tasks (title) VALUES (?)", (title,))
        conn.commit()
        return True
    except sqlite3.Error as e:
        conn.rollback()
        print(f"[DB ERROR] {e}")
        return False
    finally:
        conn.close()
```

## D. Самостоятельные задачи

### 34. Списки: пересечение двух списков (6 баллов)

**Задание:** Напиши функцию, которая возвращает **список общих элементов** двух списков **без дубликатов**, сохраняя порядок появления в первом списке.

## **Ответ:**

```python
def intersection(a, b):
    result = []
    for item in a:
        if item in b and item not in result:
            result.append(item)
    return result
```

### 35. Списки: сглаживание вложенного списка (6 баллов)

**Задание:** Напиши функцию, которая принимает список, элементы которого — списки или числа, и возвращает **плоский список** всех чисел в том же порядке. **Запрещено** использовать рекурсию и `itertools.chain`.

## **Ответ:**

```python
def flatten(lst):
    result = []
    for item in lst:
        if isinstance(item, list):
            result.extend(item)
        else:
            result.append(item)
    return result
```

### 36. Списки: группировка по чётности (6 баллов)

**Задание:** Напиши функцию, которая возвращает **словарь** с двумя ключами `'even'` и `'odd'`, где значения — списки чётных и нечётных чисел соответственно. Порядок чисел сохраняется.

## **Ответ:**

```python
def group_by_parity(numbers):
    result = {'even': [], 'odd': []}
    for number in numbers:
        if number % 2 == 0:
            result['even'].append(number)
        else:
            result['odd'].append(number)
    return result
```

### 37. SQLite: CRUD-функция (10 баллов)

**Задание:** Дана таблица `students` с колонками `id INTEGER PRIMARY KEY`, `name TEXT NOT NULL`, `grade INTEGER`. Напиши **три функции** с полной защитой соединений (`try/except/finally` + `rollback`):

**37.1.** `add_student(name, grade)` — вставляет студента. Возвращает `True` при успехе, `False` при ошибке (2 балла).

**37.2.** `get_all_students()` — возвращает список кортежей `(id, name, grade)`. При ошибке возвращает пустой список. **Обязательно** используй `sqlite3.Row` (3 балла).

**37.3.** `update_grade(student_id, new_grade)` — обновляет оценку. Возвращает `rowcount` (3 балла).

**37.4.** `delete_failing()` — удаляет всех студентов с `grade < 3`. Возвращает количество удалённых (2 балла).

## **Ответ:**

```python
import sqlite3

DB_PATH = 'students.db'

def add_student(name, grade):
    conn = sqlite3.connect(DB_PATH)
    try:
        conn.execute(
            "INSERT INTO students (name, grade) VALUES (?, ?)",
            (name, grade)
        )
        conn.commit()
        return True
    except sqlite3.Error:
        conn.rollback()
        return False
    finally:
        conn.close()

def get_all_students():
    conn = sqlite3.connect(DB_PATH)
    conn.row_factory = sqlite3.Row
    try:
        rows = conn.execute("SELECT id, name, grade FROM students").fetchall()
        return [(row['id'], row['name'], row['grade']) for row in rows]
    except sqlite3.Error:
        conn.rollback()
        return []
    finally:
        conn.close()

def update_grade(student_id, new_grade):
    conn = sqlite3.connect(DB_PATH)
    try:
        cursor = conn.execute(
            "UPDATE students SET grade = ? WHERE id = ?",
            (new_grade, student_id)
        )
        conn.commit()
        return cursor.rowcount
    except sqlite3.Error:
        conn.rollback()
        return 0
    finally:
        conn.close()

def delete_failing():
    conn = sqlite3.connect(DB_PATH)
    try:
        cursor = conn.execute("DELETE FROM students WHERE grade < ?", (3,))
        conn.commit()
        return cursor.rowcount
    except sqlite3.Error:
        conn.rollback()
        return 0
    finally:
        conn.close()
```

### 38. Flask: полный маршрут «Добавить + Показать» (8 баллов)

**Задание:** Напиши **маршрут** `/students`, который:
- На **GET** — показывает список студентов (шаблон `students.html` с переменной `students`).
- На **POST** — принимает поля `name` и `grade`, валидирует (name не пустой, grade — целое от 1 до 5), вставляет в БД, делает редирект на GET `/students`.
- При ошибке валидации — возвращает шаблон с сообщением об ошибке в переменной `error`.
- При ошибке БД — делает `rollback` и возвращает шаблон с сообщением.

## **Ответ:**

```python
from flask import Flask, render_template, request, redirect, url_for
import sqlite3

app = Flask(__name__)
DB_PATH = 'students.db'

@app.route('/students', methods=['GET', 'POST'])
def students():
    if request.method == 'POST':
        name = request.form.get('name', '').strip()
        grade_text = request.form.get('grade', '').strip()

        if not name:
            return render_template('students.html', students=[], error='Введите имя')
        try:
            grade = int(grade_text)
        except ValueError:
            return render_template('students.html', students=[], error='Оценка должна быть целым числом от 1 до 5')
        if not 1 <= grade <= 5:
            return render_template('students.html', students=[], error='Оценка должна быть от 1 до 5')

        conn = sqlite3.connect(DB_PATH)
        try:
            conn.execute(
                "INSERT INTO students (name, grade) VALUES (?, ?)",
                (name, grade)
            )
            conn.commit()
        except sqlite3.Error as e:
            conn.rollback()
            return render_template('students.html', students=[], error=str(e))
        finally:
            conn.close()
        return redirect(url_for('students'))

    conn = sqlite3.connect(DB_PATH)
    try:
        rows = conn.execute("SELECT id, name, grade FROM students").fetchall()
    except sqlite3.Error as e:
        conn.rollback()
        return render_template('students.html', students=[], error=str(e))
    finally:
        conn.close()
    return render_template('students.html', students=rows)
```

### 39. Комплексная задача: «Топ-3 студента» (8 баллов)

**Задание:** Напиши **функцию** `top_three_by_grade(students)`, которая принимает **список кортежей** `(name, grade)` и возвращает **список из трёх имён** с наивысшими оценками. Если студентов меньше трёх — вернуть всех. При равных оценках — сохраняется порядок появления в исходном списке.

**Запрещено** использовать `sorted()` и `.sort()` с `key=lambda`. Разрешён один проход с ручным поддержанием «топ-3».

## **Ответ:**

```python
def top_three_by_grade(students):
    top = []
    for name, grade in students:
        position = 0
        while position < len(top) and top[position][1] >= grade:
            position += 1
        top.insert(position, (name, grade))
        if len(top) > 3:
            top.pop()
    return [name for name, grade in top]
```

---

# Часть II

## A. Тест

**1. Что вернёт `len({'a': 1, 'b': 2, 'c': 3})`?**
- а) `3`
- б) `6`
- в) `2`
- г) Ошибку

## **Ответ: а) `3`**

**2. Что произойдёт при выполнении?**
```python
d = {'a': 1}
d['b'] = 2
print(d)
```
- а) `{'a': 1}`
- б) `{'a': 1, 'b': 2}`
- в) `{'b': 2}`
- г) Ошибку

## **Ответ: б) `{'a': 1, 'b': 2}`**

**3. Что вернёт `{'a': 1}.get('b', 0)`?**
- а) `None`
- б) `0`
- в) `KeyError`
- г) `1`

## **Ответ: б) `0`**

**4. Что произойдёт при выполнении?**
```python
t = (1, 2, 3)
t[0] = 100
```
- а) `t` станет `(100, 2, 3)`
- б) `TypeError` — кортеж неизменяем
- в) `IndexError`
- г) `t` станет `[100, 2, 3]`

## **Ответ: б) `TypeError` — кортеж неизменяем**

**5. Что вернёт `tuple([1, 2, 3])`?**
- а) `[1, 2, 3]`
- б) `(1, 2, 3)`
- в) `1, 2, 3`
- г) Ошибку

## **Ответ: б) `(1, 2, 3)`**

**6. Что вернёт `len((1,))`?**
- а) `0`
- б) `1`
- в) `2`
- г) Ошибку

## **Ответ: б) `1`**

**7. Что делает `d.keys()`?**
- а) Возвращает список ключей
- б) Возвращает «представление» ключей (view), по которому можно итерироваться
- в) Возвращает значения словаря
- г) Удаляет все ключи

## **Ответ: б) Возвращает «представление» ключей (view), по которому можно итерироваться**

**8. Как проверить, есть ли ключ `'a'` в словаре `d`?**
- а) `d['a']` — выбросит ошибку, если нет
- б) `'a' in d`
- в) `d.contains('a')`
- г) `d.has('a')`

## **Ответ: б) `'a' in d`**

**9. Что вернёт `len({1, 2, 2, 3, 3, 3})`?**
- а) `6`
- б) `3`
- в) `2`
- г) Ошибку

## **Ответ: б) `3`**

**10. Что вернёт `{1, 2, 3} & {2, 3, 4}`?**
- а) `{1, 2, 3, 4}`
- б) `{2, 3}`
- в) `{1, 4}`
- г) `{}`

## **Ответ: б) `{2, 3}`**

**11. Что вернёт `{1, 2, 3} | {3, 4}`?**
- а) `{3}`
- б) `{1, 2, 3, 4}`
- в) `{1, 2, 4}`
- г) Ошибку

## **Ответ: б) `{1, 2, 3, 4}`**

**12. Что вернёт `{1, 2, 3} - {2}`?**
- а) `{1, 3}`
- б) `{2}`
- в) `{1, 2, 3}`
- г) `{}`

## **Ответ: а) `{1, 3}`**

**13. Что произойдёт при выполнении?**
```python
s = {1, 2, 3}
s.add([4, 5])
```
- а) Множество станет `{1, 2, 3, [4, 5]}`
- б) `TypeError` — список не хешируемый, нельзя добавить в множество
- в) `ValueError`
- г) Ошибку не будет, но `[4, 5]` не добавится

## **Ответ: б) `TypeError` — список не хешируемый, нельзя добавить в множество**

**14. Какой запрос защищён от SQL-инъекции?**
- а) `cursor.execute(f"SELECT * FROM t WHERE name = '{name}'")`
- б) `cursor.execute("SELECT * FROM t WHERE name = ?", (name,))`
- в) `cursor.execute("SELECT * FROM t WHERE name = " + name)`
- г) `cursor.execute("SELECT * FROM t WHERE name = %s" % name)`

## **Ответ: б) `cursor.execute("SELECT * FROM t WHERE name = ?", (name,))`**

**15. Что делает `conn.rollback()`?**
- а) Закрывает соединение
- б) Отменяет текущую транзакцию
- в) Создаёт резервную копию
- г) Удаляет таблицу

## **Ответ: б) Отменяет текущую транзакцию**

**16. Что вернёт `cursor.rowcount` после `UPDATE t SET x = 1 WHERE id = 99`, если строки нет?**
- а) `None`
- б) `0`
- в) `1`
- г) `-1`

## **Ответ: б) `0`**

**17. Что делает `@app.route('/item/<int:item_id>')`?**
- а) Принимает только POST-запросы
- б) Связывает URL `/item/5` с функцией, где `item_id = 5` (целое число)
- в) Создаёт таблицу `item`
- г) Принимает только GET-запросы

## **Ответ: б) Связывает URL `/item/5` с функцией, где `item_id = 5` (целое число)**

**18. Что произойдёт, если отправить POST на маршрут без `methods=['POST']`?**
- а) Flask автоматически обработает POST
- б) Вернётся 404
- в) Вернётся 405 Method Not Allowed
- г) Данные потеряются

## **Ответ: в) Вернётся 405 Method Not Allowed**

**19. Что вернёт `url_for('index')`, если функция называется `def index():` и маршрут `/`?**
- а) `'index'`
- б) `'/'`
- в) `'http://127.0.0.1:5000'`
- г) Объект функции

## **Ответ: б) `'/'`**

**20. Что выведет код?**
```python
d = {1: 'a', 2: 'b'}
for key in d:
    print(key)
```
- а) `1`, `2`
- б) `'a'`, `'b'`
- в) `(1, 'a')`, `(2, 'b')`
- г) Ошибку

## **Ответ: а) `1`, `2`**

## B. Что выведет код

### 21.

```python
d = {'a': 1, 'b': 2}
d['c'] = 3
d['a'] = 100
print(d)
print(len(d))
```

## **Ответ — вывод:**

```text
{'a': 100, 'b': 2, 'c': 3}
3
```

### 22.

```python
t = (1, 2, 3)
a, b, c = t
print(a)
print(b)
print(c)
```

## **Ответ — вывод:**

```text
1
2
3
```

### 23.

```python
d = {'x': 1, 'y': 2}
keys = list(d.keys())
keys[0] = 'z'
print(d)
print(keys)
```

## **Ответ — вывод:**

```text
{'x': 1, 'y': 2}
['z', 'y']
```

### 24.

```python
def f(d):
    d['new'] = 'value'

data = {'a': 1}
f(data)
print(data)
```

## **Ответ — вывод:**

```text
{'a': 1, 'new': 'value'}
```

### 25.

```python
s = {1, 2, 3}
s.add(2)
s.add(4)
print(s)
print(len(s))
```

## **Ответ — вывод:**

```text
{1, 2, 3, 4}
4
```

### 26.

```python
a = {1, 2, 3}
b = a
a.add(4)
print(b)
print(a is b)
```

## **Ответ — вывод:**

```text
{1, 2, 3, 4}
True
```

### 27.

```python
t = ([1, 2], [3, 4])
t[0].append(99)
print(t)
```

## **Ответ — вывод:**

```text
([1, 2, 99], [3, 4])
```

### 28.

```python
words = ['apple', 'banana', 'apple', 'cherry', 'banana', 'apple']
counts = {}
for w in words:
    counts[w] = counts.get(w, 0) + 1
print(counts)
```

## **Ответ — вывод:**

```text
{'apple': 3, 'banana': 2, 'cherry': 1}
```

## C. Дописать код

### 29. Частотный словарь (4 балла)

**Код с пропусками:**

```python
def count_chars(text):
    """Возвращает словарь: символ → количество вхождений. Пробелы игнорируются."""
    result = {}
    for ch in text:
        if ch == ' ':
            ???                          # (1) пропустить пробел
        result[ch] = result.??? + 1      # (2) увеличить счётчик
    return ???                           # (3) вернуть словарь

# Пример: count_chars('hello') → {'h': 1, 'e': 1, 'l': 2, 'o': 1}
```

## **Ответ:**

```python
def count_chars(text):
    result = {}
    for ch in text:
        if ch == ' ':
            continue
        result[ch] = result.get(ch, 0) + 1
    return result
```

### 30. Инверсия словаря (4 балла)

**Код с пропусками:**

```python
def invert_dict(d):
    """Меняет местами ключи и значения. Если значений несколько — собирает список ключей."""
    result = {}
    for key, value in d.??? :                # (1) итерация по парам
        if value not in result:
            result[value] = ???              # (2) новый список
        result[value].??? (key)              # (3) добавить ключ
    return result

# Пример: invert_dict({'a': 1, 'b': 2, 'c': 1}) → {1: ['a', 'c'], 2: ['b']}
```

## **Ответ:**

```python
def invert_dict(d):
    result = {}
    for key, value in d.items():
        if value not in result:
            result[value] = []
        result[value].append(key)
    return result
```

### 31. SQLite: безопасное обновление (4 балла)

**Код с пропусками:**

```python
import sqlite3

def update_price(product_id, new_price):
    """Обновляет цену. Возвращает rowcount. При ошибке — rollback и 0."""
    conn = sqlite3.connect('shop.db')
    try:
        cursor = conn.cursor()
        cursor.execute(
            "UPDATE products SET price = ??? WHERE id = ???",   # (1) и (2)
            (new_price, product_id)
        )
        conn.???                                                # (3) фиксация
        return cursor.rowcount
    except sqlite3.Error as e:
        conn.???                                                # (4) откат
        print(f"[DB ERROR] {e}")
        return 0
    finally:
        conn.close()
```

## **Ответ:**

```python
import sqlite3

def update_price(product_id, new_price):
    conn = sqlite3.connect('shop.db')
    try:
        cursor = conn.cursor()
        cursor.execute(
            "UPDATE products SET price = ? WHERE id = ?",
            (new_price, product_id)
        )
        conn.commit()
        return cursor.rowcount
    except sqlite3.Error as e:
        conn.rollback()
        print(f"[DB ERROR] {e}")
        return 0
    finally:
        conn.close()
```

### 32. Flask: маршрут удаления (4 балла)

**Код с пропусками:**

```python
from flask import Flask, render_template, request, redirect, url_for
import sqlite3

app = Flask(__name__)

@app.route('/delete/<int:item_id>', methods=???)          # (1) метод
def delete_item(item_id):
    conn = sqlite3.connect('shop.db')
    try:
        cursor = conn.cursor()
        cursor.execute("DELETE FROM items WHERE id = ?", (item_id,))
        conn.commit()
        affected = cursor.???                              # (2) сколько удалено
    except sqlite3.Error as e:
        conn.rollback()
        affected = 0
    finally:
        conn.close()

    if affected == 0:
        return render_template('index.html', items=[], error='Не найдено')
    return ???                                             # (3) редирект на главную
```

## **Ответ:**

```python
from flask import Flask, render_template, redirect, url_for
import sqlite3

app = Flask(__name__)

@app.route('/delete/<int:item_id>', methods=['POST'])
def delete_item(item_id):
    conn = sqlite3.connect('shop.db')
    try:
        cursor = conn.cursor()
        cursor.execute("DELETE FROM items WHERE id = ?", (item_id,))
        conn.commit()
        affected = cursor.rowcount
    except sqlite3.Error as e:
        conn.rollback()
        affected = 0
    finally:
        conn.close()

    if affected == 0:
        return render_template('index.html', items=[], error='Не найдено')
    return redirect(url_for('index'))
```

### 33. Обработка POST-формы (4 балла)

**Код с пропусками:**

```python
@app.route('/add', methods=['GET', 'POST'])
def add():
    if request.method == 'POST':
        name = request.form.???('name', '').strip()        # (1) чтение поля
        if ???:                                            # (2) проверка «не пусто»
            return render_template('add.html', error='Поле обязательно')

        conn = sqlite3.connect('shop.db')
        try:
            cursor = conn.cursor()
            cursor.execute("INSERT INTO items (name) VALUES (?)", (name,))
            conn.commit()
        except sqlite3.Error as e:
            conn.???                                       # (3) откат
            return render_template('add.html', error=str(e))
        finally:
            conn.close()

        return redirect(???)                               # (4) куда редиректить
    return render_template('add.html')
```

## **Ответ:**

```python
@app.route('/add', methods=['GET', 'POST'])
def add():
    if request.method == 'POST':
        name = request.form.get('name', '').strip()
        if not name:
            return render_template('add.html', error='Поле обязательно')

        conn = sqlite3.connect('shop.db')
        try:
            cursor = conn.cursor()
            cursor.execute("INSERT INTO items (name) VALUES (?)", (name,))
            conn.commit()
        except sqlite3.Error as e:
            conn.rollback()
            return render_template('add.html', error=str(e))
        finally:
            conn.close()

        return redirect(url_for('index'))
    return render_template('add.html')
```

## D. Самостоятельные задачи

### 34. Словари: группировка по первой букве (6 баллов)

**Задание:** Напиши функцию, которая принимает **список слов** и возвращает **словарь**: первая буква → список слов, начинающихся с этой буквы (в порядке появления). **Запрещено** использовать `setdefault()` и `collections.defaultdict` — только ручная проверка `if key in dict`.

## **Ответ:**

```python
def group_by_first_letter(words):
    result = {}
    for word in words:
        first = word[0]
        if first in result:
            result[first].append(word)
        else:
            result[first] = [word]
    return result
```

### 35. Кортежи: подсчёт статистики (6 баллов)

**Задание:** Напиши функцию, которая принимает **список кортежей** `(name, grade)` и возвращает **кортеж из трёх значений**: `(min_grade, max_grade, avg_grade)`. `avg_grade` округли до 2 знаков. Если список пуст — вернуть `(None, None, None)`.

## **Ответ:**

```python
def stats(students):
    if not students:
        return (None, None, None)
    grades = [grade for name, grade in students]
    minimum = min(grades)
    maximum = max(grades)
    average = round(sum(grades) / len(grades), 2)
    return (minimum, maximum, average)
```

### 36. Множества: уникальные слова (6 баллов)

**Задание:** Напиши функцию, которая принимает **строку** и возвращает **список уникальных слов** в порядке их **первого появления** (регистр не важен: приводи к нижнему). **Запрещено** использовать `set()` — только список с проверкой `in`.

## **Ответ:**

```python
def unique_words(text):
    result = []
    for word in text.lower().split():
        if word not in result:
            result.append(word)
    return result
```

### 37. SQLite: полный CRUD для таблицы `books` (10 баллов)

**Задание:** Дана таблица `books` с колонками `id INTEGER PRIMARY KEY`, `title TEXT NOT NULL`, `author TEXT`, `year INTEGER`. Напиши **четыре функции** с полной защитой соединений:

**37.1.** `add_book(title, author, year)` — вставляет книгу. Возвращает `True`/`False` (2 балла).

**37.2.** `get_books_by_author(author)` — возвращает список кортежей `(id, title, year)` для книг указанного автора. При ошибке — пустой список. **Обязательно** `sqlite3.Row` (3 балла).

**37.3.** `update_year(book_id, new_year)` — обновляет год. Возвращает `rowcount` (3 балла).

**37.4.** `delete_old_books(before_year)` — удаляет книги, изданные **до** указанного года. Возвращает количество удалённых (2 балла).

## **Ответ:**

```python
import sqlite3

DB_PATH = 'library.db'

def add_book(title, author, year):
    conn = sqlite3.connect(DB_PATH)
    try:
        conn.execute(
            "INSERT INTO books (title, author, year) VALUES (?, ?, ?)",
            (title, author, year)
        )
        conn.commit()
        return True
    except sqlite3.Error:
        conn.rollback()
        return False
    finally:
        conn.close()

def get_books_by_author(author):
    conn = sqlite3.connect(DB_PATH)
    conn.row_factory = sqlite3.Row
    try:
        rows = conn.execute(
            "SELECT id, title, year FROM books WHERE author = ?",
            (author,)
        ).fetchall()
        return [(row['id'], row['title'], row['year']) for row in rows]
    except sqlite3.Error:
        conn.rollback()
        return []
    finally:
        conn.close()

def update_year(book_id, new_year):
    conn = sqlite3.connect(DB_PATH)
    try:
        cursor = conn.execute(
            "UPDATE books SET year = ? WHERE id = ?",
            (new_year, book_id)
        )
        conn.commit()
        return cursor.rowcount
    except sqlite3.Error:
        conn.rollback()
        return 0
    finally:
        conn.close()

def delete_old_books(before_year):
    conn = sqlite3.connect(DB_PATH)
    try:
        cursor = conn.execute(
            "DELETE FROM books WHERE year < ?",
            (before_year,)
        )
        conn.commit()
        return cursor.rowcount
    except sqlite3.Error:
        conn.rollback()
        return 0
    finally:
        conn.close()
```

### 38. Flask: маршрут «Фильтр по автору» (8 баллов)

**Задание:** Напиши **маршрут** `/books`, который:
- На **GET** с параметром `?author=Толстой` — показывает книги только этого автора.
- На **GET** без параметра — показывает **все** книги.
- Возвращает шаблон `books.html` с переменной `books` (список кортежей `(id, title, author, year)`).
- При ошибке БД — `rollback` (если применимо) и возврат шаблона с `error`.

## **Ответ:**

```python
from flask import Flask, render_template, request
import sqlite3

app = Flask(__name__)
DB_PATH = 'library.db'

@app.route('/books')
def books():
    author = request.args.get('author')
    conn = sqlite3.connect(DB_PATH)
    try:
        if author is None:
            rows = conn.execute(
                "SELECT id, title, author, year FROM books"
            ).fetchall()
        else:
            rows = conn.execute(
                "SELECT id, title, author, year FROM books WHERE author = ?",
                (author,)
            ).fetchall()
    except sqlite3.Error as e:
        conn.rollback()
        return render_template('books.html', books=[], error=str(e))
    finally:
        conn.close()
    return render_template('books.html', books=rows)
```

### 39. Комплексная задача: «Топ-N авторов по количеству книг» (8 баллов)

**Задание:** Напиши **функцию** `top_authors(books, n)`, которая принимает **список кортежей** `(title, author)` и число `n`, и возвращает **список из n имён авторов** с наибольшим количеством книг. При равном количестве — сортировка по алфавиту (по возрастанию). Если авторов меньше `n` — вернуть всех.

**Запрещено** использовать `sorted()` и `.sort()` с `key=lambda`. Разрешён ручной подсчёт частот через словарь и ручная сортировка «пузырьком» или вставками.

## **Ответ:**

```python
def top_authors(books, n):
    counts = {}
    for title, author in books:
        counts[author] = counts.get(author, 0) + 1

    authors = list(counts)
    for i in range(len(authors)):
        for j in range(0, len(authors) - i - 1):
            left = authors[j]
            right = authors[j + 1]
            if (counts[left] < counts[right]
                    or (counts[left] == counts[right] and left > right)):
                authors[j], authors[j + 1] = authors[j + 1], authors[j]
    return authors[:max(0, n)]
```
