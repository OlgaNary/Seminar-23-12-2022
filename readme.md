# Инструкция по работе с git

## Что такое гит?
***Git*** - это самая популярная реализация распределенной системой контроля версий (версионность поддерживается и на сервере и у каждого клиента). Самой распространенной реализацией ***Git*** является (Github)[https://github.com]
## Подготовка репозитория
Для создания репозитория используется команда *git init*. Для этого необходимо открыть в терминале папку с будущим репозиторием и написать *git init*. 

## Создание коммитов


### Добавление файлов к коммиту
Для добавления файла к новому коммиту используется команда *git add*. Используется онаследующим образом: в терминале с папкой-репозиторием пишем *git add <название файла>*. 


### Создание коммита
Для создания новой фиксации (коммита) используется команда *git commit*. Для этого в терминале с папкой-репозиторием пишем *git commit -m "<сообщение к коммиту>". Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***


## Перемещение между коммитами

Для перемещения на другую фиксацию (коммит) используется команда *git checkout*. Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти необходимый коммит и его хеш (номер), после чего в терминале с папкой репозиторием нужно написать: *git checkout <хеш коммита>*. После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать *git checkout master*.


## Журнал изменений
Для просмотра истории изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*.

## Ветки в Git
Чтобы создать новую ветку в Гит используется команда *git branch <имя новой ветки>*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <имя новой ветки>.* Чтобы перейти в другую ветку нужно написать *git checkout <имя ветки>.*

## Слияние веток 
Слияние веток происходит следующим образом:
Чтобы слить две ветки используется команда *git merge <имя ветки>*. Для этого нужно, находясь в ветке "чистовика" написать в терминале *git merge <имя ветки, которую нужно добавить>*.

## Разрешение конфликтов
При слиянии веток может возникнуть ситуация, когда стратегия Гит не сработает и возникнет конфликт слияния.

## Удаление веток
