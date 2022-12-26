# Инструкция по работе с GIT

## Что такое GIT? 
***Git*** - самая популярная реализация распределенной системы контроля версий (версионность поддерживается и на сервере, и у каждого клиента). Самой распространенной реализацией ***Git*** является !(GitHub)[https://github.com]

## Подготовка репозитория
Для создания репозитория используется команда "Git init". Для этого необходимо открыть в терминале папку с будущим репозитерием и написать "git init".

## Создание коммита
Для создания новой фиксации коммита используется команда "git commit". Для этого в терминале с папкой-репозиторием пишем "git commit -m "Сообщение к коммиту". Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***

### Добавление файлов к коммиту
Для добавления файлов к новому коммиту, используется комманда "git add". Используется она следующим образом: в терминале с папкой-репозиторием пишем "git add название файла".

## Перемещения между "сохранениями"
Для перемещения на другую фиксацию (Коммит) используется команда "git chechout". Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти нужный коммит и его хэш (номер), после чего в терминале с папкой-репозиторием неободимо написать "git checkout" хэш коммита". После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать "git checkout master".

## Журнал изменений
Для просмотра историй изменений используется команда "git log". Для этого в терминале с папкой-репозиторием необходимо написать "git log".


## Ветки в GIT
Для более эффективной работы в команде, в том числе с черновиками, в GIT можно создавать ветки. 
Создание ветки происходит с помощью команды "git branch "название ветки". Для того, чтобы добавить информацию в нужную ветку, необходимо предварительно на нее переключится с помощью команды "git checkout "название ветки". Проверить на какой ветке мы в данный момент находимся можно с помощью команды "git branch", система подсветит зеленым цветом ветку, на которой мы в данный момент стоим. Для того, чтобы вернуться в основную ветку, необходимо воспользоваться командой "git branch master".


## Слияние веток и способы разрешения конфликтов в системе GIT
Для того, чтобы перенести информацию из одной ветки в другую, необходимо воспользоваться функцией слияния веток. Для этого необходимо встать на ту ветку КУДА нужно перенести информацию и задать команду "git merge "название ветки ОТКУДА будет перенесена информация". При несоответствии информации в ветках в процессе слияния система выдаст конфликт. GIT предложит пути разрешения конфликта путем выбора следующих опций: принять вариант 1 ветки, принять вариант 2 ветки, оставить оба варианта. При необходимости возможно отредактировать информацию вручную и сохранить изменения (Ctrl + S). После слияния веток и размерешния конфликтов желательно сделать коммит. 

## Удаление ненужных веток
Для удаления ненужных веток необходимо воспользоваться командой "git branch -d "название ветки"

## Другие команды Git и их значение
Существуют также другие команды GIT, которые необходимы для полноценной работой с системой, а именно:
**git status** - отображает состояние папки-репозитория, в т.ч. показывает файлы, которые GIT не отслеживает.
**git diff** - позволяет отследить изменения и разницу между ними
**git log --graph** - позволяет увидить движение по всем веткам 

