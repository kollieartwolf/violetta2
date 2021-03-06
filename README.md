# violetta2

Транслятор с Python на русский псевдоязык и обратно. Делает программирование более доступным для людей с плохим восприятием английского.

Python подходит для обучения детей по нескольким причинам: 

1. Python - очень простой язык, на котором просто программировать
2. Python 3 поддерживает символы Unicode в названиях переменных
2. Python - интерпретируемый язык, что делает его запуск удобнее.

Для облегчения понимания логики языка violetta2 переводит основные английские ключевые слова и методы на русский, что облегчает читабельность кода для тех, кто не владеет английским в должной степени.

## Пример работы

Код на Python:

```
def Split2(A):
    B = list()
    C = list()
    for el in A:
        if el % 2 == 0:
            B.append(el)
        else:
            C.append(el)
    return B, C

A = list(map(int, input('Введите элементы массива через пробел: ').split()))

B, C = Split2(A)
print(B, len(B))
print(C, len(C))
```

Код на Violetta2:

```
задать Split2(A):
    B = список()
    C = список()
    для el в A:
        если el % 2 == 0:
            B.дополнить(el)
        иначе:
            C.дополнить(el)
    вернуть B, C

A = список(карта(целое, ввести('Введите элементы массива через пробел: ').разделить()))

B, C = Split2(A)
вывести(B, длина(B))
вывести(C, длина(C))
```

Можно дополнить перевод:

```
задать Разделить(Числа):
    Чётные = список()
    Нечётные = список()
    для элемент в Числа:
        если элемент % 2 == 0:
            Чётные.дополнить(элемент)
        иначе:
            Нечётные.дополнить(элемент)
    вернуть Чётные, Нечётные

Числа = список(карта(целое, ввести('Введите элементы массива через пробел: ').разделить()))

Чётные, Нечётные = Разделить(Числа)
вывести(Чётные, длина(Чётные))
вывести(Нечётные, длина(Нечётные))
```

## Использование

`$ python -m vio2 -v <filename>` - перевести файл с Python на Violetta2  
`$ python -m vio2 -p <filename>` - перевести файл с Violetta2 на Python  
`$ python -m vio2` - режим интерактивной оболочки

### Установка

`pip install vio2`

### Зависимости и требования

Зависимостей нет. Требование к версии Python: >=3.8.
