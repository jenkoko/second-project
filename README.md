# Моя самостоятельная работа #

---

## Создание локального репозитория ##

---

### Что нужно для создания локального репозитория: ###

1. Создать каталог(папку) в любом месте на компьютере;
2. Например:
```
cd ~
mkdir second-project
```
3. Делаем созданный каталог репозиторием git командой
```
git init
```
4. Далее создаем файлы репозитория, например README.dm и text.txt перейдя в каталог командой cd командой
```
touch название файла
```
5. Проверяем статус командой
```
git status
```
6. Добавляем файлы в репозиторий командой
```
git add --all или

git add README.md
```
7. Делаем коммит на эти созданные файлы командой
```
git commit -m 'Комментарий добавления файлов или причина изменения'
```
8. Проверяем статус командой git status, добавленнные файлы должны быть выделены зеленым;
9. Каманда git log выводит список изменения коммитов с временем изменения коммитов и названиями
10. Далее нужно добавить локальный репозиторий который находится на компьютере в удаленный репозиторий на сайт [github.com](github.com "Один из лучших сайтов для хранения проектов")

---

# Что такое хеш #

Хеш - это индетификатор информации о создателе, время создания и изменения закоммиченного файла

Чтобы узнать хеш файла нужно вывести командой git log лог файла

---

# Сокращенный лог #

Когда в проекте много изменений для того чтобы найти нужный коммит из тысячи изменений вызывается сокращенный лог для быстрого поиска нужных изменений

Команда для вывода сокрщенного лога git log --oneline

---

# Что такое HEAD #

В папке репозитрия есть каталог .git в котором есть файл HEAD

HEAD также как и лог показывает информацию о файле:
- кем создан
- когда создан
- изменения коммитов

---

# Статусы файлов #

Когда создаешь файлы, можно через команду git status узнать о статусе фала

Статусы бывают:
- untracked (неотслеживаемый) - новый файл созданный в локальном репозитории, но который git пока не отслеживает, просто видит
- staged (подготовленный) - статус файла после команды git add, файл еще не закоммичен(не сохранен) а только добавлен к коммиту
- modified (измененный) - если внести внутри файла измнения, добавить например какой нибудь текст в текстовый файл, то статус будет измененный
- tracked (отслеживаемый) - если файл добавлен git add а также сделан коммит git commit -m, то файл будет остлеживаемый git

---

# Оформление коммита #

Оформление коммита должно быть коротким и информативным, так как в большинстве случаев в репозитории Git работают командой, что бы было понятно командой что кто сделал и в каком месте


