# Решатель квадратных уравнений

Скрипт вычисляет корень квадратного уравнения по входящим данным.

# Как использовать

Работу скрипта обеспечивает функция get_roots, которая принимает три аргумента a,b,c и возвращает корни уравнения.

Пример использования:
```python
from quadratic_equation import get_roots


def Calculator():
    print("Введите аргументы уравнения: a,b,c")
    a = int(input())
    b = int(input())
    c = int(input())
    root1, root2 = get_roots(a, b, c)
    if root1 == None and root2 == None:
        print("Уравнение не имеет корней")
    elif root2 == None:
        print("Корень уравнения равен: %d" % root1)
    else:
        print("Корни уравнения x1 = %s, x2 = %s " % (root1, root2))
```
# Как запустить

Скрипт требует для своей работы установленного интерпретатора Python версии 3.5

Запуск на Linux:

```bash
python tests.py # может понадобиться вызов python3 вместо python, зависит от настроек операционной системы
```

Запуск на Windows происходит аналогично.

# Цели проекта

Код создан в учебных целях. В рамках учебного курса по веб-разработке ― [DEVMAN.org](https://devman.org)
