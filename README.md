### Главные слова  

----  

Здесь пойдёт речь о всяком  
Приветствую вас  
```python
print("Хело")  
```  
# Это был код, вы знали?


Ладно вернёмся к теме
# Тема
Вот список команд и их краткое описание
- cd перейти в каталог
- pwd путь каталога, в котором ты находишься
- ls содержимое папки, модификатор -a даёт возможность просмотреть невидимые файлы

----

- git init создать локальный репрозиторий, это будет та папка в которой ты находишься
- git add добовляет файлы, как бы подготавливает к сохранению, можно использовать модификатор --all, чтобы зарядить сразу все файлы
- git commit сохраняет изменения, обычно используют модификатор -m, чтобы добавить комментарий к изменениям

----
 
Это ещё не всё. Чтобы работать с гитхабом нужно туда зарегистрироваться, потом создаёшь удалённый репозиторий и ещё надо до этого было авторизоваться в gitе с помощью  
- git config --global user.name
- git config --global user.email  
Так. Теперь мы создаём ключ ssh и связываем его с удалённым репозиторие, а потом уже мы используем команду
- git push  
Указывая имя, какой локальный репозиторий хотим запушить в удалёнку
# Вот и не всё


### Дальше мы рассмотрим как читается git status и git log.  
git status очень полезная штука и сообщает нам много полезного. Дело в том, что у Файлов есть статусный модификатор, который подсказывает нам, что мы с этим файлом делали. Только что созданным файлам даётся статус untracked, тем что уже как-то отслеживаются tracked. Изменённым файлам modificated, а которые уже отправлены на комит staged.  

----

git log выдаёт подробную информацию о всех комитах. Можно также запросить сокращённую версию, если слишком много комитов, тогда оно намного компактнее изображается с сокращённым хешом. Хеш и комит однозначано взаимоопределяются. Есть также в файлах гита HEAD, который хранит ссылку на новейший комит.

----

### Продолжение
- git commit --amend --no-edit коммитит то, что забыл в последний. при это вместо ноу эдитов можно зафигачить -m "Новое сообщение" 
- git restore --staged <file> убирает указанный засторженный файл из сторжа, если не указывать ничего то все файлы папки сбросятся
- git reset --hard <commit hash> откатываем комит до указанного хеша
- git restore <file> убирает модификации файла, который не старжлся и ничего с ним кроме модификаций не было


.gitignore - файл, в котором перечислены файлы, которые будут игнорироваться системой git в связи с этим есть некоторые шаблоны:
- * сколько угодно символов
- ? один символ
- […] тож самое что и вопрос, только теперь мы задаём список символов, которые нас не устраивают
- / это обозначение каталога
- ** то ж самое что и одинароное, но оно работает с вложенными каталогами
- ! обозначает какие вариации наоборот нельзя игнорировать 

----

- git log feature/add-txt --oneline выводит сколько коммитов былов в ветке feature/add-txt
- git branch количество веток
- git checkout переносит в нужную ветку
- git merge <название_ветки> объединяет основную ветку с данной
- git branch -D <название_ветки> удаляет не нужную ветку, после слияния, обычно