# Туториал по основам системы контроля версий GIT

## Основные состояния Git
 Файлы в Git могут находиться в трех основных состояниях: зафиксированном, модифицированном и индексированном.
 В результате Git-проект разбивается на три основные области: папка Git, рабочая папка и область индексирования:
 
 ![Рабочая папка, область индексирования и папка Git](/Picture_1.jpg)

## Инициализация проекта
**Чтобы добавить возможность использовать разные версии файлов, необходимо использовать следующую команду:**

```fix
git init 
```

## Как добавить файл на остлеживание
**Чтобы добавить файл на отслеживание, используйте следующую команду:**

```
git add .
```

## Создание коммита
Чтобы создать коммит, необходимо использовать следующую команду:

```
git commit -m "message"
```
При этом рекомендуется выбирать правильные и содержательные названия изменений, чтобы потом было легче ориентироваться в документе!

## Возврат к актуальному состоянию
После переключения на другую ветку для возварщения к актуальному состоянию и продолжению работы, необходимо использовать команду:

```fix
git checkout master
```

# Инструкция по разметке Markdown

## Исходный код

В чистом Маркдауне блоки кода отбиваются 4 пробелами в начале каждой строки.

Но в GitHub-Flavored Markdown (сокращенно GFM) есть более удобный способ: ставим по три апострофа (на букве Ё) до и после кода. Также можно указать язык исходного кода.

```html
<nav class="nav nav-primary">
    <ul>
        <li class="tab-conversation active">
            <a href="#" data-role="post-count" class="publisher-nav-color" data-nav="conversation">
                <span class="comment-count">0 комментариев</span>
                <span class="comment-count-placeholder">Комментарии</span>
            </a>
        </li>
        <li class="dropdown user-menu" data-role="logout">
            <a href="#" class="dropdown-toggle" data-toggle="dropdown">
                <span class="dropdown-toggle-wrapper">
                    <span>
                        Войти
                    </span>
                </span>
                <span class="caret"></span>
            </a>
        </li>
    </ul>
</nav>
```
Самое приятное, что в коде не нужно заменять угловыескобки `< >` и амперсанд `&` на их html-сущности.
 

## Ссылки

Это встроенная [ссылка на GitHub](https://github.com/). Это — [без title](http://example.com/link).

А вот [пример][1] [нескольких][2] [ссылок][id] с
разметкой как у сносок. Прокатит и [короткая запись][]
без указания id.

[1]: https://ru.wikipedia.org/wiki/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80 "Optional Title Here"
[2]: https://ru.wiktionary.org/wiki/%D0%BD%D0%B5%D1%81%D0%BA%D0%BE%D0%BB%D1%8C%D0%BA%D0%BE
[id]: https://ru.wikipedia.org/wiki/%D0%A1%D1%81%D1%8B%D0%BB%D0%BA%D0%B0_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5) (Optional Title Here)
[короткая запись]: https://ru.wikipedia.org/wiki/%D0%9F%D0%B8%D0%BF%D0%B8%D0%BD_%D0%9A%D0%BE%D1%80%D0%BE%D1%82%D0%BA%D0%B8%D0%B9

Вынос длинных урлов из предложения способствует
сохранению читабельности исходника. Сноски можно
располагать в любом месте документа.

## Изображения

[![Alt text](https://images.unsplash.com/photo-1517649763962-0c623066013b?ixlib=rb-4.0.3ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=870&q=80)](https://unsplash.com/t/athletics)

Картинка без `alt` текста
![](https://images.unsplash.com/photo-1684674096773-1fd8d14677b2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1964&q=80)

Картинка с альтом и тайтлом:
![Alt text](https://images.unsplash.com/photo-1685073129693-ae1c07169e07?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1322&q=80 "Китай-город")

Картинки «сноски»:
![Картинка1][image1]
![Картинка2][image2]

[image1]: bike1.png
[image2]: bike2.png


## Таблицы

Рисование таблиц в Markdown
