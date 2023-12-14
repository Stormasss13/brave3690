#Инструкция по работе с Git.

##Основные команды Git для работы в локальной сети.

###Создать репозиторий в папке на локальной машине:
```sh
git init
```

###Проверяем статус файла:
```sh
git status
```

###Отслеживать добавленные файлы:

Сохранение одного файла:
```sh
git add <имя файла>
```

Сохранение всех файлов сразу:
```sh
git add .
```

###Сохранить текущее состояние:
```sh
git commit -m <"комментарий">
```

###Сливаем 2 предыдущие команды в 1 общую("git add ." + "git commit -m"):
```sh
git commit -am <"комментарий">
```

###Вызывать список коммитов:

Полная версия:
```sh
git log
```

Упрощенная версия:
```sh
git log --oneline
```

Отображение в виде графа/дерева:
```sh
git log --graph
```

###Показать разницу между версиями:
```sh
git diff
```

###Работа с ветками:

Проверерка, на какой ветке мы находимся в данный момент:
```sh
git branch
```

Создание ветки:
```sh
git branch <название новой ветки>
```

###Переключиться между разными версиями:
```sh
git checkout <имя ветки/имя коммита>
```

###Слияние веток:
```sh
git merge <имя ветки для слияния с текущей>
```

###Удаление веток:
```sh
git commit -d <имя ветки>
```

#Доп материалы:

Сайт для тренировки:

https://learngitbranching.js.org/?locale=ru_RU

#Работа удаленно с GitHub

###Копируем репозиторий из GitHub в локальный репозиторий на компьютере:
```sh
git clone <ссылка с GitHub>
```

###Связываем локольный репозиторий с удаленным:
```sh
git remote add origin <ссылка на удаленный репозиторий>
```

###Указываем основную ветку для удаленного репозитория:
```sh
 git branch -M main
```

###Направляем содержимое локального репозитория на удаленный:
```sh
git push -u origin main
```

###Слияние удаленного и локального репозитория:

```sh
git pull
```

##Как отправить свое предложение другому пользователю:
1. Делаем форк (fork) интересующего нас репозиторя.
2. Делаем ```git clone``` для нашей версии этого репзитория.
3. Создать ветку с предлагаемыми изменениями.
4. Производим все изменения только в этой ветке.
5. Отправляем эти изменения на свой аккаунт (push).
6. Далее в GitHub появляется возможность отправить pull request.