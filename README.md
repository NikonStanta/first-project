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
# Вот и всё