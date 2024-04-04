# Команды для Git  
-----


"**pwd**" - _показывает в какой папке в данный момент находимся._ 
*****

"**cd**" - сменить директорию (от англ. change directory — «сменить директорию») 


"**cd ~**" - возвращаемся в домашнию директорию.  


"**ls**" - (лс)  отобразить содержимое директории в которой сейчас находимся (от англ. list directory contents — «отобразить содержимое директории в которой сейчас находимся»).  


"**cd [название папки]**" - переходим в указаннную директорию(папку)  


"**cd ..**" - переходим на уровень выше (возвращаемся на одну директорию назад.)   


"**cd [название папки]/[название папки]**" - переходим через несколько директорий  


"**ls -a**"  - вывести расширенный список. В нём отобразятся все скрытые файлы, которые начинаются с символа . (например, файлы конфигурации). В том числе два особых файла . и .., которые обозначают текущую и родительскую директории.  


"**ls ~**" -  выведет содержимое домашней директории вне зависимости от того, что показывает pwd  


"**ls ..** " - покажет содержимое родительской директории.  


"**touch [Имя файла.расширение(пример txt)]**" -  для создания файла  


"**mkdir [Имя папки]**" - Для создания директорий (папки) через терминал  (от англ. make directory — «создать директорию»).  


"**mkdir -p [Имя папки/Имя папки/Имя папки]** " - создать целую структуру директорий (папок) одной командой  


"**cp**" - копировать  (от англ. copy — «копировать»).  


**cp что_копируем куда_копируем**  ($ cp index.html src/)  


**cp что_копируем что_копируем что_копируем куда_копируем**  ($ cp index.html style.css script.js src/)  
скопировали три файла (index.html, style.css и script.js) в папку src  


"**mv**" - переместить (от англ. move — «переместить»).  


"**cat [Имя файла]** " - Чтобы прочитать файл, в консоль нужно ввести cat (от англ. concatenate and print — «объединить и распечатать») вместе с именем файла. Команда распечатает то, что содержится в нём.(только текстовые файлы) 
**cat myfile.txt** # распечатали содержимое файла myfile.txt  


"**rm [Имя файла]**" - Чтобы удалить файл, нужно напечатать команду rm (от англ. remove — «удалить») и передать ей имя файла.
**rm example.txt** # удалили файл example.txt из текущей папки   



"**rmdir [Имя папки]**" - Удалить папку можно командой rmdir (от англ. remove directory — «удалить директорию»). Не забудьте указать имя папки.
$ **rmdir** *images* # команда удалит папку images из текущей директории  


"**rm -r [Имя папки]**" - Удаления папки с содержимым внутри (-r — от англ. recursive, «рекурсивный») 
$ **rm -r** *images* # удалили папку images со всем её содержимым из текущей директории  


"**git add [Имя файла]** " - Подготовить файлы к сохранению (коммиту)  (отдельно файл)
"**git add --all**" - Подготовить файлы к сохранению  (коммиту)  (все файлы в папке)
"**git add .** " - Подготовить файлы к сохранению (коммиту)  (всю папку)  


"**git status**  " - покажи текущее состояние репозитория.(папки)  


"**git commit -m** "Текст что изменено" " - сделай коммит и оставь комментарий, чтобы было проще понять, какие изменения внесены.  (от англ. commit, «совершать», «фиксировать» + message, «сообщение»)  


"**git log** " - увидеть все отсалвенные коммиты (от англ. log — «журнал [записей]»).  


"**git init** " - (от англ. initialize, «инициализировать») — инициализируй репозиторий.  

