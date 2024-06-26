# Команды для Git  
-----


"**pwd**" - _показывает в какой папке в данный момент находимся._ 
*****

"**cd**" - _сменить директорию (от англ. change directory — «сменить директорию»)_ 
*****

"**cd** **~**" - _возвращаемся в домашнию директорию._  
*****

"**ls**" - _(лс)  отобразить содержимое директории в которой сейчас находимся (от англ. list directory contents — «отобразить содержимое директории в которой сейчас находимся»)._  
*****

"**cd [название папки]**" - _переходим в указаннную директорию(папку)_  
*****

"**cd ..**" - _переходим на уровень выше (возвращаемся на одну директорию назад.)_   
*****

"**cd [название папки]/[название папки]**" - _переходим через несколько директорий_  
*****

"**ls -a**"  - _вывести расширенный список. В нём отобразятся все скрытые файлы, которые начинаются с символа . (например, файлы конфигурации). В том числе два особых файла . и .., которые обозначают текущую и родительскую директории._  
*****

"**ls** **~**" -  _выведет содержимое домашней директории вне зависимости от того, что показывает pwd_  
*****

"**ls ..** " - _покажет содержимое родительской директории._  
*****

"**touch [Имя файла.расширение(пример txt)]**" -  _для создания файла_  
*****

"**mkdir [Имя папки]**" - _Для создания директорий (папки) через терминал  (от англ. make directory — «создать директорию»)._  
*****

"**mkdir -p [Имя папки/Имя папки/Имя папки]** " - _создать целую структуру директорий (папок) одной командой_  
*****

"**cp**" - _копировать  (от англ. copy — «копировать»)._  
*****

**cp что_копируем куда_копируем**  _($ cp index.html src/)_  
*****

**cp что_копируем что_копируем что_копируем куда_копируем**  _($ cp index.html style.css script.js src/)  
скопировали три файла (index.html, style.css и script.js) в папку src_  
*****

"**mv**" - переместить (от англ. move — «переместить»).  
*****

"**cat [Имя файла]** " - _Чтобы прочитать файл, в консоль нужно ввести cat (от англ. concatenate and print — «объединить и распечатать») вместе с именем файла. Команда распечатает то, что содержится в нём.(только текстовые файлы) 
**cat myfile.txt** # распечатали содержимое файла myfile.txt_  
*****

"**rm [Имя файла]**" - _Чтобы удалить файл, нужно напечатать команду rm (от англ. remove — «удалить») и передать ей имя файла.
**rm example.txt** # удалили файл example.txt из текущей папки_   
*****


"**rmdir [Имя папки]**" - _Удалить папку можно командой rmdir (от англ. remove directory — «удалить директорию»). Не забудьте указать имя папки._
$ **rmdir** *images*  _команда удалит папку images из текущей директории_  
*****

"**rm -r [Имя папки]**" - _Удаления папки с содержимым внутри (-r — от англ. recursive, «рекурсивный»)_ 
$ **rm -r** *images*  _удалили папку images со всем её содержимым из текущей директории_  
*****

"**git add [Имя файла]** " - _Подготовить файлы к сохранению (коммиту)  (отдельно файл)_
"**git add --all**" - _Подготовить файлы к сохранению  (коммиту)  (все файлы в папке)_
"**git add .** " - _Подготовить файлы к сохранению (коммиту)  (всю папку)_  
*****

"**git status**  " - _покажи текущее состояние репозитория.(папки)_  
*****

"**git commit -m** "Текст что изменено" " - _сделай коммит и оставь комментарий, чтобы было проще понять, какие изменения внесены.  (от англ. commit, «совершать», «фиксировать» + message, «сообщение»)_  
*****

"**git log** " - _увидеть все отсалвенные коммиты (от англ. log — «журнал [записей]»)._  
*****

"**git log** **--oneline**" -  _Сокращённый лог, если в репозитории уже много коммитов_
*****

"**git init** " - _(от англ. initialize, «инициализировать») — инициализируй репозиторий._  
*****

**Файл HEAD** - _один из служебных файлов папки .git. Он указывает на коммит, который сделан последним (то есть на самый новый)._  
*****

**Статусы untracked/tracked, staged и modified**  
**untracked** -  _(англ. «неотслеживаемый»)  - в командной строке он будет написан так_ **Untracked files**  
**staged** - _(англ. «подготовленный»)  - в командной строке он будет написан так_ **Changes to be committed**  
**tracked** - _(англ. «отслеживаемый»)_  
**modified** -  _(англ. «изменённый»)  - в командной строке он будет написан так_ **Changes not staged for commit**  
*****

```mermaid
%% описание схемы
graph LR;
  untracked -- "git add" --> staged;
  staged    -- "git commit -m"     --> tracked/comitted;
  tracked/comitted --  "Изменения"  --> modified;
  modified -- "git add"  --> staged;

```


*****
"**git log** **--oneline**" -  _Сокращённый лог, если в репозитории уже много коммитов_  
*****

-----
# Оформление сообщений к коммитам
-----

**Примеры правильных коммитов**	

```java
_git commit -m "Исправление опечатки в заголовке главной страницы на хорватском"_  
_git commit -m "LGS-239: Дополнить список пасхалок новыми числами"_  
_git commit -m "feat: добавить подсчёт суммы заказов за неделю"_  
_git commit -m "fix: исправил ошибку в программе теслы"_  
_git commit -m "Исправить #334, добавить график температуры"_  
_git commit -m "Use library mega_lib_300"_  
```

**Для сообщений на русском языке часто рекомендуют использовать инфинитивы.**  

```java
_git commit -m "Исправить #334, добавить график температуры"_  
_git commit -m "feat: добавить подсчёт суммы заказов за неделю"_  
```

**Для сообщений на английском рекомендуется использовать повелительное наклонение** 
 
```java
_git commit -m "Use library mega_lib_300"_  
_git commit -m "Fix exit button"_  
```

*****
**Conventional Commits предлагает такой формат коммита: <_type_>: <_сообщение_>. **  

```
**feat** _(сокращение от англ. feature) — для новой функциональности;_  
**fix** _(от англ. «исправить», «устранить») — для исправленных ошибок._  
```

*****

