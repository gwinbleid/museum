## museum

**Ваша задача** – сверстать landing page Лувра – одного из крупнейших и наиболее популярных художественных музеев мира.

## Ключевые навыки:
- валидная семантическая вёрстка
- легкоподдерживаемый читаемый код
- экспорт стилей и графики из Figma
- работа с растровой и векторной графикой
- подключение шрифтов
- использование flexbox для построения сеток
- вёрстка навигационных элементов интерфейса
- вёрстка карточных элементов интерфейса
- вёрстка и стилизация интерактивных элементов интерфейса (кнопки, ссылки, переключатели)

## Работа над проектом:
В ходе основного этапа в вёрстку вносятся изменения и дополнения, добавляется адаптивность, реализуется создаваемая при помощи JavaScript интерактивность.

Благодаря этому, если вы приступили к выполнению задания на этапе stage0, ваша работа будет включать в себя весь цикл разработки: создание проекта, его поддержка и доработка.

<kbd>[![screenshot](./images/museum-prev.jpg)](https://raw.githubusercontent.com/rolling-scopes-school/tasks/master/tasks/images/museum.jpg)</kbd>

[Макет Museum](https://www.figma.com/file/7dI6mXBFTdTvXxuhZZTt5h/Museum)  
[Советы по выполнению задания](museum-hints.md)  
<!-- [Видео с обзором задания](https://youtu.be/OF9zQ0jRx4E)   -->
[Используемые в макете ссылки](https://github.com/rolling-scopes-school/stage1-tasks/blob/museum/README.md)

## Создание собственной копии макета:
- авторизуемся в Фигме
- открываем макет
- нажимаем на стрелку рядом с названием макета на панели вверху, выбираем пункт "Duplicate to your drafts"
- слева вверху открываем настройки, выбираем "Back to files"
- открываем копию макета рядом с которой есть надпись "In Drafts"

## Структура макета:
- Макет состоит из трёх блоков: `<header>`, `<main>`, `<footer>`
- Блок `<main>` состоит из шести секций `<section>`:
  - `Welcome`
  - `Visiting`
  - `Explore`
  - `Video`
  - `Tickets`
  - `Contacts`

## Интерактивность, реализуемая через css
1. Плавная прокрутка по якорям
2. Изменение стиля интерактивных элементов при наведении и при клике

## Технические требования
1. легкоподдерживаемый читаемый качественный код:
   - при написании кода следуйте гайдлайну https://codeguide.academy/html-css.html
2. вёрстка валидная, семантическая, соответствующая макету
3. приложение корректно отображается и работает в браузере Google Chrome последней версии
4. запрещается использование CSS-фреймворков (bootstrap)
5. допускается использование CSS-препроцессоров (Sass), normalize.css

## Требования к коммитам
- История коммитов должна отображать процесс разработки приложения.
- [Названия коммитов дайте согласно гайдлайну](https://docs.rs.school/#/git-convention)

## Требования к Pull Request
- Название Pull Request дайте по названию задания
- [Описание Pull Request дайте по схеме](https://docs.rs.school/#/pull-request-review-process?id=Требования-к-pull-request-pr)
  **Мержить Pull Request не нужно**.

## Критерии оценки

1. Вёрстка валидная
   - для проверки валидности вёрстки используйте сервис https://validator.w3.org/  
     Валидной вёрстке соответствует надпись "Document checking completed. No errors or warnings to show."
2. Вёрстка семантическая
   - в коде странице присутствуют следующие элементы (указано минимальное количество, может быть больше):
     - `<header>`, `<main>`, `<footer>`
     - шесть элементов `<section>` (по количеству секций)
     - только один заголовок `<h1>`
     - шесть заголовков `<h2>` (по количеству секций)
     - шесть заголовков `<h3>` (по количеству карточек)
     - два элемента `<nav>` (основная и вспомогательная панель навигации)
     - три списка `ul > li > a` (основная и вспомогательная панель навигации, ссылки на соцсети)
     - одиннадцать кнопок button (шесть из них в секции `Video`, пять в секции `Tickets`)
     - три тега `input type="radio"` (в секции `Tickets`)
     - два тега `input type="number"`(в секции `Tickets`)
     - два тега `input type="range"` (громкось и прогрес-бар видео)
     - для всех элементов `<img>` указан обязательный атрибут `alt`
3. Вёрстка соответствует макету
   - блок `<header>`
   - секция `Welcome`
   - секция `Visiting`
   - секция `Explore`
   - секция `Video`
   - секция `Tickets`
   - секция `Contacts`
   - блок `<footer>`
   - допускается отклонение вёрстки от макета до 10px по горизонтали и вертикали, если соблюдается визуальное сходство вёрстки и макета. Разрешены и даже приветствуются правки размеров и расположения криво нарисованных блоков.
   - в качестве инструмента для проверки соответствия вёрстки макету используйте расширение [PerfectPixel](https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi?hl=ru)
   - при проверке вёрстки при помощи расширения PerfectPixel в первую очередь убедетесь, что в расширении выставлен масштаб 1, в браузере и операционной системе - масштаб 100%
   - если разрешение экрана 1920рх и больше, для проверки вёрстки на соответствие макету достаточно вручную выставить макет по верхнему левому углу направляющих
   - если разрешение экрана меньше 1920рх, для проверки используем device toolbar браузера Google Chrome в режиме responsive
   - каждый блок и секция рассматриваются по раздельности, т.е. недочеты предыдущего блока не переносятся на следующий, а при переходе проверки на следующий блок, мы его выравниваем с наложенным изображением
   - относительно текста проверяем его выравнивание по левому или правому краю, отступы до границы блока. Размеры текста проверяются только по высоте. Отличие в ширине слов и отступах между буквами при сопоставлении макета и вёрстки не считается ошибкой, если используется правильный шрифт с правильно указанными свойствами
4. Требования к css
   - для построения сетки используются флексы или гриды
   - при уменьшении масштаба страницы браузера вёрстка размещается по центру, а не сдвигается в сторону
   - фоновый цвет каждого блока и секции тянется на всю ширину страницы
   - иконки добавлены в формате `.svg`. SVG может быть добавлен любым способом. Обращаем внимание на формат, а не на способ добавления
   - изображения добавлены в формате `.jpg`, изображение карты добавлено в формате `.png`
   - расстояние между буквами, там, где это требуется по макету, регулируется css-свойством `letter-spacing`
   - фоновое изображение блока `Welcome` остаётся на своём месте даже если сильно уменьшить масштаб страницы
   - переключаются радиокнопки в блоке `Tickets`, одновременно может быть выбрана только одна кнопка
5. Интерактивность, реализуемая через css
   - плавная прокрутка по якорям
   - изменение стиля интерактивных элементов при наведении и клике
     - интерактивность включает в себя не только изменение внешнего вида курсора, например, при помощи свойства `cursor: pointer`, но и другие визуальные эффекты – изменение цвета фона или шрифта, появление подчёркивания и т.д.
     - если в макете указаны стили при наведении и клике, для элемента указываем эти стили
     - если в макете стили не указаны, реализуете их по своему усмотрению, руководствуясь общим стилем макета
     - обязательное требование к интерактивности: плавное изменение внешнего вида элемента при наведении и клике не влияющее на соседние элементы
     - интерактивность при наведении карточек в секции `Visiting` предусматривает плавное растягивание подчёркивания заголовка карточки на всю ширину карточки [Демо](https://raw.githubusercontent.com/rolling-scopes-school/tasks/master/tasks/images/hover.gif)
     - интерактивность при наведении иконок социальных сетей в футере предусматривает изменение цвета иконки и круглой границы вокруг иконки на золотистый

## Материалы
- [Старт в Figma для верстальщика](https://htmlacademy.ru/blog/useful/figma)
- [Инструкция по работе в Figma для верстальщика](https://breezzly.ru/guides/start-v-figma-dlya-verstalshhika)
- [Верстка сайта с нуля из Figma](https://www.youtube.com/playlist?list=PL5_s7xdj2Vsw-bCx5nOZJMFIiHwRgok--)
