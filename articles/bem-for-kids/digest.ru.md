# Дайджест новостей по БЭМ. Выпуск №11.

Кто летом не сидел без дела, тот мы! Итоги работы нашей команды за три летних месяца: 

* [Новости библиотек](#Новости-библиотек)
* [Новости технологий](#Новости-технологий)
* [Новости инструментов](#Новости-инструментов)
* [Новости БЭМ из мира React](#Новости-БЭМ-из-мира-react)
* [Новости документации](#Новости-документации)
* [Новости мероприятий и сообщества](#Новости-мероприятий-и-сообщества)


## Новости библиотек

### bem-core

Выпустили минорную версию [v4.2.1](https://github.com/bem/bem-core/tree/v4.2.1). 

Исправлено: 

* Ошибка с инвалидацией кеша элементов при изменении DOM.
* Ошибка в `i-bem-dom__events`, приводившая к тому, что данные события не передавались в обработчик.
* Метод `isEditable` модуля `dom`. Добавлены недостающие типы.

Изменения, вошедшие в релиз:

* Синтаксические изменения в JSDoc блока `i-bem-dom`.
* Незначительная доработка документации.
* Добавление [CLA](https://github.com/bem/bem-core/blob/v4/CLA.md)(Contributor License Agreement).

Подробности в [CHANGELOG](https://github.com/bem/bem-core/blob/v4.2.1/CHANGELOG.ru.md#421). 

### bem-components

Выпустили минорную версию [v6.0.1](https://github.com/bem/bem-components/tree/v6.0.1), в которой обновили [bem-core](https://github.com/bem/bem-core/tree/v4.2.1) до версии `4.2.1` и устранили ряд ошибок: 

* Поддержка [bem-xjst 8.x](https://github.com/bem/bem-xjst/releases/tag/v8.6.0): режим `js()` был заменен на `addJs()`.
* В блоке `popup` у молификатора `target_anchor` исправлены вычисления позиции для поддержки новой версии jQuery.
* Исправлена ошибка, при которой не удалялись контролы в `select_mode_radio-check`.

Изменения, вошедшие в релиз:

* Добавление [CLA](https://github.com/bem/bem-core/blob/v4/CLA.md)(Contributor License Agreement).
* Удаление неиспользуемых шаблонов в блоке `attach`. 

Подробности в [CHANGELOG](https://github.com/bem/bem-components/blob/v6.0.1/CHANGELOG.ru.md#601).

## Новости технологий

### bem-xjst
Выпустили релизы [v8.6.12](https://github.com/bem/bem-xjst/releases/tag/v8.6.12) и [v8.6.13](https://github.com/bem/bem-xjst/releases/tag/v8.6.13).

Основные изменения: 


### bemhint-deps-schema
Выпустили новую версию плагина для bemhint — [bemhint-deps-schema 2.1.0](https://www.npmjs.com/package/bemhint-deps-schema), который проверяет, чтобы файлы `*.deps.js` соответствовали спецификации. Теперь `bemhint-deps-schema` умеет обрабатывать не только `.json`-, но и `.js`-файлы с `module.exports`.
 


## Новости инструментов


### borschik
Выпустили мажорную версию borschik [v2.0.0](https://github.com/borschik/borschik/tree/v2.0.0), где заменили [uglify-js](https://www.npmjs.com/package/uglify-js) на [uglify-es](https://www.npmjs.com/package/uglify-es) для поддержки ES6.




## Новости документации

Как и обещали, написали много нового и пересмотрели часть старой документации:

* Большой и полезный туториал по всему БЭМ-стеку: [Переходим на сторону сервера с bem-express](https://habrahabr.ru/company/yandex/blog/337166/) от Сергея Бочарова. Пока опубликовали только на Хабрахабре, но в ближайшем будущем разместим его в нашем разделе [обучающих материалов](https://ru.bem.info/platform/tutorials/).
* Новые документы в разделе [Методология](https://ru.bem.info/method/):  
  * [Уровни переопределения]()  
  * [Способы изменения блока]()  
  * [HTML по БЭМ]()  

* Переработанные и обновенные документы:  
  * [Соглашение по именованию]()
  * [Организация файловой структуры]() 
  * [JS по БЭМ]()  


## Новости мероприятий и сообщества

* Организовали несколько встреч БЭМ-сообщества — BEMup'ов, на которых Сергей Бережной провел мастер-классы по использованию библиотеки [bem-react-core](https://github.com/bem/bem-react-core). Скринкасты со всех встреч можно найти на [Youtube](https://www.youtube.com/channel/UCsHVzqjMO31I8qKHhWHsobg?view_as=subscriber) или по тегу [BEMup + video](https://ru.bem.info/forum/?labels=BEMup%2Cvideo) на форуме bem.info.
* Владимир Гриненко и Сергей Бережной выступили на FullStack Conference с докладом [BEM — The unknown](http://bit.ly/2vLP5Tu).
* Владимир Гриненко рассказал о зависимостях в компонентном вебе на HolyJSconf в Питере. Доклад [Зависимости в компонентном вебе, сделанные правильно](http://bit.ly/2rWWEDY).





## Новости БЭМ из мира React не смотрела

### bem-react-core
Выпустили bem-react-core [v0.4.3](https://github.com/bem/bem-react-core/tree/v0.4.2). В новой версии исправлен баг с потерей контекста для вложенных элементов и ряд других ошибок.

Основные изменения: 
- Рендер без CSS-класса (bem:false). 
- Поддержка [cls](https://github.com/bem/bem-react-core/blob/v0.4.2/REFERENCE.ru.md#cls), [mix](https://github.com/bem/bem-react-core/blob/v0.4.2/REFERENCE.ru.md#mix-addmix). 
- Доопределение статических полей `defaultProps` и `propTypes`. 
- Сокращенный синтаксис декларации модификаторов. 
- Поддержка [HOC](https://facebook.github.io/react/docs/higher-order-components.html) (redux, flux и других оберток). 

Написали подробную документацию – [REFERENCE](https://github.com/bem/bem-react-core/blob/master/REFERENCE.ru.md). 

Провели ряд мероприятий, посвященных bem-react-core:
* Провели вебинар [Немного БЭМ в вашем React](http://bit.ly/2nu7dd1).
* Рассказали на [митапе по БЭМ](https://events.yandex.ru/events/bemup/24-march-2017/). Видео доклада [Новости БЭМ из мира React](https://ru.bem.info/forum/1320/).
* Рассказали на [React Moscow Meetup #2](https://events.yandex.ru/events/yagosti/15-march-2017/).

### bem-react-components
Продолжаем активно развивать [bem-react-components](https://github.com/bem/bem-react-components) — библиотеку блоков для разработки с React по БЭМ-методологии. 

### create-bem-react-app
Продолжаем создавать реактовый проджект стаб [create-bem-react-app](https://github.com/bem/create-bem-react-app), который позволяет одной командой собрать готовое React/БЭМ-приложение с установленными зависимостями и правильной файловой структурой.  

Важный приятный пункт — create-bem-react-app не требует никаких предварительных настроек сборки.

### webpack-bem-loader
* Добавили генератор i18n, который обеспечивает возможность локализации компонентов.
* Появилась возможность конфигурировать каждый уровень сборки отдельно с помощью bem-config.
