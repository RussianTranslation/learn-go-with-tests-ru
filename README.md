# Изучение Go с Тестами

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
* Будьте уверены, что Вы сможете начать писать надежные, хорошо тестируемые системы на Go
* [Посмотрите видео или прочитайте, почему unit-тестирование и TDD важны](why.md)

## Содержание

### Основы Go

1. [Установка Go](install-go.md) - Настройка рабочего окружени.
2. [Hello, world](hello-world.md) - Объявление переменных, констант, if/else операторов, switch, написание первой Go-программы и написание первого теста. Синтаксис субтестов и замыканий.
3. [Целые числа](integers.md) - Продолжение изучения синтаксиса объявления функций и изучение новых способов документирования Вашего кода.
4. [Циклы](iteration.md) - Изучение цикла `for` и бенчмаркинга.
5. [Массивы и слайсы](arrays-and-slices.md) - Изучение массивов, слайсов, `len`, параметров функций, `range` и покрытие кода тестами.
6. [Структуры, методы и интерфейсы](structs-methods-and-interfaces.md) - Изучение `struct`, методов, `interface` и табличных unit-тестов (table driven tests).
7. [Указатели и ошибки (errors)](pointers-and-errors.md) - Изучение указателей и ошибок (errors).
8. [Мапы (карты)](maps.md) - Изучение хранения значений в структуре данных `map`.
9. [Внедрение зависимостей (DI)](dependency-injection.md) - Изучение внедрения зависимостей (dependency injection), как оно связано с интерфейсами и пример io (input/output).
10. [Мокинг (mocking)](mocking.md) - Возьмем существующий нетестируемый код и применим DI с мокингом для его тестирования.
11. [Многопоточность (concurrency)](concurrency.md) - Изучение, как писать многопоточный код для ускорения программного обеспечения.
12. [Оператор `select`](select.md) - Learn how to synchronise asynchronous processes elegantly.
13. [Рефлексия (reflection)](reflection.md) - Изучение рефлексии (reflection)
13. [Пакет `sync`](sync.md) - Learn some functionality from the sync package including `WaitGroup` and `Mutex`
13. [Пакет `context`](context.md) - Use the context package to manage and cancel long-running processes
14. [Intro to property based tests](roman-numerals.md) - Practice some TDD with the Roman Numerals kata and get a brief intro to property based tests
15. [Пакет `math`](math.md) - Use the `math` package to draw an SVG clock

### Build an application

Now that you have hopefully digested the _Go Fundamentals_ section you have a solid grounding of a majority of Go's language features and how to do TDD.

This next section will involve building an application.

Each chapter will iterate on the previous one, expanding the application's functionality as our product owner dictates.

New concepts will be introduced to help facilitate writing great code but most of the new material will be learning what can be accomplished from Go's standard library.

By the end of this, you should have a strong grasp as to how to iteratively write an application in Go, backed by tests.

* [HTTP server](http-server.md) - We will create an application which listens to HTTP requests and responds to them.
* [JSON, routing and embedding](json.md) - We will make our endpoints return JSON and explore how to do routing.
* [IO and sorting](io.md) - We will persist and read our data from disk and we'll cover sorting data.
* [Command line & project structure](command-line.md) - Support multiple applications from one code base and read input from command line.
* [Time](time.md) - using the `time` package to schedule activities.
* [WebSockets](websockets.md) - learn how to write and test a server that uses WebSockets.

### Questions and answers

I often run in to questions on the internets like

> How do I test my amazing function that does x, y and z

If you have such a question raise it as an issue on github and I'll try and find time to write a short chapter to tackle the issue. I feel like content like this is valuable as it is tackling people's _real_ questions around testing.

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

#### Solve some problems

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

## Что Вам потребуется

* Компьютер!
* [Установленный Go](https://golang.org/)
* Текстовый редактор
* Некоторый опыт программирования. Понимание таких концепций как: оператор `if`, переменные, функции и т.д.
* Не бояться использовать терминал

## Обратная связь

* Создайте issues/отправьте PRs ([русский репозиторий](https://github.com/ohDaddyPlease/learn-go-with-tests-ru), [оригинальный репозиторий](https://github.com/quii/learn-go-with-tests)) или [твитните автора @quii](https://twitter.com/quii) или напишите переводчику в [telegram](https://t.me.com/sergiusnovikov)

[MIT license](LICENSE.md)

[Logo is by egonelbre](https://github.com/egonelbre) Какая прелесть!
