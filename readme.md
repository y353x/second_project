**At start**
---
# Для работы с GitHub необходимо создать локальный проект.
для этого:<br>
-Создать папку проекта mkdir your_project<br>
-Создать файл описания readme.md и файлы проекта<br>
-Сделать папку git командой git init<br>
-Далее совершить git add --all чтобы добавить файлы в очередь на коммит<br>
-Делаем локальный коммит git commit -m 'комментарий к коммиту'<br>
-Создаем проект на GitHub , получаем ссылку SSH<br>
-Соединяем локальный и удаленный репозитории<br>
-Далее git push и вуаля!<br>
## Немного информации о HEAD, хэш и статусах<br>
-у каждого коммита есть свой уникальный хэш<br>
-самый последний коммит называется HEAD<br>
## Статусы Git<br>
-у Git есть несколько основных статусов<br>

--amend рассчитан на работу с последним коммитом (HEAD).
Дополнить коммит новыми файлами можно с помощью git commit --amend --no-edit. Благодаря опции --no-edit сообщение к коммиту останется таким, каким и было.
Изменить сообщение к коммиту позволяет команда git commit --amend -m "Обновлённое сообщение коммита".
<br>
Команда git restore --staged <file> переведёт файл из staged обратно в modified или untracked.<br>
Команда git reset --hard <commit hash> «откатит» историю до коммита с хешем <hash>. Более поздние коммиты потеряются!<br>
Команда git restore <file> «откатит» изменения в файле до последней сохранённой (в коммите или в staging) версии.<br>