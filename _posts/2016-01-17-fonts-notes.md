---
layout: post
title:  "Заметки о шрифтах"
date:   2016-01-17
categories: frontend
---
За&nbsp;последний год вышло много инструментов и&nbsp;новых способов работы с&nbsp;веб-шрифтами. В&nbsp;качестве краткой справки и&nbsp;подведения итогов я&nbsp;решил написать эту небольшую заметку.

Вот мой топ-5&nbsp;шрифтов:

1. [Open Sans](https://www.google.com/fonts/specimen/Open+Sans)&nbsp;&mdash; самый популярный бесплатный шрифт, подключается с&nbsp;google fonts.
2. [Lato](https://www.google.com/fonts/specimen/Lato)&nbsp;&mdash; еще один отличный бесплатный шрифт, используется в&nbsp;slack..
3. [Proxima Nova](https://typekit.com/fonts/proxima-nova)&nbsp;&mdash; платный, но&nbsp;достойный шрифт, в&nbsp;котором хорошо проработаны все языки, в&nbsp;том числе и&nbsp;тайский.
4. [Circular](http://lineto.com/The+Fonts/Font+Categories/Text+Fonts/Circular/)&nbsp;&mdash; этот шрифт приобрел популярность после того, как стал использоваться в&nbsp;Airbnb и&nbsp;Spotify.
5. [Futura](https://typekit.com/fonts/futura-pt)&nbsp;&mdash; очень старый и&nbsp;популярный геометрический шрифт без засечек. Подключить можно с&nbsp;typekit.

По&nbsp;поводу подключения шрифтов можно почитать статью на&nbsp;хабре&nbsp;&mdash; [Использование веб-шрифтов, самый лучший способ (на&nbsp;2015 год)](http://habrahabr.ru/company/paysto/blog/268771/).

Если вкратце:

* Используйте [Font Face Observer](https://www.npmjs.com/package/font-face-observer).
* Подбирайте наиболее подходящий переходный шрифт.
* Используйте `<link rel="preload" href="FiraSans-Regular.woff">` для предзагрузки woff шрифтов.
* Кешируйте шрифты в&nbsp;localStorage для повторно зашедших пользователей.

Сейчас также набирает популярность использование системных шрифтов. При их&nbsp;применении на&nbsp;Android будет использоваться Roboto, на&nbsp;Mac и&nbsp;iOS&nbsp;&mdash; San Francisco, Segoe UI&nbsp;&mdash; на&nbsp;Windows и&nbsp;фиг знает что&nbsp;&mdash; на&nbsp;Linux. Это позволяет добиться наилучшего отображения текста и&nbsp;нулевой задержки загрузки шрифта. О&nbsp;способах использования системных шрифтов есть статья на&nbsp;medium&nbsp;&mdash; [How To&nbsp;Use System Typefaces In&nbsp;Web Projects](https://medium.com/mysmartprice-design/how-to-use-system-typefaces-in-web-projects-55e699d52fe6#.dd5865q8l). Также по&nbsp;этому поводу Marcin Wichary(Design lead &amp;&nbsp;typographer at&nbsp;Medium) написал интересную статью с&nbsp;громким названием [System shock](https://medium.com/designing-medium/system-shock-6b1dc6d6596f#.6u3gprtkn).

P.S. Под конец рекомендую почитать статью Юрия Матюхина&nbsp;по [управлению поведением font-face в&nbsp;CSS](https://ymatuhin.ru/front-end/loading-font-face-css/)
