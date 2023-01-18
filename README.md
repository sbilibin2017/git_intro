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
|git config user.name|имя репозитория||
|git config user.email|имейл репозитория||
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







