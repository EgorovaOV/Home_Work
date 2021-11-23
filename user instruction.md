# Что такое git
*Это система контроля версий.Сохраненяет файлы,помогает работать в команде через создание новых веток для каждой отдельной задачи*

# Подготовка репизитория:
*настройка имени и почты:*
* git config user.name
* git config user.mail

*Инициализирует локальный репозиторий:*
* git init


# Создание сохранений
*Для того, чтобы добавитьфайлы к комиту:*
* git add file name

*Для добавления всех файлов к коммиту:*
* git add .

*Для того, чтобы зафиксировать изменения:*
* git commit -m "some info about commit"

*Если мы хотим добавиь к коммиту все файлы:*

* git commit -a -m "some info about commit"

# Проверка состояния репозитория
*Для того, чтобы проверить состояние репозитория, используем:*
* git status

*В результате использования команды видим сообщение о том, на какой ветке находимся, и какие изменения внесли.*

*Если изменения мы вносили, но видим сообщение __nothing to commit, working tree clean__, то мы просто не сохранили внесенныее изменениия, сделаем это, нажав ctrl+s.*

# Перемещения между сохранениями
*Чтобы перейти к нужному коммиту, используем:*
* git checkout __первые четыре знака коммита, к которому хотим перейти__

*А если хотим вернуться обратно в текущую версию, то используем:*
* git checkout

# Журнал изменений

# Ветки в git
*Показывает все ветки:*
* git branch

*Создание новой ветки:*
* git branch branch_name 

*Переход между ветками:*
* git checkout branch_name

# Слияние веток и решение конфликтов 
* git merge branch_name

 Добавит информацию из ветки branch_name c в текущую ветку
 
 *Конфликт веток решается с помощью ручного изменения файла и комита с этими изменениями*

# Удаление веток
*Команда branch с тегом -d удалит ветку с именем branch name:*
* git branch -d branch name

# Справка
*Вызывается с помощью --help, примеры:*
* git log --help
* git commit --help

# Работа с удаленными репозиториями

1. Создаем аккаунт на Github.com
2. Создаем локальный репозиторий.
3. "Подружить" локальный и удаленный репозитории. Github при создании нового репозитория подскажет, как это сделать.
4. Отправить с помощью команды push ваш локальный репозиторий в удаленный на github, при этом, возможно, надо авторизоваться на удаленном репозитории.
5. Провести изменения с другого рабочего места.
6. Выкачать pull актуальное состояние из удаленного репозитория.

# Если хотим помочь какому-либо проекту.

1. Находим репозиторий, для которого хотим предложить изменения, и делаем его fork.
2. Создаем свою локальную копию этого репозитория с помощью команды git clone (ссылка на форкнутый репозиторий).
3. Создаем ветку с предлагаемыми своими изменениями, делаем в ней свой вариант.
4. Отправляем изменения на свой аккаунт на github командой push.
5. Из своего аккаунта отправляем pull request со своими изменениями автору первоначального репозитрия с сопроводительной запиской.


