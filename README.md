# PureScript
Functional programming language

## 1. Типы данных и переменные
### 1.1. Типы данных
+ числа
+ булевые значения: true (1) - истина, false (0) - ложь
+ строки: "Hello world", "99", "Hi!" (строки обязательно должны оборачиваться кавычками, иначе будут интерпретированы как функции или переменные
### 1.2. Переменные
Возможно создание как неименованных, так и именнованых переменных. Создание именнованой переменной: (let <название переменной> <значение переменной>). Пример: 
```
(let per 56) # создание переменной с именем per, хранящей числовое значение, равное 56
(let line "Hello") # создание переменной с именем per, хранящей строковое значение "Hello"
```

## 2. Операторы языка
### 2.1. Базовые операторы
#### Арифметические операторы:
+ "+" (сложение) - суммирует два числа
+ "-" (вычитание) - даёт разность двух чисел
+ "*" (умножение) - даёт произведение двух чисел 
+ "/" (деление) - возвращает частное от деления числа x на y 

Примеры:
```
(+ 2 5) # Result: Number 7.0
(- 2 5) # Result: Number -3.0
(* 2 5) # Result: Number 10.0
(/ 2 5) # Result: Number 0.4
``` 
#### Операторы сравнения:
+ "<" (меньше) - определяет, верно ли, что число x меньше y. Возвращает true или false.
+ ">" (больше) - определяет, верно ли, что число x больше y. Возвращает true или false.
+ "=" (равно) - проверяет, одинаковы ли объекты. Возвращает true или false.

Примеры:
```
(< 2 5) # Result: Bool true
(> 2 5) # Result: Bool false
(= 2 5) # Result: Bool false
(= true true) # Result: Bool true
(= "st" "tr") # Result: Bool false
``` 
#### Булевые выражения:
+ "&" (И) - логический оператор AND 
+ "l" (ИЛИ) - логический оператор OR

Примеры:
```
(& false false) # Result: Bool false
(& 1 0) # Result: Bool false
(l 1 0) # Result: Bool true
(& (& 1 0) (l false true)) # Result: Bool false
```

### 2.2. Управляющие операторы
#### Условные операторы (if-then/else):
Оператор if используется для проверки условий: если условие верно, выполняется блок выражений (“if-условие-then-блок”), иначе выполняется другой блок выражений (“else-блок”). Блок “else” является необязательным.

Пример использования оператора:
```
(if (= 5 7) then "true" else "false") # Result: String "false"
(if (< -5 -1) then "true") # Result: String "true"
(if (> -5 -1) then "true") # Result: Keys ""
```
