# Инструкция по работе с GIT

## Первоначальная настройка GIT

У гита есть настройка пользователя, от которого будет идти работа. Это разумная и необходимая вещь, так как когда создается коммит, гит берет именно эту информацию для поля Author.

Чтобы настроить имя пользователя и пароль для всех проектов, нужно прописать следующие команды:

git config --global user.name ”Ivan Ivanov”

git config --global user.email ivan.ivanov@gmail.com

## Основные команды GIT

* git init – инициализация локального репозитория
* git status – получить информацию от git о его текущем состоянии
* git add – добавить файл или файлы к следующему коммиту
* git commit -m “message” – создание коммита.
* git log – вывод на экран истории всех коммитов с их хеш-кодами

## Команды ветвления

* git branch — это своего рода “менеджер веток”. Она умеет перечислять ваши ветки, создавать новые, удалять и переименовывать их.

>git branch Test - создание ветки Test

* git checkout - используется для переключения веток и выгрузки их содержимого в рабочую директорию.

>git checkout Test - переключение на ветку Test

* git merge - используется для слияния одной или нескольких веток в текущую. Затем она устанавливает указатель текущей ветки на результирующий коммит.

>git merge Test - команда для слияния в текущую ветку ветку Test

## Команды удаленного подключения

* git clone <url-адрес репозитория> – клонирование внешнего репозитория на локальный ПК

* git remote add NAME http://URL.COM - указание удаленного репозитория  для связки с локальным

* git branch -M main - указание какая ветка основная

* git push NAME main - загрузка текущего репозитория на удаленный

* git pull – получение изменений и слияние с локальной версией

* git push – отправляет локальную версию репозитория на внешний