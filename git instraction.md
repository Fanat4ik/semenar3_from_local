# Инструкция по работе с GIT
# <image src="logo_Git.jpg" alt="">

Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок - полезно для дизайнеров.

С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все ваши репозитории хранятся в определенных папках на жестком диске.

## **<span style="color:blue"> Настройка git:</span>**
> * ## git config --global user.name "<span style="color:#c5fb03"> <ваше имя></span>"
> * ## git config --global user.email "<span style="color:#c5fb03"> <адрес_почты@email.com></span>"


## **<span style="color:blue"> Команды git:</span>**

## <span style="color:#f97804"> git init</span>

Команда *git init* создаёт git репозиторий в текущей папке

## <span style="color:#f97804"> git add</span>

Команда *git add* добавляет файл в список отслеживаемых (индексируемых) файлов

## <span style="color:#f97804"> git add .</span>

Команда *git add .* добавляет все файлы в список отслеживаемых (индексируемых) файлов


## <span style="color:#f97804"> git commit</span>

Команда *git commit* фиксирует текущую версию файла(ов) 

## <span style="color:#f97804"> git commit -a</span>

Команда *git commit -a* добавляет все файлы в список отслеживаемых (индексируемых) файлов и фиксирует текущую версию файлов

## <span style="color:#f97804"> git status</span>

Команда *git status* показываест состояние репозитория

## <span style="color:#f97804"> git status -s</span>

Команда *git status -s* показываест сокращённый вид состояния файлов в репозитории

## <span style="color:#f97804"> git log</span>

Команда *git log* показывает список commit, дату их создания и автора.

## <span style="color:#f97804"> git log -p</span>

Команда *git log -p* показывает также разницу привнесённую каждым commit

## <span style="color:#f97804"> git show <span style="color:blue"> "хэш коммита"</span></span>

Команда *git show* показывает изменения отдельного commit

## <span style="color:#f97804"> git diff</span>

Команда *git diff* показывает изменения до выполнения инициализации

## <span style="color:#f97804"> git diff --staged</span>

Команда *git diff --staged* показывает разницу между зафиксированным и инициализируемым состоянием

## <span style="color:#f97804"> git checkout <span style="color:blue"> "хэш коммита"</span></span>

Команда *git checkout* позволяет перемещаться между commit

## <span style="color:#f97804"> git checkout master</span>

Команда *git checkout master* перемещает на вершину ветки мастер

## **<span style="color:blue"> Команды для ветвления в GIT:</span>**

## <span style="color:#f97804"> git branch</span>

Команда *<span style="color:#f97804"> git branch</span>* выводит список веток, а также указывает звёздочкой, в какой ветке мы сейчас находимся.

## <span style="color:#f97804"> git branch <span style="color:blue"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git branch <span style="color:blue"> "имя ветки"</span></span>* создаёт новую ветку с заданным именем.

## <span style="color:#f97804"> git checkout <span style="color:blue"> "имя ветки"</span></span>

Команда *git checkout "имя ветки"* перемещает на вершину заданной ветки.
Ранее данная команда была описана только для коммитов.

## <span style="color:#f97804"> git checkout -b <span style="color:blue"> "имя ветки"</span></span>

Команда *git checkout -b "имя ветки"* создаёт ветку и сразу  перемещает на вершину созданой ветки

## <span style="color:#f97804"> git merge <span style="color:blue"> "имя ветки"</span></span>

Данная команда *git merge <span style="color:blue"> "имя ветки"</span>*, позволяет слить одну ветку в другую, при этом указанная в команде ветка будет слита в ту ветку, в которой сейчас была написана данная команда.

## <span style="color:#f97804"> git branch -d <span style="color:blue"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git branch -d <span style="color:blue"> "имя ветки"</span></span>* удаляет указанную ветку, если та была слита с другой.

## <span style="color:#f97804"> git branch -D <span style="color:blue"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git branch -D <span style="color:blue"> "имя ветки"</span></span>* удаляет указанную ветку, даже если та не была слита с другой.

## <span style="color:#f97804"> git log --all --oneline</span>

Команда *git log --all --oneline* показывает список commit всех веток в упрощённом виде.

## <span style="color:#f97804"> git log --all --oneline --graph --decorate</span>

Команда *git log --all --oneline --graph --decorate* показывает список commit всех веток в упрощённом виде, а также схематично изоражает струтуру дерева слева от коммитов.
