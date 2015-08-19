---
author:         Денис Шевченко
title:          Template Haskell: знакомство
tags:           TH
description:    Сегодня мы приподнимем завесу тайны и познакомимся с механизмом Template Haskell.
---

Приветствую!

Для многих новичков (включая меня) механизм Template Haskell похож на чёрную магию: вроде бы работает, но *как именно* работает - абсолютно непонятно. Попробуем разобраться.

## Определение

Template Haskell (часто сокращают до TH) - это особое языковое расширение компилятора GHC, реализующее метапрограммирование времени компиляции. Речь идёт о написании специального кода, превращающегося (на этапе компиляции) в некоторый реальный Haskell-код. Многие Haskell-проекты давно используют TH, ведь он был добавлен в GHC уже более 8 лет назад.







