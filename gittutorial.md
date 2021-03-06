# Инструкция по работе с Markdown

## Работа с начертанием

Чтобы задать тексту курсивное начертание, нужно до и после него поставить по одной звездочке.
*Пример курсивного начертания*

Для полужирного начертания необходимо до и после текста поставить по две звездочки.
**Пример полужирного начертания**

Эти два начертания можно комбинировать. Чтобы задать тексту полужирное курсивное начертание, нужно до и после него поставить по три звездочки.
***Пример полужирного курсивного начертания***

## Добавление различных элементов

* Работа с изображениями

Чтобы добавить картинку необходимо: поставить "!", далее в квадратных скобках указать что это за изображение, и после в круглых скобках вставить ссылку на изображение.

![мое лицо, когда попросили в инструкцию добавить картинку](https://i.pinimg.com/originals/d7/25/e1/d725e15124c4d858da4de83a94c8959a.jpg)

* Работа с таблицами 

Вертикальными палками (|) задаем колонки таблицы. Первая строка - заголовки. Вторую строку заполняем "-" и добавляем ":" до ИЛИ до/после ИЛИ после них (это определяет сторону, по которой будет выравнивание текста). Следующие строки - данные таблицы.

|Заголовок 1|Заголовок 2|Заголовок 3|
|-------------|:------------:|-------------:|
|Данные 11|Данные 12|Данные 13|
|Данные 21|Данные 22|Данные 23|

* Работа с цитатами

Чтобы выделить текст как цитату, необходимо перед ним добавить ">".
> И вот так будет отображаться цитата!

* Работа с ссылками

Чтобы добавить ссылку необходимо в квадратные скобки вписать слово, которое будет работать как гиперссылка, далее в круглые скобки вставить саму ссылку.
Если остались вопросы, то ответы на них можно найти по [ссылке](https://docs.microsoft.com/ru-ru/contribute/markdown-reference)

# Работа с Git
## О программе
Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте.

С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

Git сохраняет в памяти не файлы целиком, а разницу между ними.
## Термины
* Репозиторием называют хранилище вашего файла и историю его изменений.
* Каждая точка сохранения вашего проекта носит название коммит (commit). 
* У каждого commit-a есть hash (уникальный id) и комментарий.
* Из таких commit-ов собирается ветка. Ветка - это история изменений.

## Основные команды
* _git init_ - создает в директории пустой репозиторий
* _git status_ - отображает состояние репозитория
* _git add <название файла>_ - добавляет отдельный файл в область подготовленных файлов. С помощью клавиши "Tab" можно быстро найти название файла.
* _git commit -m"<ваше сообщение>"_ - позволяет создать сохранение. К каждому коммииту можно добавить сообщение, чтобы было понятно, какие именно изменения содержит данный коммит.

Для создания сохранения необходимо сохранить сам файл (Ctrl+S), далее добавить измененный файл через команду _git add <название файла>_ и создать коммит. **Если не соблюсти данную последовательность, то коммит может быть создан неправильно или не создан вовсе.**

* _git log_ - просмотр истории создания коммитов
* _git checkout <название коммита>_ - просмотр файла в конкретном сохранении (коммите)

## Создание новых веток и перемещение между ними
1. Чтобы создать новую ветку, необходимо ввести команду _git branch <название ветки>_
2. Для перехода между ветками можно использовать команду _git checkout <название ветки>_
## Слияние веток

1. Для осуществления слияния веток используется команда _git merge <имя ветки, которая сливается с текущей веткой>_

## Конфликты при слиянии и решения
1. Возникают при наличии противоречащих коммитов в сливаемых ветках.
## Итоги семинара

Создан конспект по изученному материалу по работе с Git:
1. Для чего нужна программа, как она работает
2. Описаны наиболее часто используемые команды
3. Рассмотрена работа с ветками (создание, слияние, конфликты)
