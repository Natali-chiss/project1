# Шпаргалка по Git для лучшего друга  
**Система контроля версий**, или **VCS**, — это программное обеспечение, которое помогает отслеживать изменения в программах, текстовых файлах, больших документах, веб-сайтах и так далее.  
**Git** стал незаменимым инструментом в командной работе именно благодаря возможности сохранять и «склеивать» труд разных программистов.
## Основные команды:  
---
### Навигация  
* pwd (от англ. print working directory, «показать рабочую папку») — покажи, в какой я папке;  
* ls (от англ. list directory contents, «отобразить содержимое директории») — покажи файлы и папки в текущей папке;  
* ls -a — покажи также скрытые файлы и папки, названия которых начинаются с символа .; 
* cd first-project (от англ. change directory, «сменить директорию») — перейди в папку first-project;  
* cd first-project/html — перейди в папку html, которая находится в папке first-project;  
* cd .. — перейди на уровень выше, в родительскую папку;  
* cd ~ — перейди в домашнюю директорию (/Users/Username);  
* cd / — перейди в корневую директорию.  

### Работа с файлами и папками  
* touch index.html (англ. touch, «коснуться») — создай файл index.html в текущей папке;  
* touch index.html style.css script.js — если нужно создать сразу несколько файлов, можно напечатать их имена в одну строку через пробел;  
* mkdir second-project (от англ. make directory, «создать директорию») — создай папку с именем second-project в текущей папке;  
* cp file.txt ~/my-dir (от англ. copy, «копировать») — скопируй файл в другое место;  
* mv file.txt ~/my-dir (от англ. move, «переместить») — перемести файл или папку в другое место;   
* cat file.txt (от англ. concatenate and print, «объединить и распечатать») — распечатай содержимое текстового файла file.txt;  
* rm about.html (от англ. remove, «удалить») — удали файл about.html;  
* rmdir images (от англ. remove directory, «удалить директорию») — удали папку images;  
* rm -r second-project (от англ. remove, «удалить» + recursive, «рекурсивный») — удали папку second-project и всё, что она содержит;  

### Репозиторий  
* git init (от англ. initialize, «инициализировать») — инициализируй репозиторий;  
* git add todo.txt (от англ. add, «добавить») — подготовь файл todo.txt к коммиту;  
* git add --all (от англ. add, «добавить» + all, «всё») — подготовь к коммиту сразу все файлы, в которых были изменения, и все новые файлы;  
* git add . — подготовь к коммиту текущую папку и все файлы в ней;  
* git commit -m "Комментарий к коммиту." (от англ. commit, «совершать», «фиксировать» + message, «сообщение») — сделай коммит и оставь комментарий, чтобы было проще понять, какие изменения внесены;  
* git log (от англ. log, «журнал [записей]») — выведи подробную историю коммитов;  
* git log –oneline - Сокращённый лог
* git status (от англ. status, «статус», «состояние») — покажи текущее состояние репозитория;  

### Работай эффективно  
1. Выполняй сразу несколько команд с помощью &&.  
2. Вызывай команды из буфера с помощью стрелок (↑) и (↓).  
3. Используй автозаполнение с помощью клавиши Tab.  


Хеш — идентификатор коммита.

HEAD — последний коммит.

### Жизненный цикл проекта (его статусов):


```mermaid
graph LR;
untracked --"git add" --> staged (+ tracked);
staged -- "git commit" --> tracked;
```


Когда освоишь Git не забывай про [меня](https://github.com/Natali-chiss):)
