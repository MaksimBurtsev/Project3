>Для удобства подсчета пар я использовал интернет-ресурс предназначенный для генерации пар https://pairwise.teremokgames.com
___
|login|Password|
|:-:|:-:|
|Пустое|Пустое|
|Неверное значение|Неверное значение|
|standard_user|secret_sauce|
|locked_out_user||
|problem_user||
|standard_user||
| performance_glitch_user||
___
>После введения заданных параметров, были сгенерированы следующие пары
___
|login|Password|
|:-:|:-:|
|Пустое|Пустое|
|Пустое|Неверное значение|
|Пустое|secret_sauce|
|Неверное значение|Неверное значение|
|Неверное значение|secret_sauce|
|неверное значение|Пустое|
|standard_user|secret_sauce|
|standard_user|Пустое|
|standard_user|неверное значение|
|locked_out_user|Пустое|
|locked_out_user|Неверное значение|
|loc ked_out_user|secret_sauce| 
|problem_user|Неверное значение|
|problem_user|secret_sauce|
|problem_user|Пустое|
|performance_glitch_user|secret_sauce|
|performance_glitch_user|Пустое|
|performance_glitch_user|Неверное значение|
___
**Тест-кейс №1 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ничего не вводить
    -   В поле "Password" ничего не вводить
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации: "Username is required"
___
**Тест-кейс №2 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ничего не вводить 
    -   В поле "Password" ввести неверное значение
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации "Username is required"
___
**Тест-кейс №3 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ничего не вводить
    -   В поле "Password" ввести "secret_sauce"
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации “Username is required"
___
**Тест-кейс №4 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.соm/
2.  Шаги:
    -   В поле "Username" ввести неверное значение
    -   В поле "Password" ничего не вводить
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации "Password is required"
___
**Тест-кейс №5 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.соm/
2.  Шаги:
    -   В поле "Username" ввести неверное значение
    -   В поле "Password" ввести неверное значение
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации "Username and password do not match any user in this service"
____

**Тест-кейс №6 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://ww.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести неверное значение
    -   В поле "Password" ввести "secret_sauce"
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации "Username and password do not match any user in this service"
___
**Тест-кейс №7 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "standarduser"
    -   В поле "Password" ничего не вводить
    -   Нажать на кнопку "Login"
3.  Ожидаемыйй результат:
    -   Ошибка авторизации "Password is required"
___
**Тест-кейс №8 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести “standard_user"
    -   В поле "Password" ввести неверное значение
    -   Нажать кнопку "Login"
3.  Ожидаемый на результат:
    -   Ошибка авторизации "Username and password do not match any user in this service"
___
**Тест-кеис №9 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести ”standard_user"
    -   В в поле "Password” ввести "secret_sauce" 
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Авторизация прошла успешно, пользователь попадает на главную страницу сайта
___
**Тест-кейс №10 - проверка авторизации**
1.  Предусловие: 
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "locked_out_user"
    -   В поле "Password" ничего не вводить 
    -   Нажать на кнопку "Login”
3.  Ожидаемый результат:
    -   Ошибка авторизации "Password is required"
___
**Тест-кейс №11 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "locked_out_user“
    -   В поле "Password" ввести неверное значение 
    -   Нажать на кнопку "Login”
3.  Ожидаемый результат:
    -   Ошибка авторизации "Username and password do not match any user in this serviceЭ
___
**Тест-кейс №12 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "locked_out_user" 
    -   В поле "Password" ввести "secret_sauce"
    -   Нажать кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации "Sorry, this user has been locked out"
___
**Тест-кейс №13 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "problem_user"
    -   В поле "Password" ничего не вводить"
    -   Нажать кнопку "Login
3.  Ожидаемый результат:
    -   Ошибка авторизации “Password is required""
___
**Тест-кейс №14 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле “username" ввести "problem_user"
    -   В поле "Password" ввести неверное значение 
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Ошибка авторизации "Username and password do not match any user in this service"
___
**Тест-кейс №15 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести “problem_user”
    -   В поле "Password" ввести "secret_sauce"
    -   Нажать кнопку “Login"
3.  Ожидаемый результат:
    -   Авторизация прошла успешно, пользователь попадает на главную страницу сайта
___
**Тест-кейс №1б - проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "performance_glitch_user"
    -   В поле "Password" ничего не вводить
    -   Нажать на кнопку “Login”
3.  Ожидаемый результат:
    -   Ошибка авторизации “Password is required"
___
**Тест-кейс №17 - проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.com/
2.  Шаги:
    -   В поле "Username" ввести "performance_glitch_user"
    -   В поле "Password" ввести неверное значение 
    -   Нажать на кнопку "Login”
3.  Ожидаемый результат:
    -   Ошибка авторизации "Username and password do not match any user in this service"
___
**Тест-кейс №18 - Проверка авторизации**
1.  Предусловие:
    -   открыта страница авторизации https://www.saucedemo.соm/
2.  Шаги:
    -   В поле "Username" ввести "performance_glitch_user" 
    -   В поле "Password" ввести "secret_sauce" 
    -   Нажать на кнопку "Login"
3.  Ожидаемый результат:
    -   Авторизация прошла успешно, пользователь попадает на главную страницу сайта

