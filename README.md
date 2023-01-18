# GIT

### архитектура директории .git

```
|__.git
    |__branches(ветки)
    |__config(конфигурация репозитория)
    |__description(поимание)
    |__HEAD(содержит ссылку на текущую ветку, в данный момент это должна быть ветка master.)
    |__hooks(выполняемые команды при коммите)
    |__info(информация)
    |__objects(объекты)
    |__refs(информация о ветках и тегах)
```

### команды

|команда|описание|пояснение|
|---|---|---|
|git init|инициализация репозитория||
|git config --list|конфигурация репозитория|В этом файле хранятся настройки Git. Всего таких файлов три:```/etc/gitconfig``` — содержит общие для всей системы настройки.```~/.gitconfig``` — содержит настройки для вашего пользователя.```.git/config``` — находится в папке репозитория. В нём указаны настройки конкретного проекта.|
|git status|отображение состояния репозитория|untracked(не отслеживается vcs)->staged(```git add```==добавление изменений в индекс)->commited(```git commit```==фиксация изменений [Как сделать новый коммит](./commmit_help.md))

сообщение при добавлении изменений в индекс
```
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.md

nothing added to commit but untracked files present (use "git add" to track)
```

ответное сообщение:
```
[master (root-commit) dcf53ed] Добавлен README.md
 1 file changed, 35 insertions(+)
 create mode 100644 README.md
```

команда|описание|пояснение|
|---|---|---|
|git log|вывод лога коммитов||

* Стандартный вывод команды log содержит полный хеш коммита, данные автора, дату и описание изменений. У команды log широкий набор инструментов для форматирования — ознакомьтесь с [документацией](https://git-scm.com/book/ru/v2/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D1%8B-Git-%D0%9F%D1%80%D0%BE%D1%81%D0%BC%D0%BE%D1%82%D1%80-%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D0%B8-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%D0%BE%D0%B2)

```
commit d48dbb6bd7472f15844e55608a8b2058e285669e (HEAD -> master)
Author: Sergey Bilibin <s.bilibin2017@yandex.ru>
Date:   Wed Jan 18 09:38:12 2023 +0300

    Добавлена информация о команде commit

commit dcf53edab6e7b3a18a1f5f29e47e05a1722f19da
Author: Sergey Bilibin <s.bilibin2017@yandex.ru>
Date:   Wed Jan 18 09:27:52 2023 +0300

    Добавлен README.md
```






