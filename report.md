Отчёт о тестировании KeyValidator
Краткое описание : Проверка, что  инструкция по установке OpenJDK11 работает с  ОС Windows 10 ,приложение запускается и совместимо с Java 11, приложение работает согласно руководству использования
Дата начала 26.10.2020
Дата окончания 26.10.2020 было проведено дымовое тестирование методом черного ящика
На тестирование затрачено: 10 часов

В результате тестирования выявлены следующие дефекты:

https://github.com/saika1968/java1/issues/2
https://github.com/saika1968/java1/issues/1

Описание процесса тестирования
В процессе тестирования использовались следующие артефакты*:
Тест- кейс:
1. открываем инструкцию по установке OpenJDK11 https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md
2. Проверяем совместимость с Windows 10
3. Устанавливаем OpenJDK11
4. Запускаем приложение и командой java - version проверяем совместимость с java11
5. Проверяем работу приложения в соответствии с инструкцией https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md
6. Проверяем валидацию ключей из инструкции https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md

В качестве тестовых данных использовались данные  инструкции https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md

Валидные ключи
8f05e6a7-70e9-33d7-bfe7-b19eae0d8998
80b427f8-92cd-3aae-ba04-3927fbe17c6
b295bc63-9f03-3b4b-af80-969b39f8c262
387eedc6-12e9-3b32-9881-63b6b5e85317
c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180
Ожидаемый результат: Валидация происходит,высвечиватся команда ОК

Невалидные ключи:
18252235-78e0-44a5-8720-556f0c7da17a
e66075b6-ddad-445e-baf6-161b3289522b
b6d53250-f07e-4352-a293-6102ddf7f1ca
c2bc778a-1cb9-46c6-b435-0489649d2a42
2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1
Ожидаемый результат: Валидация  происходит , высвечивается команда FATL

Тестирование производилось в следующем окружении:

Windows 10 64-bit
openjdk version "11.0.9" 2020-10-20
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.9+11)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.9+11, mixed mode)
