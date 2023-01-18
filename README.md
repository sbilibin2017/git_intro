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

|команда|описание|
|---|---|
|git init|инициализация репозитория|
|git config user.name|имя репозитория|
|git config user.email|имейл репозитория|
|git status|отображение состояния репозитория|
```On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.md

nothing added to commit but untracked files present (use "git add" to track) ```
|git status|отображение состояния репозитория|
