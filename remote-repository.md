[< на главную](./readme.md)

[< Создание репозитория и добаление данных](./create.md)

---

## Как подключиться к удаленному репозиторию?

Для того, чтобы связать созданный нами локальный репозиторий с удаленным, нужно выполнить команду `git remote add origin [ссыслка на созданный репозиторий]`

```
D:\lesson\GIT> git remote add origin https://github.com/Ararat-M/git-instruction.git
```

Иногда бывает так, что проект имеет несколько удаленных репозиториев – в таком случае каждому из них присваивается собственное имя. Главный репозитарий принято называть origin.

---

## Как отправить изменения в удаленный репозиторий?

Когда в локальном репозитарии создан коммит и мы подключились к удаленному, можно отправить его на сервер. Это нужно делать каждый раз, когда нужно обновить данные в удаленном репозитарии.

Отправка коммита осуществляется с помощью команды `git push -u origin master`, которая имеет два параметра - имя удаленного репозитория (***origin***) и ветку, в которую необходимо внести изменения (***master***).

```
D:\skillfactory\GIT> git push -u origin master
info: please complete authentication in your browser...
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (7/7), 1.85 KiB | 946.00 KiB/s, done.
Total 7 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Ararat-M/git-instruction.git
```
## Как полностью клонировать удаленный репозиторий?

Чтобы клонировать удаленный репозиторий, и получить полностью работоспособную копию нужно использовать команду `git clone [ссылка на репозиторий]`

```
D:\lesson\GIT> git clone https://github.com/Ararat-M/git-instruction.git
Cloning into 'git-instruction'...
remote: Enumerating objects: 14, done.
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 14 (delta 3), reused 14 (delta 3), pack-reused 0
Receiving objects: 100% (14/14), 4.19 KiB | 858.00 KiB/s, done.
Resolving deltas: 100% (3/3), done.
```

## Как клонировать изменения с удаленного репозитария?

В случае, если другим пользователям нет необходимости делать клон удаленного репозитария, а нужно просто получить информацию об изменениях, это можно сделать с помощью команды `git pull`

```
D:\lesson\GIT> git pull origin master
https://github.com/Ararat-M/git-instruction.git
* branch master -> FETCH_HEAD
Already up-to-date.
```

команда `git pull` скачивает только новые изменения в проекте.

---

[>]()