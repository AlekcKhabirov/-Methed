echo "# -Methed" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/AlekcKhabirov/-Methed.git
git push -u origin main

#запушить
git remote add origin https://github.com/AlekcKhabirov/-Methed.git
git branch -M main
git push -u origin main
 
 #дополнения
git-config
Действия после установки git
посмотреть настройки
git config --list
git config --global user.name “имя”
git config --global user.email “почта”


git config --global core.safecrlf warn
git config --global core.quotepath off
git config --global init.defaultBranch main # Ветка по умолчанию
windows
git config --global core.autocrlf true
MAC & UNIX
git config --global core.autocrlf input
Действия при инициализации нового репозитория и при работе с ним
инициализация git репозитория
git init
текущее состояние репозитория
git status
добавить в трек (отслеживаемые) файл или папку
git add index.html
добавить все файлы из корня в трек
git add .
выполнить коммит (сделать слепок) текущего состояния проекта
git commit -m "сообщение"
git log --oneline  посмотреть историю коммитов

### показывает изменения
```shell
git diff
git diff --color-words // показывает по строкам изменения
отменить коммит "ПЕРЕПИСЫВАЕТ ИСТОРИЮ"
вернуться к коммиту старому но оставить текущие изменения
git reset 'HASH commit'
вернуться к коммиту и удалить все изменения
git reset --hard 'HASH commit'
откатить изменения у всех файлов трека
git checkout .  
git checkout name.file  // откатить изменения в одном файле или каталоге
откатить изменения в одном файле или каталоге
git checkout name.file
отправить изменения в удаленный репозиторий
git push 
клонирование репозитория
git clone https://github.com/AlekcKhabirov/-Methed.git
сохраняет изменения отслеживаемых файлов и выполняет коммит
git commit -a -m 'сохраняет изменения отслеживаемых файлов и выполняет коммит

#дополнения LVL2
# GIT LVL 2
### Получение изменений с Github
```shell
git pull --rebase
```
### Восстановление файла
```shell
git restore index.js
```
### Восстановление файла
```shell
git log # логи
git log -p # логи с diff
```
### Посмотреть коммиты файла
```shell
git blame README.md
```
### Поиск подстроки в файлах
```shell
git grep строка
```
### Откатить изменения до коммита
```shell
git reset
git reset --hard HEAD~
```
### Дописать последний коммит
```shell
git commit --amend
```
### путешествие по коммитам
```shell
git checkout <хеш коммита>
git checkout main # вернуться
```
### путешествие по коммитам
```shell
git stash # убрать в stash
git stash pop # достать из stash
```
git log --graph # просмотр в виде графика
git log --graph --oneline # просмотр в виде удобного графика
### работа с ветками
```shell
git checkout -b {имя ветки} # создать новую ветку
git checkout main # перейти в ветку
git merge {имя ветки} # слить ветку
```
