[< на главную](./readme.md)

---
## Установка и настройка GIT
Для начала работы нам нужно установить сам [GIT](https://git-scm.com/), проверить установлен ли у вас GIT можно с помощью команды `git version`

```
C:\Users\User>git version
git version 2.38.0.windows.1
```

Для того чтобы завершить настройку нужно установить имя пользователя, а так же e-mail пользователя, для этого необходимо выполнить команды `git config --global user.name` и `git config --global user.e-mail`

```
C:\Users\User>git config --global user.name alex

C:\Users\User>git config --global user.e-mail alex@gmail.com
```

С настройкой разобрались, теперь можно создать репозиторий и загрузить в него данные.

---
[Создание репозитория и добаление данных >](./create.md)