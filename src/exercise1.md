**Классы эквивалентности и граничные значения**
>  Если допустимыми значениями являются целые числа от 1 до 100 включительно, то разделяем три класса эквивалентности:
>
    - меньше 1
    - от 1 до 100 
    - больше 100

Граничными значениями для этих классов являются "1" и "100",
также важно проверить, как система будет обрабатывать недопустимые значения, которые могут быть введены пользователем:
>
    - отрицательные числа 
    - нецелые числа
    - символы и/или буквы
 
Итого получается 10 проверок:
1.  Отрицательное число
2.  0
3.  1
4.  2
5.  нецелое число
6.  99
7.  100
8.  101
9.  Символы №;:??()*)_*, также пробел (любое числовое значение, отрицательное, нецелое и т. п. содержащие символы будет являться недопустимым).
10. Буквы, также пробел (любое числовое значение, отрицательное, нецелое и т. п. содержащае буквы будет являться недопустимым).
>  На примере, выполняется один из способов, когда мы проверяем не два, а три значения на границе:
- граничное значение,
- значение перед границей,
- значение после границы.
>  Берется 3 значения (добавляем значение, при котором условие продолжает выполняться), при втором подходе (когда получается больше проверок) вероятность пропуска бага (ошибки) ниже.
Второй способ, это когда мы проверяем 2 значения на верхней и нижней границах класса эквивалентности:
1.  При котором еще действует старое условие
2.  При котором уже действует новое условие.
>  Обычно выбор способа определения граничных значений осуществляется тестировщиком на основе различных факторов, таких как время на проверку, опыт обнаружения подобных багов и структура кода. 
Однако, для минимально необходимых проверок, мы можем использовать второй способ и исключить тесты 2 и 99, при которых условие продолжает выполняться. Таким образом, остаются 8 проверок.
___
**Тест-кейс №1 - проверка на отрицательные числа**
1. Предусловия:
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "-1"
-  нажать на кнопку "ок"
3. Ожидаемый результат:
-  ошибка авторизации
___
**Тест-кейс №2 - проверка на числа меньше "1"**
1. Предусловия:
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "0"
-  нажать на кнопку "ок"
3. Ожидаемый результат:
-  ошибка авторизации
___
**Тест-кейс №3 - проверка граничного числа "1"**
1. Предусловия:
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "1"
-  нажать на кнопку "ок"
3. Ожидаемый результат:
-  авторизация прошла успешно
___
**Тест-кейс №4 - проверка на нецелое число от 1 до 100**
1. Предусловия:
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "1.5"
-  нажать на кнопку "ок"
3. Ожидаемий результат:
-  ошибка авторизации
___
**Тест-кейс №5 - проверке граничного числа "100"**
1. Предусловия: 
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "100"
-  нажать на кнопку “ок"
3. Ожидаемый результат: 
-  авторизация прошла успешно
___
**Тест-кейс №6 - проверка на числа больше 100**
1. Предусловия: 
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "101"
-  нажать на кнопку "ок"
3. Ожидаемый результат:
-  ошибка авторизации
___
**Тест-кейс №7 - проверка на специальные символы**
1. Предусловия:
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "№"
-  нажать на кнопку "ок"
-  ввести в поле ввода значение “_"
-  нажать на кнопку “ок"
3. Ожидаемый результат:
-  ошибка авторизации
___
**Тест-кейс №8 - проверка на буквы**
1. Предусловия:
-  открыто поле ввода возраста
2. Шаги:
-  ввести в поле ввода значение "L"
-  нажать на кнопку "ок"
-  ввести в поле ввода значение "М"
-  нажать на кнопку "ок"
3. Ожидаемый результат:
-  ошибка авторизации 