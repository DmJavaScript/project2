# project2
![Version][shield-version]
[![Build status][shield-build]][info-build]

Одностраничный сайт "Научиться учиться", посвящённый техникам и способам обучения. Свёрстан в рамках учебной программы Яндекс.Практикума.
## Стек: HTML, CSS (Flexbox).

### Сайт сейчас содержит:
* Анимацию фоновых фигур на CSS
* Отзывчивую вёрстку, шириной от 1600 px до 1100 рх
* iframe-видео с использованием YouTube API IFrame
* Оптимизированные изображения через сервисы tinypng.com, iloveimg.com/resize-image/resize-svg

### В проект возможны добавления в будущем:
* Добавить в Readme инструкции по развёртыванию
* Улучшить доступность сайта согласно a11y (tabindex (для навигации с клавиатуры))
* Добавить подключение системных шрифтов
* JS-скролл (при удалении от секции header произойдёт размытие картинки “опять двойка”)
* JS-анимация (при появлении секции technics картинки будут “потрясываться” до момента полного 	открытия секции)
* JS-эффект падающего снега из курсора с эффектом боке, на чёрных секциях kaufman и footer
* ООП для класса с генерацией падающего снега
* БЭМ для CSS, JS (модули на каждую фичу)

### Использованные материалы и полезные для будущих изменений:

* [`Курс Яндекс.Практикум`](https://praktikum.yandex.ru/)
* [`Доступность a11y`](udacity.com/course/web-accessibility--ud891) <https://medium.com/web-standards/pragmatic-a11y-rules-b16dd2f77685>
* [`В HTML сделать имена файлов к альтернативным изображениям для поддержки Retina дисплеев`](webdesign.tutsplus.com/ru/tutorials/quick-tip-how-to-use-html5-picture-for-responsive-images--cms-21015)



##Инструкции по развёртыванию:

#### установить Git для вашей операционной системы
Его необходимо скачать с официального сайта <https://git-scm.com/downloads>

#### используя утилиту Git Bash
склонировать проект напрямую в свой репозиторий командой
```shell
git clone https://github.com/DmJavaScript/project2.git
```

установите все необходимые плагины с помощью автоматической пакетной установки,  для этого достаточно ввести команду
```shell
npm install  (используемые в проекте плагины подтянуться из списка установки файла package.json При желании вы можете изменить их список или установить более свежие версии плагинов. Для этого необходимо установить знак ^ (каретки) перед необходимыми плагинами в файле package.json Например, "cross-env": "^6.0.3",)
```


#### Полезно знать следующее:
Для запуска локальной сборки проекта необходимо в Git Bash ввести команду
```shell
npm run build  (cборка проекта скомпилируется в директории dist/) тогда Вы сможете отнести собранный проект и он запустится локально без дополнительных программ
```

Для работы с проектом в режиме разработки можете воспользоваться командой
```shell
npm run dev  (запускает локальный сервер разработки сайта с обновлениями изменений в реальном времени)
```

Для внесения изменений на уже развернутом проекте может использовать следующий алгоритм работы, команды
```shell
git checkout develop  (название ветки вашей разработки может быть другой, тут для примера, названа develop)
git pull origin develop  (актуализация информации по этой ветке)
git status (показывает какие файлы вы уже изменили и которые будут отправлены на сервер при следующих действиях)
git add .  (в очередь на загрузку ставятся все изменения, что Вы произвели в проекте! Это относится и к удаленным вами файлам)

git commit -m 'описываете здесь то, что добавили в очередь на загрузку'
git tag -a git v0.0.1 -m 'описание содержания версии коммита для внешних пользователей' (текст в дальнейшем можно будет отредактировать, важно ставить новер версий и соблюдать нумерацию. В последней части команды можно проставлять контрольную сумму или часть от неё)

git push origin develop   (запускаете процесс отправки подготовленных данных на сервер. Обращайте внимание на название ветки в которой произвдите изменения. Стоит develop в качестве примера)
git push origin v0.0.1    (отправьте своё описание версии на сервер. Если забыли это сделать, можно, но нежелательно делать это одной командой git push --tags  команда отправляет все неотправленные ранее теги на сервер)
```

финально страхуетесь командой
```shell
git pull origin develop (если всё в порядке, то придет ответ от сервера, что информация в актуальном состоянии)
```





## Минимальные системные требования:

Русский язык в операционной системе для правильного отображения шрифтов.

Компьютер с установленным на нём одним из перечисленных ниже браузеров.
Версии браузеров поддерживаются начиная от:
* edge: "17",
* firefox: "60",
* chrome: "64",
* safari: "10"

### ссылка на мой репозиторий https://github.com/DmJavaScript/project2