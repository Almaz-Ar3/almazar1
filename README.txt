Создание проектов
|||
git init - создает новый репозиторий Git. С ее помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий
git clone ssh://git@github.com/[username]/[repository-name].git - Создать локальную копию удаленного репозитория
___
Базовый список
|||
git status - Проверить статус
git add [file-name.txt] - Добавьте файл в промежуточную область
git add -A - Добавить все новые и измененные файлы в промежуточную область
git commit -m "[commit message]" - Зафиксировать изменения
git rm -r [file-name.txt] - Удалить файл (или папку)
___
Ветки и слияние
|||
git branch - Список веток (звездочка обозначает текущую ветку)
git branch -a - Список всех веток (локальных и удаленных)
git branch [branch name] - Создать новую ветку
git branch -d [branch name] - Удалить ветку
git push origin --delete [branch name] - Удалить удаленную ветку
git checkout -b [branch name] - Создайте новую ветку и переключиться на нее
git checkout -b [branch name] origin/[branch name] - Клонировать удаленную ветку и переключиться на нее
git branch -m [old branch name] [new branch name] - Переименовать локальную ветку
git checkout [branch name] - Переключиться на ветку
git checkout - - Switch to the branch last checked out
git checkout -- [file-name.txt] - Отменить изменения в файле
git merge [branch name] - Слияние ветки с активной веткой
git merge [source branch] [target branch] - Merge a branch into a target branch
git stash - Спрятать изменения в черновом рабочем каталоге
git stash clear - Удалить все спрятанные записи
___
Совместное использование и обновление проектов
|||
git push origin [branch name] - Отправить ветку в удаленный репозиторий
git push -u origin [branch name] - Отправить изменения в удаленный репозиторий (и запомните ветку)
git push - Отправка изменений в удаленный репозиторий (запомненная ветка)
git push origin --delete [branch name] - Удалить удаленную ветку
git pull - Обновление локального репозитория до последнего коммита
git pull origin [branch name] - Вытягивать изменения из удаленного репозитория
git remote add origin ssh://git@github.com/[username]/[repository-name].git - Добавить удаленный репозиторий
git remote set-url origin ssh://git@github.com/[username]/[repository-name].git - Установите исходную ветвь репозитория на SSH
___
Проверка и сравнение
|||
git log - Посмотреть изменения
git log --summary - Посмотреть изменения (подробно)
git log --oneline - Просмотр изменений (кратко)
git diff [source branch] [target branch] - Предварительный просмотр изменений перед объединением