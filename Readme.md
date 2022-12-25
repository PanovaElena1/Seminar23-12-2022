# Инструкция по работе с GIT

## Что такое GIT? 
***Git*** - самая популярная реализация распределенной системы контроля версий (версионность поддерживается и на сервере, и у каждого клиента). Самой распространенной реализацией ***Git*** является !(GitHub)[https://github.com]



## Подготовка репозитория
Для создания репозитория используется команда "Git init". Для этого необходимо открыть в терминале папку с будущим репозитерием и написать "git init".



## Создание коммита
Для создания новой фиксации коммита используется команда "git commit". Для этого в терминале с папкой-репозиторием пишем "git commit -m "Сообщение к коммиту". Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***


### Добавление файлов к коммиту
Для добавления файлов к новому коммиту, используется комманда "git add". Используется она следующим образом: в терминале с папкой-репозиторием пишем "git add название файла".


## Перемещения между коммитами

## Перемещения между "сохранениями"
Для перемещения на другую фиксацию (Коммит) используется команда "git chechout". Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти нужный коммит и его хэш (номер), после чего в терминале с папкой-репозиторием неободимо написать "git checkout" хэш коммита". После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать "git checkout master".

## Журнал изменений
Для просмотра историй изменений используется команда "git log". Для этого в терминале с папкой-репозиторием необходимо написать "git log".


## Ветки в GIT

## Слияние веток и разрешение конфликтов

## Удаление веток