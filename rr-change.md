[< на главную](./readme.md)

[< Работа с удаленным репозиторием](./remote-repository.md)

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

---
* [Как подключиться к удаленному репозиторию?](./rr-connection.md)
* [Как полностью клонировать удаленный репозиторий?](./rr-clone.md)
* [Как клонировать изменения с удаленного репозитария?](./rr-pull.md)