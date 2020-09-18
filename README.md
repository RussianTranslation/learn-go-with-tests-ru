# Изучение Go через Тестирование

<p align="center">
  <img src="red-green-blue-gophers-smaller.png" />
</p>

[Art by Denise](https://twitter.com/deniseyu21)

[![Build Status](https://travis-ci.org/quii/learn-go-with-tests.svg?branch=main)](https://travis-ci.org/quii/learn-go-with-tests)
[![Go Report Card](https://goreportcard.com/badge/github.com/quii/learn-go-with-tests)](https://goreportcard.com/report/github.com/quii/learn-go-with-tests)

## Где читать

- [Gitbook](https://quii.gitbook.io/learn-go-with-tests)
- [EPUB или PDF](https://github.com/quii/learn-go-with-tests/releases)

## Переводы

- [English](https://github.com/quii/learn-go-with-tests)
- [中文](https://studygolang.gitbook.io/learn-go-with-tests)
- [Português](https://larien.gitbook.io/aprenda-go-com-testes/)
- [日本語](https://andmorefine.gitbook.io/learn-go-with-tests/)

[Поблагодарить автора :coffee:](https://www.buymeacoffee.com/quii)!

## Почему

* Изучение языка программирования Go посредством написания тестов
* **Освоение TDD**. Go - прекрасный язык программирования, чтобы изучить TDD,  так как он (Go) легкий в изучении, а тестирование встроено в сам язык
* Будьте уверены, что вы сможете начать писать надежные, хорошо тестируемые системы на Go
* [Посмотрите видео или прочитайте, почему unit-тестирование и TDD важны](why.md)

## Содержание

### Основы Go

1. [Установка Go](install-go.md) - Настройка рабочего окружени.
2. [Hello, world](hello-world.md) - Объявление переменных, констант, if/else операторы, switch оператор, написание первой Go-программы и написание первого теста. Синтаксис субтестов и замыканий.
3. [Целые числа](integers.md) - Продолжение изучения синтаксиса объявления функций и изучение новых способов документирования Вашего кода.
4. [Циклы](iteration.md) - Изучение цикла `for` и бенчмаркинга.
5. [Массивы и слайсы](arrays-and-slices.md) - Изучение массивов, слайсов, `len`, параметров функций, `range` и покрытие кода тестами.
6. [Структуры, методы и интерфейсы](structs-methods-and-interfaces.md) - Изучение `struct`, методов, `interface` и табличных unit-тестов (table driven tests).
7. [Указатели и ошибки (errors)](pointers-and-errors.md) - Изучение указателей и ошибок (errors).
8. [Мапы (карты)](maps.md) - Узнайте, как хранить значения в структуре данных `map`.
9. [Внедрение зависимостей (DI)](dependency-injection.md) - Изучение внедрения зависимостей (dependency injection), как оно связано с интерфейсами и пример пакета io (input/output).
10. [Мокинг (mocking)](mocking.md) - Возьмем существующий нетестируемый код и применим DI с мокингом для его тестирования.
11. [Многопоточность (concurrency)](concurrency.md) - Узнайте, как писать многопоточный код для ускорения программного обеспечения.
12. [Оператор `select`](select.md) - Узнайте, как элегантно синхронизировать асинхронные процессы.
13. [Рефлексия (reflection)](reflection.md) - Изучение рефлексии (reflection)
13. [Пакет `sync`](sync.md) - Изучение некоторых функций пакета `sync`, включая `WaitGroup` и `Mutex`
13. [Пакет `context`](context.md) - Использование пакета `context` для управления и завершения длительных процессов
14. [Введение в тесты на основе свойств](roman-numerals.md) - Практика TDD над упражнением с римскими цифрами и краткое описание тестов на основе свойств
15. [Пакет `math`](math.md) - Применение пакета `math` чтобы нарисовать SVG-часы

### Создание приложения

Теперь, после успешного изучения раздела _Основы Go_, у вас есть уверенные знания основных возможностей Go и как тестировать через TDD.

Данный раздел демонстрирует создание приложения.

Каждая глава будет повторять предыдущую, расширяя функциональность приложения, как того требует наш владелец продукта.

Будут представлены новые концепции, которые помогут облегчить написание отличного кода, но большая часть нового материала будет посвящена изучению того, что можно сделать из стандартной библиотеки Go.

К концу этого раздела вы будете понимать, как итеративно писать приложение на Go, опираясь на тесты.

* [HTTP-сервер](http-server.md) - Мы создадим приложение, которое слушает HTTP-запросы и отвечает на них.
* [JSON, роутинг и встраивание](json.md) - Мы заставим наши конечные точки (endpoints) возвращать JSON и узнаем, как создавать маршрутизацию (роутинг).
* [IO и сортировка](io.md) - Мы будем сохранять и читать наши данные с диска, а также рассмотрим сортировку данных.
* [Командная строка и структура проекта](command-line.md) - Поддержка нескольких приложений из одной кодовой базы и чтение ввода из командной строки.
* [Время](time.md) - Использование пакета `time` для создание расписания.
* [Вебсокеты (webSockets)](websockets.md) - как написать и протестировать сервер, использующий вебсокеты (webSockets).

### Вопросы и ответы

Я часто сталкиваюсь с вопросами в интернете, например:

> Как мне протестировать мою суперскую функцию, которая делает x, y и z

Если у вас похожий вопрос, создайте issue на github, и я постараюсь найти время, чтобы написать короткую главу, чтобы найти решение этой проблемы. Мне кажется, что подобный контент ценен, поскольку он решает _реальные_ вопросы людей по поводу тестирования.

* [OS exec](os-exec.md) - An example of how we can reach out to the OS to execute commands to fetch data and keep our business logic testable/
* [Error types](error-types.md) - Example of creating your own error types to improve your tests and make your code easier to work with.
* [Context-aware Reader](context-aware-reader.md) - Learn how to TDD augmenting `io.Reader` with cancellation. Based on [Context-aware io.Reader for Go](https://pace.dev/blog/2020/02/03/context-aware-ioreader-for-golang-by-mat-ryer)
* [Revisiting HTTP Handlers](http-handlers-revisited.md) - Testing HTTP handlers seems to be the bane of many a developer's existence. This chapter explores the issues around designing handlers correctly.

## Внести вклад

* _Этот проект на стадии разработки_. Если вы хотите внести свой вклад, пожалуйста, свяжитесь с нами.
* Прочитайте руководство [contributing.md](https://github.com/quii/learn-go-with-tests/tree/842f4f24d1f1c20ba3bb23cbc376c7ca6f7ca79a/contributing.md)
* Есть идеи? Создайте issue

## Background

I have some experience introducing Go to development teams and have tried different approaches as to how to grow a team from some people curious about Go into highly effective writers of Go systems.

### What didn't work

#### Read _the_ book

An approach we tried was to take [the blue book](https://www.amazon.co.uk/Programming-Language-Addison-Wesley-Professional-Computing/dp/0134190440) and every week discuss the next chapter along with the exercises.

I love this book but it requires a high level of commitment. The book is very detailed in explaining concepts, which is obviously great but it means that the progress is slow and steady - this is not for everyone.

I found that whilst a small number of people would read chapter X and do the exercises, many people didn't.

#### Решение проблем

Katas are fun but they are usually limited in their scope for learning a language; you're unlikely to use goroutines to solve a kata.

Another problem is when you have varying levels of enthusiasm. Some people just learn way more of the language than others and when demonstrating what they have done end up confusing people with features the others are not familiar with.

This ends up making the learning feel quite _unstructured_ and _ad hoc_.

### What did work

By far the most effective way was by slowly introducing the fundamentals of the language by reading through [go by example](https://gobyexample.com/), exploring them with examples and discussing them as a group. This was a more interactive approach than "read chapter x for homework".

Over time the team gained a solid foundation of the _grammar_ of the language so we could then start to build systems.

This to me seems analogous to practicing scales when trying to learn guitar.

It doesn't matter how artistic you think you are, you are unlikely to write good music without understanding the fundamentals and practicing the mechanics.

### What works for me

When _I_ learn a new programming language I usually start by messing around in a REPL but eventually, I need more structure.

What I like to do is explore concepts and then solidify the ideas with tests. Tests verify the code I write is correct and documents the feature I have learned.

Taking my experience of learning with a group and my own personal way I am going to try and create something that hopefully proves useful to other teams. Learning the fundamentals by writing small tests so that you can then take your existing software design skills and ship some great systems.

## Для кого 

* Люди, заинтересованные в Go.
* Люди, которые уже знают Go, но хотят изучить тестирование через TDD.

## Что вам потребуется

* Компьютер!
* [Установленный Go](https://golang.org/)
* Текстовый редактор
* Некоторый опыт программирования. Понимание таких концепций как: оператор `if`, переменные, функции и т.д.
* Не бояться использовать терминал

## Обратная связь

* Создайте issues/отправьте PRs ([русский репозиторий](https://github.com/ohDaddyPlease/learn-go-with-tests-ru), [оригинальный репозиторий](https://github.com/quii/learn-go-with-tests)) или [твитните автора @quii](https://twitter.com/quii) или напишите переводчику в [telegram](https://t.me.com/sergiusnovikov)

[MIT license](LICENSE.md)

[Logo is by egonelbre](https://github.com/egonelbre) Какая прелесть!
