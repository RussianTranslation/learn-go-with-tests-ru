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
* [Вебсокеты (WebSockets)](websockets.md) - как написать и протестировать сервер, использующий вебсокеты (webSockets).

### Вопросы и ответы

Я часто сталкиваюсь с вопросами в интернете, например:

> Как мне протестировать мою суперскую функцию, которая делает x, y и z

Если у вас похожий вопрос, создайте issue на github, и я постараюсь найти время, чтобы написать короткую главу, чтобы найти решение этой проблемы. Мне кажется, что подобный контент ценен, поскольку он решает _реальные_ вопросы людей по поводу тестирования.

* [OS exec](os-exec.md) - Пример того, как мы можем обратиться к ОС для выполнения команд для выборки данных и обеспечения тестируемости нашей бизнес-логики.
* [Типы `error`](error-types.md) - Пример создания собственных типов ошибок для улучшения тестирования и упрощения работы с кодом.
* [Контекстно-зависимый Reader](context-aware-reader.md) - Узнайте, как TDD дополняет `io.Reader` с отменой (cancellation). Основывается на [Контекстно-зависимый io.Reader для Go] (https://pace.dev/blog/2020/02/03/context-aware-ioreader-for-golang-by-mat-ryer)
* [Возвращение к HTTP-обработчикам](http-handlers-revisited.md) - Установление HTTP-обработчиков кажется ужасом для многих разработчиков. В этой главе рассматриваются вопросы, связанные с правильным проектированием обработчиков.


## Внести вклад

* _Этот проект на стадии разработки_. Если вы хотите внести свой вклад, пожалуйста, свяжитесь с нами.
* Прочитайте руководство [contributing.md](https://github.com/quii/learn-go-with-tests/tree/842f4f24d1f1c20ba3bb23cbc376c7ca6f7ca79a/contributing.md)
* Есть идеи? Создайте issue

## Истоки

У меня есть некоторый опыт представления Go командам разработчиков, и я пробовал разные подходы к тому, как вырастить команду из людей, интересующихся Go, в высокоэффективных Go разработчиков.

### Что не сработало

#### Чтение _какой-то_ книги

Мы попробовали использовать [синюю книгу] (https://www.amazon.co.uk/Programming-Language-Addison-Wesley-Professional-Computing/dp/0134190440) и каждую неделю обсуждать следующую главу вместе с упражнениями.

Мне нравится эта книга, но она требует большой отдачи. В книге очень подробно объясняются концепции, что, конечно, здорово, но это означает, что прогресс идет медленно и неуклонно - это не для всех.

Я обнаружил, что, хотя небольшое количество людей читало главу X и выполняло упражнения, многие люди этого не делали.

#### Решение проблем

Каты (kata exercises) - это весело, но они обычно ограничены в возможностях изучения языка; вы вряд ли будете использовать горутины для решения каты.

Другая проблема - это когда у вас разный уровень энтузиазма. Некоторые люди просто изучают язык больше, чем другие, и, демонстрируя то, что они сделали и знают, в конечном итоге сбивают людей с толку функциями, с которыми другие не знакомы.

Это приводит к тому, что обучение кажется совершенно _неструктурированным_ и _бесполезным_.

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
