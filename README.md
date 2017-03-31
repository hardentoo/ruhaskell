[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/ruHaskell/forall)

ruHaskell
=========

Сайт русскоязычного сообщества Haskell-разработчиков.

### Цель

Мы уверены, что каждому Haskell-энтузиасту есть что рассказать коллегам, но наши блоги разбросаны по просторам интернета, а кроме того, не всем хочется строить собственное блоговое пространство. Поэтому наш сайт представляет собой единое место обмена опытом, где каждый сможет рассказать обо всём, так или иначе связанном с разработкой на Haskell.

### Темы

Принимаются материалы, имеющие прямое или косвенное отношение к Haskell. Это может быть что угодно:

- Разжёвывание фундаментальной теории, о каких-нибудь категориях и иже с ними.
- Рассмотрение любых аспектов языка, от Hello World до свободных монад и трансформерных ужасов.
- Рассказ об инструментах, связанных с Haskell.
- Готовые практические рецепты. Что называется, копи-паст - и вперёд!
- Истории успеха или неудачи, связанные с практической разработкой на Haskell.
- Пиар программного решения, реализованного с помощью Haskell.

Причём технический уровень статей может быть рассчитан на любых читателей, от зелёных новичков до экспертов.

### Авторам

Статьи принимаются в формате `Markdown`, рекомендуется использовать расширение `.md`.

#### Информация о статье

В начале каждой статьи должен присутствовать информационный блок следующего вида:

```
---
author:         Денис Шевченко
title:          Yesod: знакомство
tags:           Yesod, веб
description:    Yesod - это мощный веб-фреймворк, написанный на языке Haskell.
---
```

где:

- `author` - имя автора статьи,
- `title` - название статьи,
- `tags` - один или более тематических тегов, перечисленных через запятую,
- `description` - краткое описание статьи, необходимое для обновлений в RSS.

Кроме того, существует опциональное поле `hrefToOriginal`. Если оригинал публикуемой вами статьи находится на стороннем ресурсе, просто допишите поле `hrefToOriginal` к вышеупомянутым полям:

```
hrefToOriginal: https://www.fpcomplete.com/user/astynax/basics/pine-tree
```

В результате этого в верхней правой части статьи будет размещена ссылка на оригинал.

**Внимание!** Если автором оригинала публикуемой вами статьи являетесь _не вы_ - убедитесь в том, что автор согласен на публикацию его статьи в рамках нашего ресурса.

#### Правила именования

Имя файла статьи должно быть сформировано следующим образом:

```
гггг-мм-дд-краткое-имя-статьи.md
```

Например:

```
2014-12-27-yesod-raw-deploy.md
```

URL этой статьи станет таким:

```
/posts/2014/12/27/yesod-raw-deploy.html
```

Это позволит отфильтровать статьи по дате публикации. Причём если номер месяца или дня меньше 10, то его необходимо начинать с `0`. Например, публикация от 1 мая должна быть названа так:

```
2014-05-01-yesod-raw-deploy.md
```

#### Расположение

Все Markdown-статьи хранятся в ветке `master`. Иерархически они располагаются в каталоге `posts`, но не в корне, а обязательно в своём тематическом подкаталоге. Имя подкаталога соответствует названию категории. Например, все статьи из категории `web` располагаются в каталоге `posts/web/`. Разумеется, поскольку имя каталога участвует в формировании базового URL статьи, оно должно быть английским.

Посколько Git не любит пустые каталоги, тематические подкаталоги будут создаваться по мере написания статей.

### Локальная сборка

Вы можете собрать сайт у себя:

```bash
$ git clone git@github.com:ruHaskell/ruhaskell.git
$ cd ruhaskell
$ stack setup
$ ./just_build.sh
```

После этого откройте в браузере страницу `_site/index.html`.

Для удобства можно запустить скрипт `watch.sh`, при изменении постов
сайт будет собираться автоматически. Если у вас установлен Firefox
с расширением [MozRepl](https://github.com/bard/mozrepl/wiki),
также будет обновляться вкладка с локальной версией сайта:

```bash
$ ./watch.sh
```

### Устав нашего монастыря

Запрещены:

1. **оскорбления в любой форме**,
2. **явный оффтоп**,
3. **спам**.

Статьи и/или комментарии, содержащие первое, второе и/или третье, будут удалены.

### Обратная связь

Вопросы? Предложения? Критика? Стучитесь в наш [чат](https://gitter.im/ruHaskell/forall) или пишите [Юрию Сыровецкому](mailto:cblp@cblp.su) и [Денису Шевченко](mailto:me@dshevchenko.biz).
